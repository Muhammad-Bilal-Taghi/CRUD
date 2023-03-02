# CRUD (create, read, update, delete) system using JavaScript and local storage.
That allows the user to add, edit, and delete user records. The code begins by declaring variables that store references to various HTML elements, such as buttons and input fields. It also initializes an empty array to store user records, and retrieves any saved records from local storage.

The code defines a function called DisplayInfo, which generates an HTML table based on the contents of the userArray. Each row in the table represents a user record, and includes buttons to edit or delete the record. The function is called initially to display any existing records.

The addUserBtn.onclick function is triggered whenever the user clicks the "Add User" button. If the user is in edit mode (i.e. edit_id is not null), the function updates the corresponding record in userArray with the new name. Otherwise, it adds a new record to the end of the array. The function then saves the updated array to local storage, clears the input field, and reverts the button text to its original state.

The code also includes two additional functions, EditInfo and DeleteInfo, which are called when the user clicks the corresponding buttons in the table. EditInfo sets edit_id to the index of the selected record, updates the input field with the record's name, and changes the button text to "Save Changes". DeleteInfo removes the selected record from the array and calls SaveInfo to update local storage.
