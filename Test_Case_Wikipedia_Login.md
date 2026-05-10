# Test Case — User Login Flow

**Project:** Wikipedia Web Application
**Module:** Authentication — Login
**Prepared by:** Sonia Hlel/QA Tester
**Date:** April 2026
**Status:** ✅ Executed

---

## Overview

This test case covers the full login flow on Wikipedia including valid login, invalid credentials, edge cases, and security checks.

---

## Test Environment

| Item | Details |
|---|---|
| Browsers tested | Chrome 124, Firefox 125, Safari 17 |
| Devices | Windows 11 PC, iPhone 13 (iOS 17), Samsung Galaxy S21 (Android 14) |
| Test URL | https://en.wikipedia.org/w/index.php?title=Special:UserLogin |
| Valid test account | qa.tester.test01@gmail.com / QaTester2024! |
| Invalid credentials | qa.tester.test01@gmail.com / wrongpassword123 |

---

## Test Cases

### ✅ TC-001 — Valid Login

| Field | Details |
|---|---|
| **Test ID** | TC-001 |
| **Title** | User logs in with valid credentials |
| **Priority** | 🔴 High |
| **Precondition** | User has a registered Wikipedia account |

**Steps:**
1. Open https://en.wikipedia.org/w/index.php?title=Special:UserLogin
2. Enter username: `QaTesterPro`
3. Enter password: `QaTester2024!`
4. Click **"Log in"**

**Expected Result:** User is redirected to the Wikipedia homepage. Top-right corner shows the username "QaTesterPro" and a user menu.

**Actual Result:** ✅ PASS — Redirected to homepage, username displayed correctly in top-right corner.

---

### ❌ TC-002 — Invalid Password

| Field | Details |
|---|---|
| **Test ID** | TC-002 |
| **Title** | Login fails with wrong password |
| **Priority** | 🔴 High |
| **Precondition** | User has a registered Wikipedia account |

**Steps:**
1. Open https://en.wikipedia.org/w/index.php?title=Special:UserLogin
2. Enter username: `QaTesterPro`
3. Enter wrong password: `wrongpassword123`
4. Click **"Log in"**

**Expected Result:** Error message appears in red — *"Incorrect password entered. Please try again."* User stays on login page.

**Actual Result:** ✅ PASS — Error message displayed correctly. User not logged in.

---

### ❌ TC-003 — Empty Fields Submission

| Field | Details |
|---|---|
| **Test ID** | TC-003 |
| **Title** | Login attempted with empty username and password |
| **Priority** | 🟡 Medium |
| **Precondition** | None |

**Steps:**
1. Open https://en.wikipedia.org/w/index.php?title=Special:UserLogin
2. Leave both username and password fields empty
3. Click **"Log in"**

**Expected Result:** Error message appears — *"Please enter your username."* Focus moves to the username field.

**Actual Result:** ✅ PASS — Error displayed, fields highlighted correctly.

---

### 🔒 TC-004 — CAPTCHA After Multiple Failed Attempts

| Field | Details |
|---|---|
| **Test ID** | TC-004 |
| **Title** | CAPTCHA appears after repeated failed logins |
| **Priority** | 🔴 High |
| **Precondition** | None |

**Steps:**
1. Open https://en.wikipedia.org/w/index.php?title=Special:UserLogin
2. Enter any username with wrong password
3. Repeat 5 times consecutively

**Expected Result:** After multiple failed attempts, a CAPTCHA challenge appears before allowing further login attempts.

**Actual Result:** ✅ PASS — CAPTCHA displayed after 5 failed attempts. Further attempts blocked until CAPTCHA is solved.

---

### 🔑 TC-005 — Forgot Password Link

| Field | Details |
|---|---|
| **Test ID** | TC-005 |
| **Title** | "Forgot password" link redirects to reset page |
| **Priority** | 🟡 Medium |
| **Precondition** | None |

**Steps:**
1. Open https://en.wikipedia.org/w/index.php?title=Special:UserLogin
2. Click **"Forgot your password?"** link below the login form

**Expected Result:** User is redirected to https://en.wikipedia.org/w/index.php?title=Special:PasswordReset — email input field visible.

**Actual Result:** ✅ PASS — Redirected correctly to password reset page.

---

### 📱 TC-006 — Login on Mobile Safari (iPhone 13)

| Field | Details |
|---|---|
| **Test ID** | TC-006 |
| **Title** | Login works correctly on iPhone 13 — Safari |
| **Priority** | 🔴 High |
| **Precondition** | Test on iPhone 13, iOS 17, Safari 17 |

**Steps:**
1. Open Safari on iPhone 13
2. Navigate to https://en.wikipedia.org/w/index.php?title=Special:UserLogin
3. Enter valid username and password
4. Tap **"Log in"**

**Expected Result:** Login succeeds. User redirected to Wikipedia homepage. Layout fully responsive — no broken elements, no overflow, username visible in top menu.

**Actual Result:** ✅ PASS — Login successful. Responsive layout correct on mobile.

---

### 🌐 TC-007 — Cross-Browser Login (Firefox & Safari Desktop)

| Field | Details |
|---|---|
| **Test ID** | TC-007 |
| **Title** | Login works consistently across all browsers |
| **Priority** | 🟡 Medium |
| **Precondition** | Test on Firefox 125 and Safari 17 (desktop) |

**Steps:**
1. Repeat TC-001 on Firefox 125
2. Repeat TC-001 on Safari 17 desktop

**Expected Result:** Login works identically on all browsers. No visual or functional differences.

**Actual Result:** ✅ PASS — Consistent behavior across Chrome, Firefox, and Safari.

---

## Summary Table

| Test ID | Title | Priority | Result |
|---|---|---|---|
| TC-001 | Valid login | 🔴 High | ✅ PASS |
| TC-002 | Invalid password | 🔴 High | ✅ PASS |
| TC-003 | Empty fields | 🟡 Medium | ✅ PASS |
| TC-004 | CAPTCHA after failures | 🔴 High | ✅ PASS |
| TC-005 | Forgot password | 🟡 Medium | ✅ PASS |
| TC-006 | Mobile Safari | 🔴 High | ✅ PASS |
| TC-007 | Cross-browser | 🟡 Medium | ✅ PASS |

**Total: 7 tests — 7 PASS — 0 FAIL**

---

*Tested by: Sonia Hlel/QA Tester — April 2026 — Wikipedia.org*
