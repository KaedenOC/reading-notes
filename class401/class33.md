# `<Login />` and `

[What is Role Based Access Control (RBAC)?](https://www.digitalguardian.com/blog/what-role-based-access-control-rbac-examples-benefits-and-more)

## RBAC

- **Role-Based Access Control** (RBAC) is a method of access control that defines permissions and privileges based on roles assigned to individual users or groups.

- Roles are created based on job responsibilities or functions within an organization, and permissions are assigned to these roles rather than to individual users. This approach provides a flexible and scalable way to manage access control within a system.

## Example of RBAC:

Web application that manages user accounts. The application has four main roles: User, Administrator, Manager, and Guest. Each role has specific roles and corresponding permissions:

**User Role**:

- Create: Can create a new account

- Read: Can view their own account details

- Update: Can update their own account details

- Delete: Can delete their own account

**Administrator Role**:

- Create: Can create a new account

- Read: Can view any user's account details

- Update: Can update any user's account details

- Delete: Can delete any user's account

**Manager Role**:

- Create: Can create a new account

- Read: Can view any user's account details

- Update: Can update any user's account details

- Delete: Cannot delete any user's account

**Guest Role**:

- Create: Cannot create a new account

- Read: Can view their own account details

- Update: Cannot update any account details

- Delete: Cannot delete any account

## Benefits of RBAC

- Access control simplification, Scalability, Reduced administrative overhead, Improved security,and Auditing and compliance.

## React-Cookie vs. React-Cookies

- The **react-cookie** library provides a simple API for managing cookies in React applications. It allows you to set, get, and remove cookies easily. It supports server-side rendering (SSR) and provides options for setting cookie expiration, path, domain, and secure flags.

- The choice between react-cookie and react-cookies would depend on the specific requirements and preferences of your project. Both libraries offer similar features and functionality for managing cookies in React applications. It is recommended to evaluate the documentation, community support, and any additional features provided by each library to determine which one aligns better with your project's needs.
