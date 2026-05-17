# Test Report – Boarding House Management System

## 1. Testing Overview

Project: Boarding House Management System  
Testing Types:
- API Testing
- UI Testing
- Functional Testing

Tools Used:
- Postman
- Browser UI
- Excel Test Cases

---

## 2. Tested Modules

| Module | Test Type |
|---|---|
| User Management | API + UI |
| Room Management | API + UI |
| Tenant Management | API + UI |
| Contract Management | API + UI |
| Invoice Management | API + UI |
| Payment Management | API + UI |

---

## 3. Test Execution Results

| Test Case ID | Feature | Status |
|---|---|---|
| TC001 | Create User API | Pass |
| TC002 | Invalid User API | Fail |
| TC003 | Get Users API | Pass |
| TC004 | Create Room API | Pass |
| TC005 | Update Room API | Pass |
| TC006 | Delete Room API | Pass |
| TC007 | Create Tenant API | Pass |
| TC008 | Update Tenant API | Pass |
| TC009 | Create Contract API | Pass |
| TC010 | Get Contract API | Pass |
| TC011 | Create Invoice API | Fail |
| TC012 | Create Payment API | Fail |
| TC013 | Login UI | Pass |
| TC014 | Invalid Login UI | Fail |
| TC015 | Add Room UI | Pass |
| TC016 | Update Room UI | Pass |
| TC017 | Add Tenant UI | Pass |
| TC018 | Create Contract UI | Pass |
| TC019 | Create Invoice UI | Pass |
| TC020 | Payment UI | Pass |

---

## 4. Bugs Found

| Bug ID | Description | Status |
|---|---|---|
| BUG01 | User API accepts invalid data | Fixed |
| BUG02 | Tenant API behavior issue | Not Fixed |
| BUG03 | Invoice API accepts negative amount | Not Fixed |
| BUG04 | Payment API returns 500 error | Not Fixed |

---

## 5. Bug Details

### BUG01 – Invalid User Data Accepted

Steps:
1. Send POST /api/users
2. Input empty or invalid fields
3. Send request

Expected Result:
- Validation error returned

Actual Result:
- User created successfully

Status:
- Fixed

---

### BUG03 – Invoice API Accepts Negative Amount

Steps:
1. Send POST /api/invoices
2. Input negative amount
3. Send request

Expected Result:
- Error message returned

Actual Result:
- Invoice created successfully

Status:
- Not Fixed

---

### BUG04 – Payment API Returns 500

Steps:
1. Send POST /api/payments
2. Use invalid invoice id
3. Send request

Expected Result:
- Validation error returned

Actual Result:
- 500 Internal Server Error

Status:
- Not Fixed

---

## 6. Conclusion

Most API and UI functions are working correctly.
Some validation and exception-handling issues were identified during testing.
Further bug fixing and validation improvements are recommended.