# Using Autorize Extension

## Purpose

Autorize helps automate authorization testing by replaying requests using attacker sessions.

---

# Workflow

## Step 1

Capture victim requests.

---

## Step 2

Configure attacker cookies inside Autorize.

Example:

```http
PHPSESSID=REDACTED
toktok=61686
```

---

## Step 3

Enable Autorize interception.

---

## Step 4

Replay victim requests automatically.

---

# Response Interpretation

## Secure Result

- 403 Forbidden
- Login page
- Empty response
- Ownership correction

---

## Potential Vulnerability

- Similar response lengths
- Victim data exposure
- Unauthorized modification
- Matching account information

---

# Important Note

A `Bypassed!` result alone does not confirm a vulnerability.

Always inspect response bodies manually.
