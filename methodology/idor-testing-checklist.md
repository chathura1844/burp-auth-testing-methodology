# IDOR Testing Checklist

## Read Access Testing

- [ ] Change numeric IDs
- [ ] Change UUIDs
- [ ] Replay victim requests using attacker session
- [ ] Compare response bodies
- [ ] Check sensitive information exposure

---

## Write Access Testing

- [ ] Test save/update endpoints
- [ ] Test delete functionality
- [ ] Test account modification requests
- [ ] Verify whether changes persist

---

## High-Value Targets

- [ ] /api/
- [ ] /ajax/
- [ ] upload functionality
- [ ] booking/order systems
- [ ] invoices
- [ ] profile editing
- [ ] password reset workflows

---

## Evidence Collection

- [ ] Save Burp screenshots
- [ ] Save Comparer outputs
- [ ] Save HTTP requests
- [ ] Redact sensitive tokens before publishing
