# UISpecDocument
->[Requirements](#requirements) 

->[Components](#components)

->[Layout of UI](#layout-of-ui)

->[Details of Components](#details-of-components)

->[Behavior of Page](#behavior-of-page)
#### **Requirements**
User management screen must be included list of all users. Also, addition of new user must be included. An user can be added only if user has Username, display name, phone, email and selectable user role. 

### **Components**

+ New User **Button**
+ Hide Disabled User **Checkbox**
+ Save User **Button**
+ New User **Form**
  - Username: **Label** -->> Input **Text**
  - Display Name: **Label** -->> Input **Text**
  - Phone: **Label** -->> Input **Text**
  - Email: **Label** -->> Input **Text**
  - User Roles: **Label** -->> Select **Option** ("Guest", "Admin", "SuperAdmin")
  - Enabled: **Label** -->> **Checkbox**
+ User **Table**
  - **Table Headers** : "ID", "User Name", "Email", "Enabled"

### **Layout of UI**
In the beginning of the user management screen, top navigation bar should be presented. In the navigation bar, **New User** button , **Hide Disabled User** checkbox and **Save User** button exists. These are the **must** of the user management screen.

### **Details of Components**
 #### New User **Button**

This button will be used to add another user. Example of button CSS Style is given below:
```
.button {
  background-color: lightblue;
  border: none;
  color: white;
  padding: 2px 12px;
  font-size: 15px;
  margin: 50px 50px;
  cursor: pointer;
}
```
Also, using ``` &#43; ``` html code can be classified as plus sign &#43; for New User Button.

#### Hide Disabled User **Checkbox**

This checkbox will be used to hide disabled user from user list. Example of button HTML code is given below:
```
<!DOCTYPE html>
<html>
<body>
  <input type="checkbox" id="user" name="user" value="disable">
  <label for="user">Hide Disabled User</label><br>
</body>
</html>
```

#### Save User **Button**

This button will be used to save user from new user addition content. Example of button CSS Style is given below:

```
.button {
  background-color: rgb(180,255,255);
  border: none;
  color: white;
  padding: 2px 12px;
  font-size: 15px;
  margin: 50px 50px;
  cursor: pointer;
}
```

#### New User **Form**

This form will be used to get new user contents such as Username,display name, phone, email, user role. Example of form HTML code is given [here](https://www.w3schools.com/howto/tryit.asp?filename=tryhow_css_responsive_form).

#### User **Table**

This table will be used to display all of users' ID, User Name, Email and option that user is enabled or not. Each table header have same functionality which is to order ascending or descending of that columns' data. For example, &#8593; sign means data must order ascending while &#8595; sign means data must order descending. Also if an users' enabled information `true`, this users' data will be displayed in user table.

### Behavior of Page

User Management Screen needs to handle user data and new user entry. There should be a table of user information in the content aligned to the left side of the page. Table headers need to order data of each column. Top side of the page, there should be a navigation bar which displays New User button and Hide Disabled User checkbox. Pressing New User button needs to navigate us to New User Form. Also, another button named Save User button should be appeared at the right side of the navigation bar. After filling the form, pressing Save User button has to save the user. Saved user needs to be in the user table. 

