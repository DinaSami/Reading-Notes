## Access Control (ACL)

### When is basic authorization used v. bearer authorization
Basic authorization is used to authenticate a user (grab authorization header, extract components, autheticate). Bearer Authorization is validating that a user has the correct token to proceed in the route, bearer authorization we are authenticating the token.

### What does the JSON web token package do
Creates a token based off of a users hashed username from the database + the app SECRET.

### What considerations should we make when creating and storing a SECRET
Storing the secret someplace secure, (.env files are good) and storing secrets with some level of encryption.


## Term

+ encryption
+ token
+ bearer
+ secret
+ JSON Web Token


## Preview :
Encryption is turning something from plain text into a undecipherable code.

Token is something that is generated unique to a user that is used to verify whether or not that user has access to certain parts of the site

Bearer the header in which tokens are passed

Secret the unique identifier of the app that is used in conjunction with the username to create a token

JSON Web Token "defines a compact and self-contained way for securely transmitting information between parties as a JSON object. This information can be verified and trusted because it is digitally signed".

### 5 steps to simple role-based access control (RBAC) :

RBAC is the idea of assigning system access to users based on their role in an organization. It's important to remember that not every employee needs a starring role.

### What is RBAC?

RBAC is nothing more than the idea of assigning system access to users based on their role within an organization. The system needs of a given workforce are analyzed, with users grouped into roles based on common job responsibilities and system access needs. Access is then assigned to each person based strictly on their role assignment. With tight adherence to access requirements established for each role, access management becomes much easier.

### Benefits of RBAC?

With the proper implementation of RBAC, the assignment of access rights becomes systematic and repeatable. Further, it is much easier to audit user rights, and to correct any issues identified.

### RBAC implementation :

Hopefully I have convinced you to take a closer look at RBAC. If so, consider the following simplified five-step approach to getting it implemented:

1. Inventory your systems

2. Analyze your workforce and create roles

3. Assign people to roles

4. Never make one-off changes

5. Audit

### Role-based access control :

Role-based access control (RBAC) restricts network access based on a person's role within an organization and has become one of the main methods for advanced access control. The roles in RBAC refer to the levels of access that employees have to the network.

### EXAMPLES OF ROLE-BASED ACCESS CONTROL :

Through RBAC, you can control what end-users can do at both broad and granular levels. You can designate whether the user is an administrator, a specialist user, or an end-user, and align roles and access permissions with your employees’ positions in the organization. Permissions are allocated only with enough access as needed for employees to do their jobs.





