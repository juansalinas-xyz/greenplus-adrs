# Authentication management

- Status: ACCEPTED
- Deciders: Didier Brange, Santiago Ianello, Lautaro Carreño, Sofia Torres, Felipe Ponce, Johann Meza, Ariel Vaca, Jorge Agurto, Juan Salinas
- Date: 31-01-2024 

## Context and Problem Statement

When developing a web platform, it is expected to be secure; users expect that their access data does not have to be vulnerable.

Many web platforms provide a way to log in with your Google account, giving the user easy access to their accounts.

## Decision Drivers

- We need secure authentication
- We need to detect and respond to potential security threats

## Considered Options

- [Auth0 NextJS](https://auth0.com/docs/quickstart/webapp/nextjs)
- [JWT](https://jwt.io/introduction)

## Decision Outcome

Chosen option: Auth0, because it offers an easy an fast way to create an authorization/ authentication process

### Positive Consequences

- The development process for authorization and authentication will be faster

### Negative Consequences

- Free plan allow only 7.500 active users 

## Pros and Cons of the Options

### JWT (JSON Web Tokens)

- Good, because JWT provides a secure method to authenticate users using tokens.
- Good, because have a large community
- Good, because From the backend you do not need to have a record of the tokens
- Bad, because have the token exposed in the client's browser

### Auth0

- Good, because auth0 offers easy integration with various platforms and technologies
- Good, because implements security practices and provides tools to monitor and respond to potential security threats
- Good, because robust and efficient authentication system to guarantee the security and proper management of user identity.
- Good, because centralized user management, improve security, and offer a smoother login experience for our users.
- Bad, because depending on plan and usage, using Auth0 may incur additional costs
- Bad, because depends on a third-party service for authentication management