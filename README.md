# GPS

The goal of this project was to minimize the time taken for the professor's commute from RIT to his home and vice versa. A bunch of GPS data in the form of text files was provided and the project was divided into three parts:
1. For the first part, a normal GPS text file was parsed and a KML file was generated that could be rendered on Google Earth to view the path. 
2. The second part involved deciding a cost function that would help in identifying the best path from RIT to home among 200 different paths. 
3. The third part was to integrate the first and second part and find out the best path. Some minor tasks were also assigned which included stop detection (red light or stop sign), turn detection, and halt detection (errands).  

The cost function designed for the project: 
Cost_function = Objective Function + Regularization 
              = (T)/30             + 1/10 * (T1 + T2 + T3)
            T = Trip time in minutes
           T1 = Total time at stop signs in minutes
           T2 = Total time spent below 20mph in minutes
           T3 = Total time spent above 60mph in minutes
           


