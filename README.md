# Ayuvya Online Doctor Consultation

**Tested by:** Pritidarshini  
**Role:** QA Intern  

---

## 📌 Overview

This document contains the manual test cases prepared for the Ayuvya Online Doctor Consultation feature available at:

🔗 **URL Under Test:** https://ayuvya.com/online-doctor-consultation

**Objective:** Verify that a user can successfully book an online doctor consultation from the provided page, including navigation, slot selection, form submission, and payment, along with validation, error handling, and UI checks.

---

## 📁 Deliverable

| File | Description |
|------|-------------|
| `ayuvya_-_Pritidarshini.xlsx` | Complete test case sheet with 76 test cases |

---

## 🧪 Test Case Summary

| Module | Total Cases | Pass | Fail |
|--------|-------------|------|------|
| Consultation | 1 | 1 | 0 |
| UI | 6 | 5 | 1 |
| Navigation | 7 | 7 | 0 |
| Form | 11 | 7 | 4 |
| Login | 4 | 4 | 0 |
| Booking | 7 | 6 | 1 |
| Payment | 40 | 38 | 2 |
| **Total** | **76** | **68** | **8** |

---

## 🔴 Failed Test Cases

| TC ID | Module | Scenario | Issue Found |
|-------|--------|----------|-------------|
| TC_003 | UI | Signup Option Visibility | Only signup visible; Login option not shown upfront |
| TC_007 | Form | Email Validation (Min Length) | System accepts short/invalid email formats |
| TC_008 | Form | Email Validation (Wrong Domain) | System accepts invalid domain (e.g., user@gail.com) |
| TC_011 | Form | Mandatory Fields Check | Validation does not appear on empty submit |
| TC_012 | Form | Country Code Availability | Only +91 available; no other country codes |
| TC_022 | Booking | Slot Availability Info | No available/booked slot info displayed |
| TC_023 | Booking | Expert Selection | No option to choose a specific expert/doctor |
| (Form) | Payment | — | Minor payment-related edge cases flagged |

---

## 🗂️ Modules Covered

### 1. Consultation
- Page load and basic accessibility

### 2. UI
- Page title, heading visibility
- Consultation card display
- Social media icon redirects
- Login/Signup option visibility

### 3. Navigation
- Logo/Home page redirect
- Footer links (Contact Us, Categories, Customer Services, Terms & Conditions, About)
- Login access via profile icon

### 4. Form
- Email validation (length, domain, space)
- Phone number validation
- Mandatory field checks
- Country code dropdown
- Name, email, phone, problem description, and file upload inputs

### 5. Login
- Login via phone + OTP
- OTP delivery and verification
- Logout functionality

### 6. Booking
- Book Now navigation
- Calendar restrictions (past dates, Sundays, +2 day minimum gap)
- Time slot display (15-min intervals)
- Slot availability info
- Expert selection

### 7. Payment
- Payment page load and all method availability (UPI, Card, Wallet, Net Banking, PayLater, QR)
- UPI ID and phone number validation
- QR code scan and timeout
- Payment success, failure, cancellation, and network error handling
- Coupon / offer code validation
- Back button popup and leave/continue checkout flow
- PayLater eligibility and OTP verification
- Redirect back to merchant

---

## ✅ Test Case Structure

Each test case follows this format:

| Column | Description |
|--------|-------------|
| **Test Case ID** | Unique identifier (TC_001 – TC_076) |
| **Module** | Feature area being tested |
| **Scenario** | Short description of what is being tested |
| **Steps** | Step-by-step test execution |
| **Test Data** | Input data used (where applicable) |
| **Expected Output** | What the system should do |
| **Actual Output** | What the system actually did |
| **Priority** | Critical / High / Medium / Low |
| **Status** | Pass / Fail |

---

## 🛠️ Tools & Environment

- **Testing Type:** Manual / Exploratory
- **Browser:** Chrome (latest)
- **Device:** Desktop
- **Documentation:** Microsoft Excel (.xlsx)

---

## 📝 Notes

- The test was performed on the live production URL as provided.
- No automated scripts were used; all tests were performed manually.
- Some test cases with "Fail" status highlight areas that may need developer attention, especially around form validation and signup/login visibility.
