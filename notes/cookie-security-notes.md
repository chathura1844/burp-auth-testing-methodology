# Cookie Security Notes

## Important Cookie Flags

### Secure

Prevents cookies from being transmitted over HTTP.

---

### HttpOnly

Prevents JavaScript access to cookies.

---

### SameSite

Helps reduce CSRF risks.

---

# Sensitive Cookies

Examples:

- PHPSESSID
- session
- auth_token
- login_string

---

# Observations

Missing `Secure` flags may increase risk if cookies are transmitted over insecure connections.

However, risk depends on whether the cookie is authentication-related.
