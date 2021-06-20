# Authentication

## What is OAuth
1. What is OAuth?

    OAuth is an open-standard authorization protocol or framework that describes how unrelated servers and services can safely allow authenticated access to their assets without actually sharing the initial, related, single logon credential.

2. Give an example of what using OAuth would look like.

    The simplest example of OAuth is when you go to log onto a website and it offers one or more opportunities to log on using another website’s/service’s logon.

3. How does OAuth work? What are the steps that it takes to authenticate the user?

    When a user has already signed into one website or service. The user then initiates a feature/transaction that needs to access another unrelated site or service.

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


4. What is OpenID?


    OpenID would serve as a single sign-in, vouching for the identities of users rather than having multiple logins for multiple websites.



# Authorization and Authentication flows
1. What is the difference between authorization and authentication?
2. What is Authorization Code Flow?
3. What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?
4. What is Implicit Flow with Form Post?
5. What is Client Credentials Flow?
6. What is Device Authorization Flow?
7. What is Resource Owner Password Flow?