# Authentication

## OAuth

1. **What is OAuth?**

   - A protocol or framework that allows the access between unrelated servers or services.

2. **Give an example of what using OAuth would look like.**

   - Accessing GitHUB from netlify.
  
3. **How does OAuth work? What are the steps that it takes to authenticate the user?**

   - A request token is sent to the clients software upon a third party site requests to access the website in need, Authentication is needed from client to have an access token which will be used (silently) later by the third party to access the website.

4. **What is OpenID?**

   - Having an ID that authinticates the user to access different services.

## Authentication and Authorization Flows

1. **What is the difference between authorization and authentication?**

   - Authentication is identification. Authorization is permission

2. **What is Authorization Code Flow?**

   - The exchange of authorization code for a token.

3. **what is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?**

   - Acquiring a proof key to give authorization.

4. **What is Implicit Flow with Form Post?**

   - *needs extra reading just to understand the general idea.*

5. **What is Client Credentials Flow?**

   - passing the used ID and secrets to gain authentication.  

6. **What is Device Authorization Flow?**

   - The exchange of client ID for token between devices.  

7. **What is Resource Owner Password Flow?**
 
   - The storage and use of client credentials by the server. 