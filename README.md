# Kirsch's Stresses Calculator

### Programming language
- Python 3.8

### Libraries
- Tkinter
- Numpy
- Pandas
- Matplotlib

### Scripts list
- induced_stresses_calc.py
- front_GUI.py
- load_parameters_GUI.py
- visualization_GUI.py
- export_data_GUI.py
- induced_stresses_calc_backend.py

### induced_stresses_calc.py
Is the main script, who use Tkinter for generate a GUI with 4 tabs called: "How to Use", "Load Parameters", "Visualization" and "Export Data". In addition, it has a "dark mode" that modifies the color of the widgets.

### front_GUI.py
Contain a tab called "How to Use". In this tab, through images (folder "images"), the meaning of the parameters used by the application are shown.

### load_parameters_GUI.py
Contain a tab called "Load Parameters". In this tab the inputs parameters are loaded, which are divided into: boundary boxes, excavations, stresses fields and strength parameters.

### visualization_GUI.py
Contain a tab called "Visualization". In this tab the results are shown, where you can select which variable to display from the following: 
- Major principal stress (P)
- Minor principal stress (Q)
- Max shear stress (Tmax)
- Normal stress - X-axis (Sx)
- Normal stress - Y-axis (Sy)
- Shear stress - XY-plane (Txy)
- Strength factor

### export_data_GUI.py
Contain a tab called "Export Data". In this tab you can export the result of the calculations in a .csv file, where you can select a specific variables or export an entire file.

### induced_stresses_calc_backend.py
Contain a data treatment and functions used to realize stress calculations, including Kirsch's stresses formulas, rotate functions and overlap stresses functions. Also, this script considers the following objects: "BoundaryBox", "Geometry_circle" and "Geometry_ellipse", where all of calculations are realizing in the BoundaryBox object, while the geometries are used as restrictions for the points generation and as input parameters for each Kirsch's formulae.

### How to use:
First, you must install the dependencies using this command:

`pip install -r requirements.txt`

Finally, execute the script `induced_stresses_calc.py` to deploy the app.


##### P.D.: The comments in the scripts are written in Spanish, I must translate them into English.

### Some views of the app:

<img src="https://github.com/vmyelicich/kirsch-stresses-calc/blob/master/views/Screenshot_6963.png" width="80%" height="80%"/></img>

<img src="https://github.com/vmyelicich/kirsch-stresses-calc/blob/master/views/Screenshot_6964.png" width="80%" height="80%"/></img>

<img src="https://github.com/vmyelicich/kirsch-stresses-calc/blob/master/views/Screenshot_6965.png" width="80%" height="80%"/></img>

<img src="https://github.com/vmyelicich/kirsch-stresses-calc/blob/master/views/Screenshot_6966.png" width="80%" height="80%"/></img>
