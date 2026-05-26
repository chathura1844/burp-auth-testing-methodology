# Burp Suite Authorization Testing Methodology

A practical methodology for testing broken access control, IDOR, session binding, and authorization enforcement using Burp Suite Repeater, Autorize, and Comparer.

## What This Project Demonstrates

- Authorization testing methodology
- IDOR validation workflow
- Session binding analysis
- Secure vs vulnerable response comparison
- Burp Suite Autorize usage
- Evidence collection for AppSec testing

## Tools Used

- Burp Suite Professional
- Autorize extension
- Repeater
- Comparer
- HTTP History

## Key Learning

A vulnerability is not confirmed only because the response is `200 OK`.  
The real proof is whether an attacker can view or modify another user's data.

## Repository Structure

- `methodology/` - testing workflows and checklists
- `case-study/` - redacted authorization testing example
- `sample-requests/` - safe redacted HTTP samples
- `screenshots/` - Burp evidence screenshots
- `checklists/` - access control testing checklist
- `notes/` - cookie and session security notes
