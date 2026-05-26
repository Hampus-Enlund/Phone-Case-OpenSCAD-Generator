# Phone-Case-OpenSCAD-Generator
With this repository you can generate OpenSCAD code for 3D modelling phone cases for a few pre-loaded phones. In addition, it is possible to adjust clearance and case thickness, as well as enter dimensions of other phones to quickly generate cases fitting those phones as well.

# Before running the code
- The code is made to run on jupyter notebook desktop version. It is recommended to use jupyter through the anaconda launcher as imported libraries and pop-up techniques are coded to fit this particular setup.
- Before running the code, make sure that the phone_dimensions.csv file in in the same directory as the Python Phonecase V8 file. In jupyter notebook, the .csv can be dragged to the directory to the file explorer widget on the browser the Python Phonecase V8 file is ran on.
- Note, that in  order to retrieve a .stl file with the 3D model for the phone case, you will need to have the OpenSCAD software installed.

# Running the python code
When running the code, a pop-up window will appear. Here you will be asked to enter three variables before generating the code:
- Case's thickness: This will determine how thick the back and sides of the case will be. Please enter a value in mm according to your printing setup. If unsure how much to set, around 2-5 mm is recommended. Note, that the lip thickness is not determined by this setting, and is instead determined in the phone_dimensions.csv file.
- Clearance: This will determine the clearance between the case and the phone, making sure that the phone will have a good fit in the case. Some plastics may shrink wile or after printing, so setting a proper clearance is crucial for having the phone fit. Please enter a value in mm according to your printing setup. If unsure how much to set, around 0.2 mm is recommended.
- Phone selection: This drop down menu will include all phones entered into the phone_dimensions.csv file. If you wish to use a phone not available in the drop down menu, add it to the .csv file and restart the pyhton program and it will appear.

When pleased with the settings entered, click "Generate code" and a second pop-up notifying about the success should appear. The generated .scad file will appear in your 'documents' folder with the name generated "{selected phone} case.scad". You may click "Exit program" to exit, when you've confirmed that the file has appeared as expected.

# Exporting to a .stl file in OpenSCAD
When you have the .scad file, you may open it with OpenSCAD. The phone case will generate automatically and nearly immediately and a preview should appear on the top right hand side of the window.
There is no need to change the code, although if you still wish to adjust some variables, you may do so from the list of variables in the first lines of the code and relaunch the program.
When you're satisfied with the preview, you may export the model to a .stl file and proceed with producing it.

# Other notes
The project was Created by Mattias Tallgård and Hampus Enlund as a project in a course covering engineering applications of programming.
For the dimensions of the iPhones included as pre-loaded phones, Apple's "Accessory-Design-Guidelines" document was used. Accessed May 17:th 2026 at https://developer.apple.com/accessories/Accessory-Design-Guidelines.pdf
