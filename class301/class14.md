# Authentication

[What is OAuth](https://www.csoonline.com/article/3216404/what-is-oauth-how-the-open-authorization-framework-works.html)

- **OAuth (Open Authorization)** is a widely-used protocol that enables a user to grant a third-party application access to their data or resources, without having to share their login credentials.

- One example of using OAuth is when a user wants to grant a mobile app access to their Facebook or Google account without sharing their username and password with the app. 

- The third-party application initiates the OAuth process by sending an authentication request to the authorization server.
The user is redirected to the authorization server's login page and enters their credentials.
The authorization server verifies the user's identity and prompts the user to grant or deny access to the requested resources.
If the user grants access, the authorization server issues an access token to the third-party application.
The third-party application uses the access token to access the user's resources or data.

- **OpenID** is a decentralized authentication protocol that enables a user to use a single set of login credentials to access multiple applications or websites. OpenID allows users to authenticate themselves with an identity provider (IDP) rather than having to create separate login credentials for each application or website.

[Authorization and Authentication flows](https://auth0.com/docs/get-started/authentication-and-authorization-flow)

- Authentication is the process of verifying a user's identity. Authentication is typically performed by requesting a username and password. Authorization is the process of granting or denying access to resources or data based on the authenticated user's permissions.

- redirect the user to the auth servers login page,  user enters their credentials and is authenticated by the authorization server, authorization server issues an authorization code to the client application, client application exchanges the authorization code for an access token.

- **(Proof Key for Code Exchange)** is a variation of the Authorization Code Flow that provides an additional layer of security. PKCE is designed to protect against attacks such as code injection and interception of the authorization code.

- **Implicit Flow** with Form Post is an OAuth 2.0 flow that is used to obtain an access token directly from the authorization endpoint, without the use of an authorization code. This flow is typically used by client-side applications such as mobile apps and single-page web applications.

- **Client Credentials Flow** is an OAuth 2.0 flow that is used by server-to-server applications to obtain an access token. In this flow, the client application (acting on behalf of itself) requests an access token from the authorization server using its client ID and client secret.

- **Device Authorization Flow** is an OAuth 2.0 flow that is used for devices with limited input capabilities, such as smart TVs and gaming consoles. In this flow, the device displays a user code and instructs the user to go to a URL and enter the code.

- **Resource Owner Password Flow** is an OAuth 2.0 flow that is used when the client application already has the user's credentials, such as when the user enters their username and password directly into the client application.

## Additional Resources

[Auth0 for single page apps](https://auth0.com/docs/libraries/auth0-react)

