# README.md

## Read Assignment 15

1.OAuth is an open-standard authorization protocol that allows websites to share resources or assets among users.

2. Site having one or more ways of logging in, using another website to authenticate, and once done, the website you are trying to connect/login to will log you in using the permission gained from the other website. Some DOD websites, like benefits or other VA websites, use this idea.

3. How OAuth works. Below are the steps they mentioned:
   The first website connects to the second website on behalf of the user, using OAuth, providing the user’s verified identity.
   The second site generates a one-time token and a one-time secret unique to the transaction and parties involved.
   The first site gives this token and secret to the initiating user’s client software.
   The client’s software presents the request token and secret to their authorization provider (which may or may not be the second site).
   If not already authenticated to the authorization provider, the client may be asked to authenticate. After authentication, the client is asked to approve the authorization transaction to the second website.
   The user approves (or their software silently approves) a particular transaction type at the first website.
   The user is given an approved access token (notice it’s no longer a request token).
   The user gives the approved access token to the first website.
   The first website gives the access token to the second website as proof of authentication on behalf of the user.
   The second website lets the first website access their site on behalf of the user.
   The user sees a successfully completed transaction occurring.
   OAuth is not the first authentication/authorization system to work this way on behalf of the end-user. Many authentication systems, notably Kerberos, work similarly. What is special about OAuth is its ability to work across the web and its wide adoption. It succeeded with adoption rates where previous attempts failed (for various reasons).

4. OpenID is one of the security technologies that has the same concept as OAuth. It is a single sign-in, checking, or vouching for users’ identities. It started in 2005 but was reinvented in 2014 as an authentication layer for OAuth; both "technologies now complement each other in many implementations”

5.Authentication verifies the user (who the user is), while authorization verifies what access they have or are allowed.

6. Authorization Code Flow

The user clicks Login
Auth0's SDK redirects the user to the Auth0 Authorization Server (/authorize endpoint)
Your Auth0 Authorization Server redirects the user to the login and authorization prompt
The user authenticates using one of the configured login options and may see a consent page listing the permissions Auth0 will give to the regular web application
Your Auth0 Authorization Server redirects the user back to the application with an authorization code, which is good for one use
Auth0's SDK sends this code to the Auth0 Authorization Server (/oauth/token endpoint) along with the application's Client ID and Client Secret
Your Auth0 Authorization Server verifies the code, Client ID, and Client Secret
Your Auth0 Authorization Server responds with an ID Token and Access Token (and optionally, a Refresh Token
Your application can use the Access Token to call an API to access information about the user
The API responds with requested data

      7. Mobile applications can use the Authorization Code Flow during authentication but with additional security. The OAuth 2.0 provides an Authorization Code Flow version that uses Proof of Key for Code Exchange or PKCE

       8. The Implicit Flow with Form Post, provided by OAuth 2.0, is an alternative to the Authorization Code Flow 4. This is intended for Public Clients or applications that cannot secure Client Secrets 

        9. In Client Credentials Flow, the M2M or machine-to-machine application, uses the system to "authenticates and authorizes the app rather than a user”

        10. In the Device Authorization Flow, the device asks the user to authorize the device by asking the user to go to the link through their smartphones/computers and do the authorization there.

       11. The Resource Owner Password Flow should only be used when the "redirect-based flows (like the Authorization Code Flow) cannot be used 4". It asks the users to provide credentials like username and password using an interactive form.
