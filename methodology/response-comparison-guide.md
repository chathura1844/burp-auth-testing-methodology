# Response Comparison Guide

## Goal

Determine whether authorization enforcement exists.

---

# Compare These Elements

- Response length
- Returned account ID
- User email
- Profile name
- Sensitive information
- Login redirects
- Error messages

---

# Secure Comparison Example

| Victim | Attacker Replay |
|---|---|
| 26910 bytes | 4528 bytes |

Large differences often indicate authorization enforcement.

---

# Vulnerable Comparison Example

| Victim | Attacker Replay |
|---|---|
| 26910 bytes | 26890 bytes |

Very similar responses may indicate IDOR or broken access control.

---

# Important Observation

If attacker replay still contains victim information:

- victim email
- victim profile
- victim account details

then authorization may be broken.

---

# Burp Comparer Indicators

## Secure

- Login page
- Forbidden page
- Redirect
- Empty response

## Vulnerable

- Same profile data
- Same account information
- Similar response structure
