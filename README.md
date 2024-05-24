# This demo document is designed for the business people, software developers, and executable stakeholders to understand the standard operating process (SOP).

## 0101. User Management
### Overview
This section is responsible for creating and managing users, groups and roles. It ensures the authentication and authorization of users from different locations. It includes 
1.	User: Each user is assigned a unique identity within the context. By creating a user entity, it is ensured.
2.	User Group: To make it easier to administer a large number of users, users can be organized into named groups. Groups can in turn be assigned membership in other groups. 
3.	Authorization : After creating a user, S/he needs some permission to use the system. Each process (menu) has some action (add, edit, view, delete, etc.) that we call authorization events. This event must be permissible for authorized and responsible users. This section is to assign all kinds of authorization. 
4.	Authorization Role: Like “user group” Authorization can be grouped based on common user responsibility and assigned to user so that S/he can get a set of authorization permission.
5.	Location binding: If an organization wants the user to use the system from a definite location, the user can be assigned for specific or multiple locations from where S/he can continue his/her official operation.

### Business Constraints
1.	Single user can be assigned an authorization or authorization role so that S/he can get permissible for a set of authorization at a glance.
2.	The User Group can be assigned an Authorization role or single authorization.
### Activities 
1.	01.01.01-User creation (Insert, Update, Delete)
2.	01.01.02-Change Password
3.	01.01.03-Forget Password
4.	01.01.04-Create user group
5.	01.01.05-Assign user authorization
6.	01.01.06-Location binding
7.	01.01.07-Active / Inactive user.
8.	01.01.08-Login User

### 01.01.01-User creation
#### Process Flowchart (Insert)

![image](https://github.com/iqbaldiit/SOPs/assets/11534659/c32d412c-3178-4bc2-a757-1f58d8d29043)

#### Activity Description

![user_management_activity](https://github.com/iqbaldiit/SOPs/assets/11534659/7779d21e-67f2-40cf-9882-70b957a1077e)



### Business Constraints
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

