# [What is OAuth](https://www.csoonline.com/article/3216404/what-is-oauth-how-the-open-authorization-framework-works.html)

1. What is OAuth?
      * open-standard authorization protocol or framework that describes how unrelated servers and services can safely allow authenticated access to their assets without actually sharing the initial
2. Give an example of what using OAuth would look like.
      * when you log onto a website and it offers that you can log in with another websites credentials
3. How does OAuth work? What are the steps that it takes to authenticate the user?
      * its the process of a user prooving its ownership of identity. 
      * the steps are listed below 
            1. The first website connects to the second website on behalf of the user, using OAuth, providing the user’s verified identity.
            2. The second site generates a one-time token and a one-time secret unique to the transaction and parties involved.
            3. The first site gives this token and secret to the initiating user’s client software.
            4. The client’s software presents the request token and secret to their authorization provider (which may or may not be the second site).
            5. If not already authenticated to the authorization provider, the client may be asked to authenticate. After authentication, the client is asked to approve the authorization transaction to the second website.
            6. The user approves (or their software silently approves) a particular transaction type at the first website.
            7. The user is given an approved access token (notice it’s no longer a request token).
            8. The user gives the approved access token to the first website.
            9. The first website gives the access token to the second website as proof of authentication on behalf of the user.
            10. The second website lets the first website access their site on behalf of the user.
            11. The user sees a successfully completed transaction occurring.
            12. OAuth is not the first authentication/authorization system to work this way on behalf of the end-user. In fact, many authentication systems, notably Kerberos, work similarly. What is special about OAuth is its ability to work across the web and its wide adoption. It succeeded with adoption rates where previous attempts failed (for various reasons).
4. What is OpenID?
      * OpenID is for humans logging into machines, OAuth is for machines logging into machines on behalf of humans.

## [Authorization and Authentication flows](https://auth0.com/docs/flows)

1. What is the difference between authorization and authentication?
      * Authentication verifies the identity of a user or service, and authorization determines their access rights.
2. What is Authorization Code Flow?
      *  enables a client application to obtain authorized access to protected resources like web APIs
3. What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?
      * an OpenId Connect flow specifically designed to authenticate native or mobile application users. This flow is considered best practice when using Single Page Apps (SPA) or Mobile Apps.
4. What is Implicit Flow with Form Post?
      *  which is intended for Public Clients, or applications which are unable to securely store Client Secrets.
5. What is Client Credentials Flow?
      * With machine-to-machine (M2M) applications, such as CLIs, daemons, or services running on your back-end, the system authenticates and authorizes the app rather than a user.
6. What is Device Authorization Flow?
      * With input-constrained devices that connect to the internet, rather than authenticate the user directly, the device asks the user to go to a link on their computer or smartphone and authorize the device.
7. What is Resource Owner Password Flow?
      * Though we do not recommend it, highly-trusted applications can use the Resource Owner Password Flow, which requests that users provide credentials (username and password), typically using an interactive form.
## Videos

### Bookmark and Review

[Auth0 for single page apps](https://auth0.com/docs/libraries/auth0-react)