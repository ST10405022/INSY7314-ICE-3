# PulseVote Backend

---

## 01 – Setting up Foundations
✅ Evidence: Server running successfully in terminal.  
![server-confirmation.png](server-confirmation.png)

---

## 02 - Adding SSL
✅ Evidence: HTTPS server running successfully.  
![02_security_warning.png](02_security_warning.png)
![02_terminal_run.png](02_terminal_run.png)

---

## 03 - Adding Authentication with JWT
✅ Evidence: Successful register, login and protected responses in Postman.
- **Register a new user**  
![03_register.png](03_register.png)
- **Login with valid credentials**  
![03_login.png](03_login.png)
- **Access protected route (Authorized)**  
![03_protected_authorised.png](03_protected_authorised.png)
- **Access protected route (Unauthorized)**  
![03_protected_unauthorised.png](03_protected_unauthorised.png)

---

## 05 - Securing your login
✅ Evidence:  
- **Invalid email rejected**  
![05_register_invalid_email.png](05_register_invalid_email.png)  
- **Weak password rejected**  
![05_register_invalid_password.png](05_register_invalid_password.png)  
- **Invalid login email**  
![05_login_invalid_email.png](05_login_invalid_email.png)  
- **Invalid login password**  
![05_login_invalid_password.png](05_login_invalid_password.png)
