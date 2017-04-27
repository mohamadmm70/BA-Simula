BA-Simula  is an open source numerical computational code for simulating 5MW NREL spar-type floating wind turbine but the code is flexible for further changes to implement for other spar-type wind turbines with different characteristics.

To run the model follow these steps:

1- Download BA-Simula.rar to you computer.

2- Extract BA-Simula to creat BA-Simula folder

3- Define wind turbine and invironmental properties for each modul (note that BA-Simula defualt properties are set for NREL 5MW spar-type floatint wind turbine)

4- Set the initial conditions of motion and run duration time in DES function and run the model from matlab editor section.

5- For extracting motion response frequency spectrum first save the output of BA-Simula as a .mat file then read the file from FFT time history function. Next choose each mode of motion and run the function to see the results.

Note: This code contains 25 individual functions which are coupled by EOM function with each other. Functions BEMhansen and cylinder calculates blades aredynamic induction factors for non-cylindrical airfoils and cylindrical airfols respectively using blade element momentum theory. Functions a and aa are used to call axial and tangential induction factors in F_Aero function. In a same way functions C, Cl, Cd, Clr, Cdr are used to call blade chord line length, lift and drag coefficients of airfolis and lift and drag coefficients of blade sections respectively. Functions F_Aero, F_Hydro, F_Bouyonomi, F_Mooringonomi calculate aerodynamic, hydrodynamic, bouyancy and mooring loades on system respectively. Functions Fun_nom1,2,3 calculates horizontal and vertical tensions in each mooring line by solving equations represented in functions lin1,2,3 and then F_Mooring defines the resultant mooring system load on structure. Finally, Function Load are used to calculatae loades time history that wind turbine system is subjected from load functions either individualy or resultant and function M_Power is used to estimate power production or in other words to calculate the effective moment in power generation.    
