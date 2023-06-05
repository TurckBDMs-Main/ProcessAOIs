Step 1: Setup Turck IO-Link Master via Catalog Files
Step 2: Import AOI of device
Step 3: Call AOI in project, along with corresponding CPS commands to copy data in/out of the AOI
Step 4: Find the Process Data of the device from the Controller tags tied to the Port you are connected into in the IO-Link master.
Step 5: Type an instance name for the AOI along with the Process Data Variables. Instance names can be whatever you want and can be descriptive of the application which will make things easy to understand when you use the data throughout the program. 
Step 6: Drag and Drop Process Data Variables from the AOI to the CPS commands as necessary. 
Step 7: From the AOI, use the Ctrl+W command to open the declare variable box which will fill in the data type automatically. 3 times doing this (max) and all errors should dissapear in the rung.
Step 8: To use/control the data from/to the AOI, use the dot notation using the instance name you created in Step 5. Example <AOI_Name>.Data. So if you named the AOI AquariumSensor, you could use AquariumSensor.Temperature_F in your program when you need to use that value. 

