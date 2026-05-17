# Test Summary – Boarding House Management System

## 1. Testing Scope

The following modules were tested:
- User Management
- Room Management
- Tenant Management
- Contract Management
- Invoice Management
- Payment Management

Testing included:
- API Testing
- UI Testing
- Functional Testing

---

## 2. Test Case Statistics

| Item | Count |
|---|---|
| Total Test Cases | 20 |
| Passed | 16 |
| Failed | 4 |

---

## 3. Bug Statistics

| Item | Count |
|---|---|
| Total Bugs Found | 4 |
| Fixed Bugs | 0 |
| Unfixed Bugs | 4 |

---

## 4. Main Issues Found

- Invalid user data still accepted by API
- Tenant API returned unexpected behavior
- Invoice API accepts negative amount
- Payment API returns 500 Internal Server Error

---

## 5. Final Result

Most core functions of the system are working correctly.
However, several validation and exception-handling issues still need improvement before production deployment.