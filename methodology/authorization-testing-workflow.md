# Authorization Testing Workflow

## Step 1 — Capture Victim Request

Open Burp Suite HTTP history and identify authenticated account requests.

Example:

GET /admin/account.php?id=61685

---

## Step 2 — Send to Repeater

Right click request → Send to Repeater.

---

## Step 3 — Replay Using Attacker Session

Replace victim cookies with attacker cookies while preserving target resource ID.

Example:

Victim:
toktok=61685

Attacker:
toktok=61686

---

## Step 4 — Compare Responses

Analyze:
- response length
- login redirects
- 403 pages
- sensitive data exposure

---

## Step 5 — Validate Authorization

Check whether:
- victim data exposed
- unauthorized modification possible
- ownership enforcement exists
