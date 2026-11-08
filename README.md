# Simple Phishing Test Project with GoPhish

This project shows how to install, set up, and test a phishing simulation using GoPhish on Kali Linux. We used a safe testing email and a virtual inbox tool called Mailtrap to test everything safely without using any real personal information.

## 🚀 My Test Environment
* **Attacker Machine:** Kali Linux VM (Running GoPhish)
* **Target Email:** A fresh Proton Mail account (`projecttestuser1@proton.me`)
* **Safe Mail Carrier:** Mailtrap Sandbox (To send and catch the emails safely)

---

## 🛠️ Commands I Used

Open the terminal in Kali Linux and run these commands step-by-step:
```bash
# 1. Update your Kali Linux system
sudo apt update

# 2. Install GoPhish automatically
sudo apt install gophish -y

# 3. Start the GoPhish server
sudo gophish
```

---

## 📸 Project Pictures (Evidence)

Please put your saved project pictures inside the spaces below:

---
### Picture 1: GoPhish Dashboard Home Screen
* **What picture goes here:** The very first screen you saw right after logging into GoPhish with the username `admin` and password `kali-gophish`. It shows an empty homepage.
<!-- PUT PICTURE 1 HERE -->


---
### Picture 2: Email Template Setup
* **What picture goes here:** The screen where you typed the email body text about the "Unusual sign-in activity detected from Lagos, Nigeria" and added the `{{.URL}}` link.
<!-- PUT PICTURE 2 HERE -->


---
### Picture 3: Fake Landing Login Page
* **What picture goes here:** The screen where you pasted the HTML code for the login boxes and checked the "Capture Credentials" and "Capture Passwords" boxes.
<!-- PUT PICTURE 3 HERE -->


---
### Picture 4: Sending Profile Settings
* **What picture goes here:** The screen where you pasted your Mailtrap host name, username, and password strings so GoPhish could connect to Mailtrap.
<!-- PUT PICTURE 4 HERE -->


---
### Picture 5: Final Campaign Results (The Best Proof!)
* **What picture goes here:** Your final dashboard screenshot showing the 4 colored circles filled with the number 1. It shows that the email was successfully Sent, Opened, Clicked, and that data was Submitted!
<!-- PUT PICTURE 5 HERE -->


---

## ⚠️ Problems I Faced and How I Fixed Them

### 1. Tuta Account Hold Problem
* **The Problem:** I tried to make a free account on Tuta email, but their system locked me out for 48 hours for safety.
* **The Fix:** I changed my plan and made a free account on **Proton Mail** instead, which let me log in immediately using a quick picture puzzle.

### 2. Normal Email Accounts Blocking GoPhish
* **The Problem:** Standard email services like Gmail or Yahoo block automated phishing test emails immediately and suspend your account.
* **The Fix:** I signed up for a free tool called **Mailtrap**. It gave me safe fake login codes to put into GoPhish so my emails would send smoothly.

### 3. Link Not Loading ("Site Can't Be Reached")
* **The Problem:** When I clicked the phishing test link on my normal computer browser, the page did not load. This happened because the link was looking inside my normal PC instead of inside the Kali VM.
* **The Fix:** I logged into Mailtrap **inside my Kali Linux browser** instead. When I clicked the link inside Kali, the fake login screen loaded perfectly.

### 4. Why "Email Reported" Was Zero (0)
* **The Problem:** I noticed the "Email Reported" metric on the final dashboard stayed at 0, and I wanted to make sure nothing was broken.
* **The Fix:** This is completely correct! The circle stays at 0 because our basic email template did not have a special report button hooked up to it. It shows that our test target fell for the trick and did not report the email.

---
*Disclaimer: This project was made strictly for school work and legal learning purposes. No real people were phished.*
