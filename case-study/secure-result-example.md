# Secure Authorization Example

## Victim Request

```http
GET /admin/account.php?id=61685
```

Returned:
- Full account profile
- Victim account information

---

## Attacker Replay

Same request replayed using attacker session.

Returned:
- Login page
- Reduced response size
- No victim information exposed

---

# Conclusion

The application enforced authorization controls and prevented unauthorized access.
