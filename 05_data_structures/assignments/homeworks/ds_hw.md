### Homework Assignment: Simple Contact Manager

#### Objective:
Create a simple contact manager application in Python that utilizes tuples, lists, and dictionaries. The application should allow the user to store and manage contact information.

#### Instructions:

1. **Define a Contact Tuple**:
   - Create a tuple `contact` that holds the following information: `name`, `phone_number`, and `email`.

2. **Create a Contact List**:
   - Initialize an empty list called `contacts_list` to store multiple contact tuples.
   - Add at least three contact tuples to the `contacts_list`.

3. **Access and Display Contacts**:
   - Write a function `display_contacts` that iterates over the `contacts_list` and prints each contact's information in a readable format.
  
4. **Modify Contact Information**:
   - Since tuples are immutable, create a new list with updated contact information if any contact needs to be modified.
   - Write a function `update_contact` that takes `contacts_list`, an index of the contact to be updated, and the new information as parameters. The function should return a new list with the updated contact information.

5. **Implement List Methods**:
   - Write functions to add and remove contacts from the `contacts_list` using the list methods `append()` and `remove()`.

6. **Create a Dictionary for Quick Lookup**:
   - Create a dictionary `contacts_dict` where the keys are contact names and the values are tuples containing the contact's phone number and email.
   - Write a function `create_contacts_dict` that takes `contacts_list` and returns `contacts_dict`.

7. **Search for a Contact**:
   - Write a function `search_contact` that takes `contacts_dict` and a name as parameters and returns the contact's information if found.

8. **Main Program**:
   - Combine all the functions and implement a simple command-line interface to interact with the user, allowing them to add, update, remove, and search for contacts.

#### Submission:
Submit a single Python file `contact_manager.py` containing your implementation. The file should include:

- Definitions of all the required functions.
- A main program that demonstrates adding, updating, removing, and searching contacts.

#### Example Output:

```
Welcome to the Contact Manager!
1. Display contacts
2. Add a contact
3. Update a contact
4. Remove a contact
5. Search for a contact
6. Exit

Enter your choice: 1

Contacts:
Name: John Doe, Phone: 123-456-7890, Email: john.doe@example.com
Name: Jane Smith, Phone: 987-654-3210, Email: jane.smith@example.com
Name: Emily Johnson, Phone: 555-555-5555, Email: emily.johnson@example.com

Enter your choice: 2
Enter name: Michael Brown
Enter phone number: 222-333-4444
Enter email: michael.brown@example.com
Contact added!

Enter your choice: 5
Enter name to search: Emily Johnson
Contact found: ('555-555-5555', 'emily.johnson@example.com')
```

Feel free to expand the functionality as you see fit. Happy coding!