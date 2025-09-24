# SSL/TLS and Web Application Security

## Summary

SSL/TLS are cryptographic protocols that secure and verify communication between clients and servers, ensuring confidentiality, integrity, and authenticity. HTTPS is HTTP transported over SSL/TLS, meaning that all data (headers, body, cookies) is encrypted and the server’s identity is validated. SSL/TLS is critical in web applications because it prevents eavesdropping, tampering, and man-in-the-middle attacks; without it, sensitive information such as logins or personal data can be exposed. In addition, mechanisms like HTTP Strict Transport Security (HSTS) strengthen protection by forcing browsers to always use HTTPS and disallowing insecure downgrades (Mozilla, 2025). Free services such as Let’s Encrypt make HTTPS widely accessible by offering automated certificates, helping to raise the security baseline of the web (Let’s Encrypt, 2025).

---

## Reflection

- **Did adding SSL/HTTPS affect any part of your application?**
Yes, the application now runs over HTTPS instead of HTTP, which required updating configurations for both backend and frontend. Some API calls needed their URLs updated to `https://localhost`.

- **Were there any challenges in trusting the certificate or configuring your stack?**
The biggest challenge was dealing with browser security warnings caused by the self-signed certificate. Importing the certificate into the Trusted Root Certification Authorities solved this, but it added extra setup steps.

- **What steps would be different when preparing for production deployment?**
In production, self-signed certificates should not be used. Instead, a trusted CA like Let’s Encrypt would issue certificates, and SSL would be managed at the server or cloud provider level (e.g., via NGINX reverse proxy or AWS/Heroku certificate management). Auto-renewal and monitoring would also be configured to avoid expired certificates causing outages.

---

## References

- Mozilla. 2025. *HTTP Strict Transport Security (HSTS)*. [Online]. Available at: [https://developer.mozilla.org/en-US/docs/Web/Security/HTTP_strict_transport_security](https://developer.mozilla.org/en-US/docs/Web/Security/HTTP_strict_transport_security)
- Let’s Encrypt. 2025. *Why HTTPS?* [Online]. Available at: [https://letsencrypt.org/docs/why-https/](https://letsencrypt.org/docs/why-https/)
