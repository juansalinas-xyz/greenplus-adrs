# Authentication management

- **Status**: proposed
- **Deciders**: Johann Meza
- **Date**: 01/29/2024

## Context and Problem Statement

In the development of a web platform, we need a robust and efficient authentication system to guarantee the security and proper management of user identity.

Currently, we face challenges with the traditional authentication approach, which is complex to manage, presents security risks, and does not provide an optimal experience for users.

With Auth0, we can centralize user management, improve security, and offer a smoother login experience for our users.

## Decision Drivers

- We need secure authentication
- We need to detect and respond to potential security threats

## Considered Options

- [Auth0 NextJS](https://auth0.com/docs/quickstart/webapp/nextjs)
- [JWT](https://jwt.io/introduction)

## Decision Outcome

Chosen option: Auth0, easy implementation, test mode with 7500 users, large community and security. Integrations with multiple platforms

### Positive Consequences

- Good documentation
- Large community

### Negative Consequences

- If the app grows, a cost will be required
- Maybe a little complex for those with little experience.

## Pros and Cons of the Options

### JWT (JSON Web Tokens)

- Good, because JWT provides a secure method to authenticate users using tokens.
- Good, because have a large community
- Good, because From the backend you do not need to have a record of the tokens
- Bad, because have the token exposed in the client's browser

### Auth0

- Good, because auth0 offers easy integration with various platforms and technologies
- Good, because implements security practices and provides tools to monitor and respond to potential security threats
- Bad, because depending on plan and usage, using Auth0 may incur additional costs
- Bad, because depends on a third-party service for authentication management