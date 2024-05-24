![image](https://github.com/iqbaldiit/SOPs/assets/11534659/f2341cf7-f62f-4c4d-b56f-644fd14f4c7d)#Demo of a standard operating Procedure (SOPs).
This document is designed for the business people, software developers, and executable stakeholders to understand the standard operating process (SOP).

Overview
This section is responsible for creating and managing users, groups and roles. It ensures the authentication and authorization of users from different locations. It includes 
1.	User: Each user is assigned a unique identity within the context. By creating a user entity, it is ensured.
2.	User Group: To make it easier to administer a large number of users, users can be organized into named groups. Groups can in turn be assigned membership in other groups. 
3.	Authorization : After creating a user, S/he needs some permission to use the system. Each process (menu) has some action (add, edit, view, delete, etc.) that we call authorization events. This event must be permissible for authorized and responsible users. This section is to assign all kinds of authorization. 
4.	Authorization Role: Like “user group” Authorization can be grouped based on common user responsibility and assigned to user so that S/he can get a set of authorization permission.
5.	Location binding: If an organization wants the user to use the system from a definite location, the user can be assigned for specific or multiple locations from where S/he can continue his/her official operation.

Business Constraints
1.	Single user can be assigned an authorization or authorization role so that S/he can get permissible for a set of authorization at a glance.
2.	The User Group can be assigned an Authorization role or single authorization.
Activities 
1.	01.01.01-User creation (Insert, Update, Delete)
2.	01.01.02-Change Password
3.	01.01.03-Forget Password
4.	01.01.04-Create user group
5.	01.01.05-Assign user authorization
6.	01.01.06-Location binding
7.	01.01.07-Active / Inactive user.
8.	01.01.08-Login User
01.01.01-User creation
Process Flowchart (Insert)

  

Activity Description (Insert)
Step	Activity	Responsible	Description / Case / User stories
1	Request for creating users. (M)	Employee	Scenario: Once an employee has enrolled but the user is not created automatically at the time of onboarding.
Case: Employee manually fill-up a user creation form (Employee code, name, department, designation, Purpose) and request to system admin to create a user.  [Ref: MSF-01]

2	Enter Employee Information	System Admin	System admin opens the User creation interface and sets employee code to find out the employee information from the system.
3	Check Request Validity	System	System checks by the “employee code” that the employee meets the following criteria
1.	Employee existence.  
2.	Active Employee who has valid official information.
3.	Duplicate user check.
If the criteria not matched system admin may view the following message on screen
1.	For criteria 1: “Invalid Employee code. Try again!”
2.	For criteria 2: “This employee is inactive. Please activate the employee first.”
3.	For criteria 2: “Onboarding process is still incomplete. Please complete the onboarding process first.”
4.	For criteria 3: “User already exists by this employee. Login ID: <login_id>” 
4	Get Employee Information	System	After completing step 3, if the request is valid, the system will provide Employee information with employee name, phone and email.
5	Submit 	System Admin	System admin will view employee’s information at user creation interface with Auto suggested Login ID. If the user wants, S/he can change the login ID as desired but Login ID must be unique.
6	Create user record	System	Case: After submitting, System will create a new user with checking all validity (Duplicate, Uniqueness) and update the user database. If there is any inconsistency show the message of step 3.
Deliverable: Auto user password will be created. 
7	Generate Email	System	Once a record has been created successfully, the system will send an email to the Employee with user name & password. [Ref: ENF-01]


Business Constraints
1.	User login ID must be unique. [Recommended “Employee code”]
2.	One employee must not have multiple users.
3.	Employee must be active with his active official Information.
4.	If an employee exists, Phone, email and name must be matched with employee information or this information can be set while creation of user.
5.	Users can’t be deleted if the user logged in once.
6.	Only email & phone can be updated with preserving history.
7.	Users can be activated or inactivated in any time any situation.
8.	Inactive users can’t log in to the system and can’t operate any operation.
9.	If the user is not bound with location, S/he can log in from around the world.
10.	Users can be bound with multiple locations and once bound, S/he can log in the system only from a defined location or area.
11.	One user can’t exist in multiple user groups.

