# JSON Web Token (JWT) Research

## Summary

JSON Web Token (JWT) is an open standard for securely transmitting information between parties as a JSON object (Auth0, n.d.). It is widely used for authentication and authorization in web applications because it allows stateless verification of user identity without storing session data on the server, which improves scalability and performance (JWT.io, n.d.). A JWT consists of three parts: a header specifying the algorithm, a payload containing claims or user data, and a signature ensuring integrity and authenticity. The server signs the token, and the client includes it in subsequent requests to authenticate and authorize access. If a web application does not use SSL/TLS, JWTs transmitted over HTTP can be intercepted or modified, exposing sensitive information. A real-world example of JWT misconfiguration involved leaking sensitive user data due to improper token handling (Morata, 2023).

---

## References

- Auth0. n.d. JSON Web Tokens. Available at: [https://auth0.com/docs/secure/tokens/json-web-tokens](https://auth0.com/docs/secure/tokens/json-web-tokens) (Accessed: 24 September 2025).
- JWT.io. n.d. JSON Web Tokens. Available at: [https://jwt.io](https://jwt.io) (Accessed: 24 September 2025).
- Morata, D. 2023. *JWT misconfiguration and PII-sensitive information leak*. Medium. [Online] Available at: [https://medium.com/@moratadave/jwt-misconfiguration-and-pii-sensitive-information-leak-03196ab243e2](https://medium.com/@moratadave/jwt-misconfiguration-and-pii-sensitive-information-leak-03196ab243e2) (Accessed: 24 September 2025).
