# Authentication Notes

This topic is important to me because I want to create an application that gives security to my user.

## [Retrospective 15](https://connerkt.github.io/Reading-Notes/301/Class15/Retro15)

## References

[What is OAuth](https://www.csoonline.com/article/3216404/what-is-oauth-how-the-open-authorization-framework-works.html).

[Authorization and Authentication Flows](https://auth0.com/docs/flows).

[Single Page App Video](https://auth0.com/docs/libraries/auth0-react).

## What is OAuth? Notes

**OAuth** allows websites and services to share assets among users.

Its an open-standard authorization protocol or framework that describes how unrelated servers and services can safely allow authenticated access to their assets without actually sharing the single logon credential.

Created by Twitter,Google,and other companies.

This is a step by step basis on how it works:

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

### What is OAuth Questions

1. What is OAuth?
2. Give an example of what using OAuth would look like.
3. How does OAuth work? What are the steps that it takes to authenticate the user?
4. What is OpenID?

### What is OAuth Answers

1. Its a protocol that gives users access to the data on one website to another site.
2. When a user wants to sign in for twitter, but use google to sign in for them.
3. You get a token once trying to login, so we can use that token to get information back.
4. Its a way for users to authenticate and authorize themselves across different websites with only one set of credentials.

## Authorization and Authentication flows Notes

Auth0 uses the OpenID Protocol and OAuth Authorization Framework to authenticate users and get their authorization to access protected resources.

With Auth0 you can easily support different flows in your applications and APIs without worrying about ODIC/OAuth 2.0 specs.

Because web apps are server-side apps, they can use Authorization Code Flow, which exchanges an Authorization Code for a token.

Then we perform PKCE, which uses proof key for code exchange.

An alternate of ACF (Authorization Code Flow) Implicit Flow exist, which is intended for public clients or applications which are unable to securely store Client Secrets.

Hybrid Flow exist for apps that are able to securely store Client Secrets, which combines features of Authorization Code Flow and Implicit Flow with Form Post to allow your application to have immediate access to an ID token while still providing for secure and safe retrieval of access and refresh tokens.

Client Credentials Flow - With machine-to-machine (M2M) applications, such as CLIs, daemons, or services running on your back-end, the system authenticates and authorizes the app rather than a user. 

Device Authorization Flow - This allows users to authorization without having to input text, but using other applications such as your phone or computer.

Not recommended, Resource Owner Password Flow is for highly trusted applications which requests that users provide credentials.

### Authorization and Authentication flows Questions

1. What is the difference between authorization and authentication?
2. What is Authorization Code Flow?
3. What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?
4. What is Implicit Flow with Form Post?
5. What is Client Credentials Flow?
6. What is Device Authorization Flow?
7. What is Resource Owner Password Flow?

### Authorization and Authentication flows Answers

1. Authorization grants or denies access based on the results from the authentication.
2. This is where the client exchanges an auth code for access token.
3. PKCE adds an additional security step by generating a code verifier and challenge for users.
4. The access token is obtained directly from the authorization server and returned in a hidden form field.
5. App can directly exchange credentials for access token without authentication.
6. For apps with limit input capabilities, where the user authorizes through other devices.
7. Exchanging the user's creds for an access token, which is dangerous.

## Things I want to know more about

I want to understand on how to use OAuth, so I can make apps that allow users to have unique data for them.
I want to learn on the process one by one of using Auth, and getting the access token, and then receiving resources.