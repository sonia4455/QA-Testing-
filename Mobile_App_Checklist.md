# Mobile App QA Checklist

**Prepared by:** Sonia Hlel/QA Tester  
**Date:** april  2026 
**App Type:** Android  
**Testing Type:** Manual / Functional

---

> Use this checklist before any mobile app release. Check each item and note any issues found.

---

## 📲 1. Installation & Launch

- [ ] App installs successfully from store / build file
- [ ] App launches without crashes
- [ ] Splash screen displays correctly
- [ ] App loads within acceptable time (under 3 seconds)
- [ ] App works after being closed and reopened

---

## 🔐 2. Authentication

- [ ] Login with valid credentials works
- [ ] Login with invalid credentials shows error message
- [ ] Empty fields show validation messages
- [ ] "Forgot password" flow works end-to-end
- [ ] Logout works and session is cleared
- [ ] Auto-logout after inactivity (if applicable)

---

## 🧭 3. Navigation

- [ ] All menu items navigate to the correct screen
- [ ] Back button works on every screen
- [ ] No dead-end screens (always a way to go back)
- [ ] Bottom navigation / tab bar works correctly
- [ ] Deep links open the correct screen (if applicable)

---

## ✏️ 4. Forms & Inputs

- [ ] All text fields accept correct input
- [ ] Keyboard type matches input (numeric for phone, email keyboard for email)
- [ ] Required fields show error if left empty
- [ ] Character limits are enforced
- [ ] Copy/paste works in input fields
- [ ] Form submission works and shows confirmation

---

## 🌐 5. Network & Connectivity

- [ ] App works correctly on WiFi
- [ ] App works correctly on 4G/5G
- [ ] App handles loss of internet gracefully (shows error, not crash)
- [ ] App recovers when connection is restored
- [ ] Slow network doesn't cause crash or freeze

---

## 🎨 6. UI & Layout

- [ ] UI displays correctly on small screen (5")
- [ ] UI displays correctly on large screen (6.7")
- [ ] No text is cut off or overlapping
- [ ] Images load correctly (no broken images)
- [ ] Buttons are tappable and large enough
- [ ] Dark mode works correctly (if supported)
- [ ] Landscape mode works correctly (if supported)

---

## ⚡ 7. Performance

- [ ] App does not freeze or lag during normal use
- [ ] Scrolling is smooth (no jank)
- [ ] App does not overheat the device
- [ ] Battery usage is reasonable
- [ ] Memory usage does not grow excessively over time

---

## 🔔 8. Notifications

- [ ] Push notifications are received correctly
- [ ] Tapping notification navigates to correct screen
- [ ] Notification content is accurate
- [ ] Notifications can be disabled in settings

---

## 📷 9. Device Features

- [ ] Camera access works (if applicable)
- [ ] Photo library access works
- [ ] Location services work (if applicable)
- [ ] Microphone access works (if applicable)
- [ ] Permissions prompt appears correctly on first use

---

## 🔄 10. Edge Cases

- [ ] App handles incoming call during use (no crash)
- [ ] App works after device sleep/wake
- [ ] App works after switching to another app and returning
- [ ] App handles very long text input without breaking layout
- [ ] App works with accessibility settings (large text, high contrast)

---

## 📋 Issues Found

| # | Screen | Issue Description | Severity | Screenshot |
|---|---|---|---|---|
| 1 | | | | |
| 2 | | | | |
| 3 | | | | |

---

## ✅ Final Sign-off

| Item | Status |
|---|---|
| All critical items passed | ⬜ Yes / ⬜ No |
| All bugs documented | ⬜ Yes / ⬜ No |
| Ready for release | ⬜ Yes / ⬜ No |

**QA Tester:** Sonia Hlel


---

*Prepared by: Sonia Hlel/QA Tester — April 2026*
