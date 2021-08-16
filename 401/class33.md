## <Login /> and <Auth />

### Review, Research, and Discussion

Why is the Context API useful?

The React Context API is a way for a React app to effectively produce global variables that can be passed around. This is the alternative to "prop drilling" or moving props from grandparent to child to parent, and so on. Context is also touted as an easier, lighter approach to state management using Redux.

Can a component outside of a provider get its context?

To access a React context outside of the render function, we can use the useContext hook. We create the UserContext by calling the React. createContext method with a default context value. Then in the Users component, we call the useContext hook with UserContext to accxess the current value of UserContext .

What are some common use cases for using the Context API?

Some sample use cases where the Context API proves helpful are: Theming — Pass down app theme. i18n — Pass down translation messages. Authentication — Pass down current authenticated user.

Describe “Context Hell”?

Like the callback hell, usual when jQuery was used for everything, the React Context hell is the nasty code you get taking advantage of the React Context API.

### Terms

global state : In the causal domain, a global state is a set of local states which are all concurrent with each other. By concurrent, we mean that no two states have a cause and effect relationship with each other.

global context : This global context is about how concerned we are worldwide, how we make decisions about global issues and how we can act in a responsible way to make the world a better place. The opportunities and tensions provided by world- interconnectedness.

provider : Every Context object comes with a Provider React component that allows consuming components to subscribe to context changes. The Provider component accepts a value prop to be passed to consuming components that are descendants of this Provider. One Provider can be connected to many consumers.

consumer : The Consumer component allows a React component to subscribe to the context changes. The component makes the data available using a render prop.

### Preparation Materials

DEFINITION OF ROLE-BASED ACCESS CONTROL (RBAC)

Role-based access control (RBAC) restricts network access based on a person's role within an organization and has become one of the main methods for advanced access control. The roles in RBAC refer to the levels of access that employees have to the network.

Employees are only allowed to access the information necessary to effectively perform their job duties. Access can be based on several factors, such as authority, responsibility, and job competency. In addition, access to computer resources can be limited to specific tasks such as the ability to view, create, or modify a file.


EXAMPLES OF ROLE-BASED ACCESS CONTROL

Through RBAC, you can control what end-users can do at both broad and granular levels. You can designate whether the user is an administrator, a specialist user, or an end-user, and align roles and access permissions with your employees’ positions in the organization. Permissions are allocated only with enough access as needed for employees to do their jobs.

What if an end-user's job changes? You may need to manually assign their role to another user, or you can also assign roles to a role group or use a role assignment policy to add or remove members of a role group.

Some of the designations in an RBAC tool can include:

Management role scope – it limits what objects the role group is allowed to manage.
Management role group – you can add and remove members.
Management role – these are the types of tasks that can be performed by a specific role group.
Management role assignment – this links a role to a role group.
By adding a user to a role group, the user has access to all the roles in that group. If they are removed, access becomes restricted. Users may also be assigned to multiple groups in the event they need temporary access to certain data or programs and then removed once the project is complete.

Other options for user access may include:

Primary – the primary contact for a specific account or role.
Billing – access for one end-user to the billing account.
Technical – assigned to users that perform technical tasks.
Administrative – access for users that perform administrative tasks.










