# Access Control (ACL)

[5 steps to RBAC](https://www.csoonline.com/article/3060780/5-steps-to-simple-role-based-access-control.html)

**Role-Based Access Control** (RBAC) is a security model that provides a method for managing and controlling access to resources within an organization. It revolves around the concept of assigning roles to users and granting permissions based on those roles.

We care about RBAC because it offers several advantages for access control management:

- Simplified Administration, Granular Access Control, Enhanced Security, and Scalability.

A **Role/Permission hierarchy** implemented using RBAC typically consists of multiple roles, each with a set of associated permissions.

To implement RBAC:

- **Identify Roles** - Determine the different roles within the organization and define their responsibilities and required access levels.

- **Assign Permissions** - Identify the permissions required for each role.

- **Role Assignment** - specific roles based on their job responsibilities and the principle of least privilege. Users may be assigned to multiple roles if necessary.

- **Access Control Enforcement** - Implement mechanisms to enforce access control based on assigned roles and associated permissions.

[wiki - RBAC](https://en.wikipedia.org/wiki/Role-based_access_control)

- **Authorization** is the next step that determines what you are allowed to do or access based on your authenticated identity.

Three **primary rules** defined for RBAC:

- Role Assignment, Role Authorization, and Permission Authorization.

- RBAC is like a system of organized keys and locks that control who can access certain rooms or files within the company.

- Each employee is given a role, like a job title, such as "Manager," "Employee," or "Guest." These roles define what each person is allowed to do and access. For example, a manager may have access to sensitive information and can make important decisions, while an employee may have access to certain files and can perform specific tasks. A guest may have limited access and can only view certain information.

[RBAC tutorial](https://www.youtube.com/watch?v=C4NP8Eon3cA)

- Access rights are associated with the Role. Different roles have different rights to access different material.

- Access rights, or authorization, are activated after a user successfully goes through the process of authentication. Authentication verifies the user's identity to ensure they are who they claim to be.

- RBAC can bring several benefits to a business:

**Improved Security**: RBAC helps enhance security by enforcing the principle of least privilege. Users are granted access only to the resources necessary for their roles, reducing the risk of unauthorized access or accidental misuse of sensitive information.

**Simplified Access Management**: RBAC provides a structured approach to access management. Instead of individually assigning permissions to each user, access is granted based on predefined roles.

**Scalability and Flexibility**: RBAC is scalable and adaptable to changing business needs. As an organization grows or evolves, new roles can be defined and assigned without significant administrative overhead.

