# Read Class 15

1. **What does it mean to authenticate a user ?**:

   - **Authentication** is the process of confirming that a user is who they say they are and that they have the right credentials to log in to a protected resource or to perform a privileged action in an application.

   - Authentication is an essential aspect of web application security. It is the process of verifying the identity of a user who is trying to access a protected resource or perform a privileged action within an application
  
   - To authenticate a user means to verify their identity. It ensures that the user is who they claim to be by validating their credentials, such as username and password.

2. **What does it mean to authorize a user?**:

   - **Authorization** is the process of granting or denying permissions to authenticated users or entities based on predefined rules and policies It determines what actions users are allowed to perform and which resources they can access within an application or system.

   - This process ensures that users have appropriate levels of access and privileges, preventing unauthorized actions and data breaches while maintaining data security and privacy.

   - To authorize a user means to grant or deny access to certain resources or actions based on their authenticated identity. It determines what a user is allowed to do within an application once they have been successfully authenticated.

3. **What are the three possible outcomes of the AuthenticationManager’s authenticate() method?**:

    - Successful authentication: The user's credentials are valid, and they are granted access.

    - Failed authentication: The user's credentials are invalid, and they are denied access.

    - Disabled or locked account: The user's account may be disabled or locked due to various reasons, such as too many failed login attempts or administrative actions.
