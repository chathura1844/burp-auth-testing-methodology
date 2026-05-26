# Account Endpoint Authorization Analysis

## Target

Authenticated account management functionality.

---

# Tested Endpoint

```http
GET /admin/account.php?id=61685
```

---

# Methodology

- Captured victim request
- Replayed request using attacker session
- Compared responses using Burp Comparer

---

# Observed Behavior

Victim response returned full account page.

Attacker replay returned login page / reduced response content.

---

# Result

Authorization enforcement appears functional.

No confirmed IDOR observed during testing.

---

# Lessons Learned

- Ownership binding is important
- Response comparison is critical
- Similar response sizes require manual validation
