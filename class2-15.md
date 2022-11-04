## Reading Notes 15

### What is OAuth

#### What is OAuth

OAuth is an *open-standard authorization* protocol that allows websites to share resources or assets among users [^1]. 

  It *describes how unrelated servers and services can safely allow authenticated access to their assets without actually sharing the initial, related, single logon credential [^1]*. It is also known as secure third-party.
  
#### Give an example of what using OAuth would look like.

An example would be a website having one or more ways of logging in, uses another website to authenticate, and once done, the website you are trying to connect/log in will log you in uisng the permission gained from the other website. Some DOD website, like benefits or other VA websites uses this idea. 

#### How does OAuth work? What are the steps that it takes to authenticate the user?

The CSO Online explained in their article [What is OAuth? How the open authorization framework works](https://www.csoonline.com/article/3216404/what-is-oauth-how-the-open-authorization-framework-works.html) how Oauth works. Below are the steps they mentioned:

- The first website connects to the second website on behalf of the user, using OAuth, providing the user’s verified identity.
- The second site generates a one-time token and a one-time secret unique to the transaction and parties involved.
- The first site gives this token and secret to the initiating user’s client software.
- The client’s software presents the request token and secret to their authorization provider (which may or may not be the second site).
- If not already authenticated to the authorization provider, the client may be asked to authenticate. After authentication, the client is asked to approve the authorization transaction to the second website.
- The user approves (or their software silently approves) a particular transaction type at the first website.
- The user is given an approved access token (notice it’s no longer a request token).
- The user gives the approved access token to the first website.
- The first website gives the access token to the second website as proof of authentication on behalf of the user.
- The second website lets the first website access their site on behalf of the user.
- The user sees a successfully completed transaction occurring.
- OAuth is not the first authentication/authorization system to work this way on behalf of the end-user. In fact, many authentication systems, notably Kerberos, work similarly. What is special about OAuth is its ability to work across the web and its wide adoption. It succeeded with adoption rates where previous attempts failed (for various reasons). 

#### What is OpenID?

OpenID is one of the security tehnologies that has same concept as OAuth. It is a single sign-in, cehcking or vouching for user's idntities. It started in 2005, but reinvented in 2014 to as an *authentication layer for OAuth*; both "technologies now complement each other in many implementations" - [^1]: [What is OAuth? How the open authorization framework works](https://www.csoonline.com/article/3216404/what-is-oauth-how-the-open-authorization-framework-works.html).


## Authorization and Authentication flows

#### What is the difference between authorization and authentication?

Authentication verifies the user (who the user is) while the authorization verifies what access they have or allowed [^3].

#### What is Authorization Code Flow?

The image and steps below are from: [Auth0 Docs: Authorization Code Flow](https://auth0.com/docs/get-started/authentication-and-authorization-flow/authorization-code-flow), it shows the authorization code flow[^4]:

![image](https://user-images.githubusercontent.com/113204667/200006609-e5668121-e3d7-4e7f-91bb-aa9f6241d69b.png)

- The user clicks Login
- Auth0's SDK redirects the user to the Auth0 Authorization Server (/authorize endpoint)
- Your Auth0 Authorization Server redirects the user to the login and authorization prompt
- The user authenticates using one of the configured login options and may see a consent page listing the permissions Auth0 will give to the regular web application
- Your Auth0 Authorization Server redirects the user back to the application with an authorization code, which is good for one use
- Auth0's SDK sends this code to the Auth0 Authorization Server (/oauth/token endpoint) along with the application's Client ID and Client Secret
- Your Auth0 Authorization Server verifies the code, Client ID, and Client Secret
- Your Auth0 Authorization Server responds with an ID Token and Access Token (and optionally, a Refresh Token
- Your application can use the Access Token to call an API to access information about the user
- The API responds with requested data


#### What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)

Mobile applications can use the *Authorization Code Flow* during autentication but with additional security. The *OAuth 2.0* provdes *Authorization Code Flow version* that uses Proof of Key for Code Exachange or known as PKCE [^2]. 

#### What is Implicit Flow with Form Post?

The *Implicit Flow with Form Post*, rovided by OAuth 2.0, is an alternative to th *Authorization Code Flow* [^2]. This is intended for Public Clients, or applications that are unable to secure Client Secrets securely [^2].

#### What is Client Credentials Flow?

In *Client Credentials Flow*, the M2M or machine-to-machine application, uses the system to "authenticates and authorizes the app rather than a user" - [^2]: [Auth0 Docs: Authentication and Authorization Flows](https://auth0.com/docs/get-started/authentication-and-authorization-flow).


#### What is Device Authorization Flow?

In the *Device Authorization Flow*, the device asks the user to authorize the device by asking the user to go to the link thourgh their smartphones/computers, and do the authorization there. - - [^2]: [Auth0 Docs: Authentication and Authorization Flows](https://auth0.com/docs/get-started/authentication-and-authorization-flow).

#### What is Resource Owner Password Flow?

The *Resource Owner Password Flow* should only be used when the "redirect-based flows (like the Authorization Code Flow) cannot be used [^2]". It ass the users to provide credentials like username and password using an interactive form [^2].


[^1]: [What is OAuth? How the open authorization framework works](https://www.csoonline.com/article/3216404/what-is-oauth-how-the-open-authorization-framework-works.html)
[^2]: [Auth0 Docs: Authentication and Authorization Flows](https://auth0.com/docs/get-started/authentication-and-authorization-flow)
[^3]: [Auth0  Docs: Authentication vs. Authorization](https://auth0.com/docs/get-started/identity-fundamentals/authentication-and-authorization)
[^4]: [Auth0 Docs: Authorization Code Flow](https://auth0.com/docs/get-started/authentication-and-authorization-flow/authorization-code-flow)

