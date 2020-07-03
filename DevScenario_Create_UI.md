**Dev Scenario Create UI (Destruction)**
1)	Develop the create page with the header containing the title ,add the footer with two buttons
2)	Create two sections 1) Application information 2) Selection criteria (with no content)
3)	Create an input box in the application section, enhance it to a value help input box (value help only)
4)  Add a message strip in the Selection Criteria section
5)	Create a fragment containing the select dialog and add the function in the controller which would bring up the dialog on press of f4 (empty dialog box)
6)	Add the search field and the close button to close the dialog
7)	Create function in the controller to handle dialog box close event
8)	Make a call to backend API 
9)	Bind the API data with the select dialog (use custom data).
10)	Create function in controller to handle the search of an application group within the dialog box
11)	Create function in the controller to handle selection of a particular application group
12) Make an API call based on selected  application to the backend (to get the data for the selection criteria section)
13)	Create blocks dynamically in the selection criteria section based on the legal ground details obtained from the API call
	- Dynamic legal ground blocks, Processing mode block with the Radio Button Group (fixed)
14)	Create the controls in each block dynamically based on the data type of each detail of the legal ground.
15)	Bind the respective data to each of the controls (Custom data)
16)	Enhance the back end API to return the processing mode data as well.
17)	Based on the simulation condition enable or disable the radio buttons in the Processing mode block.
18)	Add the function to handle the click of the cancel button-
	- Create a confirmation message box asking if user really wants to cancel
	- Stay on the same page without keeping user input intact if No is pressed
	- Don’t commit the changes and add the navigation functionality back to the main page if yes is pressed.
19)	Add the function in the controller to handle click of the schedule button
	- Gather the data entered by the user from different sections and controls to form payload to pass to the destruction API
	- Call the API passing the data 
	- On successful display a message toast and navigate to the main screen
	- Add validations
	  - If the user has not selected the application group itself and clicks on schedule button throw up appropriate error message
	  - If the user has selected a valid application group but has left one or more of the mandatory fields under the selection criteria empty then an appropriate error message should be shown
	  - If there is any error thrown up during the API call then the appropriate error message should be displayed

