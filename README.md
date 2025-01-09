# JS-Chapter6
JavaScript Chapter 6 Programming Assignment

In this project you will explore how to filter the contents of one selection list based on an option chosen in another selection list. The web form you are given contains three selection lists with the make, model, and trim of cars that one might consider purchasing. Your script will link the three selection lists so that selecting a car make will filter the list of car models and selecting a car model will filter the list of car trims. A preview of the completed form in which a single car is chosen from a combination of makes, models, and trims, is shown in Figure 6-41.

![image](https://github.com/user-attachments/assets/b7c7fdf4-ad76-4c98-a8cc-862698847983)
Figure 6-41

Do the following:

Use your code editor to open the index.html and script.js files. Enter your name and the date in the comment section of each file and commit.

Go to the index.html file in your code editor and link the page to the script.js file, deferring loading of the script. Study the contents of the form. Note that the class value of each option in the Model selection list corresponds to a car company listed in the Make selection list and that the class value of each option in the Trim selection list corresponds to a model name in the Model selection list. You will use this correspondence in writing a script that filters each selection list based on the option chosen from the previous selection list. Commit your changes to the file.

Go to the script.js file in your code editor. Some of the variables and the event handlers have already been created for you but the script is not complete. You will need to create two functions: one to show all the options within a selection list and the other to filter the options within a selection list to show only those options that match a previously chosen car make or car model.

Create the showAll() function. The function has a single parameter named selectList that will represent one of the selection lists shown in the web form. Within the function do the following:

Declare a variable named options that references the collection of option elements within selectList.

Declare a variable named optionLength equal to the length of the options node list.

Add a for loop that iterates through the items in the options node list. For each item in the collection change the value of the style.display property to “block” in order to display the option within the selection list.

Create the filterSelect() function. The function has two parameters named selectList and category, where selectList will represent one of the selection lists in the web form and category will determine which options within that selection list will be displayed on the web page. Within the function do the following:

Declare a variable named options that references the collection of option elements within selectList.

Declare a variable named optionLength equal to the length of the options node list.

Add a for loop that iterates through the items in the options node list. For each item in the options collection, insert an if else statement that sets the style.display property of the item to “block” if the className property of the option equals the category variable, otherwise set the style.display property to “none” (to hide the option).

Create an onclick event handler for the selectVehicle button to run an anonymous function when clicked. Within the anonymous function, insert a command that writes the text “make model trim” to the vehicle paragraph in the web page, where make , model , and trim are the text values of the selected options from the three selection lists. (Hint: You will have to use the text property of the selected option from each selection list to return the text of the option.)

Commit your changes to the file and then open index.html in your browser.

Verify that as you select options from the Make selection list, the options in the Model selection list are filter to show only cars from that make. Verify that as you select options from the Model selection list, the Trim selection list is filtered to show only trim options for that selected model.

Verify that when you click the Select button, the text of the make, model, and trim are displayed at the bottom of the web page.
