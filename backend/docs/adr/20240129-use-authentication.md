# Authentication management

- **Status**: proposed
- **Deciders**: -
- **Date**: 01/29/2024

## Context and Problem Statement

When developing a web platform, it is expected to be secure; users expect that their access data does not have to be vulnerable.

Many web platforms provide a way to log in with your Google account, giving the user easy access to their accounts.

## Decision Drivers

- We need secure authentication
- We need to detect and respond to potential security threats

## Considered Options

- [Auth0 NextJS](https://auth0.com/docs/quickstart/webapp/nextjs)
- [JWT](https://jwt.io/introduction)

### Positive Consequences

- Good documentation
- Large community

### Negative Consequences

- If the app grows, a cost will be required
- Maybe a little complex for those with little experience.

## Pros and Cons of the Options

### JWT (JSON Web Tokens)

- Pro, because JWT provides a secure method to authenticate users using tokens.
- Pro, because have a large community
- Pro, because From the backend you do not need to have a record of the tokens
- Cons, because have the token exposed in the client's browser

### Auth0

- Pro, because auth0 offers easy integration with various platforms and technologies
- Pro, because implements security practices and provides tools to monitor and respond to potential security threats
- Pro, because robust and efficient authentication system to guarantee the security and proper management of user identity.
- Pro, because centralized user management, improve security, and offer a smoother login experience for our users.
- Cons, because depending on plan and usage, using Auth0 may incur additional costs
- Cons, because depends on a third-party service for authentication management