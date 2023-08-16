# Roles, Claims, and JWT Tokens

This topic is important to me because I want to be able to control different aspects of my auth, and be able to have more control over the user experience.

## [Retrospective 19](https://connerkt.github.io/Reading-Notes/401/Class19/Retro19)

## References

[Claims Based Auth](https://docs.microsoft.com/en-us/aspnet/core/security/authorization/claims?view=aspnetcore-2.1)

[Intro to Claims](https://andrewlock.net/introduction-to-authentication-with-asp-net-core/)

[JWT Auth](https://codeburst.io/jwt-to-authenticate-servers-apis-c6e179aa8c4e)

## Claims Based Auth

When an identity is created it maybe be assigned one or more claims issues by a trusted party.

A **Claim** is a name value pair that represents information about the subject(user).

Claims focus on describing who the subject is, rather than what they can do.

With Claim based auth, it involves checking the values of claims associated with an identity to determine whether access to a resource should be granted.

If you go to a 18+ site, and it asks you for your DOB, it would evaluate based on that claim and give you access or not.

Your claim can check for the presence of something you ask on the current identity.

We can then choose what to let the user access based on that.

## Intro to Claims

So what is Authorization, what is claims, and  what is auth.

The simple answer is that Authentication is the process of determining who you are, while Authorization revolves around what you are allowed to do, i.e. permissions.

Claims are essentially just checking who you are, and what to do with you if you don't pass.

## JWT Auth

A **JWT** stands for JSON Web Token, and is a means of representing claims to be transfered between two parties.

Its signed with a JWS (JSON Web Signature) and then Encrypted using JWE (JSON Web Encryption).

Its just a way to encode JSON objects and use that encoded object as access tokens for authentication.

**Structure of a JWT**

- A JWT consists of three parts: Header, Payload, and Signature.
- Header contains metadata, Payload contains claims, and Signature is used to verify the token's authenticity.

**Use of JWT in Server-to-Server Communication**

- JWT can be used to securely transmit information between servers without relying on sessions.
- Servers can use JWT to authenticate themselves to other servers or APIs.

Step 1: Generating a JWT

    Explains how to generate a JWT using a library or tool.
    The process involves creating the header, payload, and signing the token.

Step 2: Sending the JWT

    Describes how the generated JWT is sent in the HTTP header as an authorization token.

Step 3: Validating the JWT

    Discusses the process of validating the received JWT on the server's end.
    This involves checking the signature, expiration time, and other claims.

Step 4: Granting Access

    Once the JWT is validated, the server grants access to the requester based on the claims in the token.

## Things I want to know more about

I want to learn more about JWT and claim based Auth.

I want to learn the goods between one and the other.