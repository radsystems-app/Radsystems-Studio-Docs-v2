---
title: Two Factor Authentication
description: 
published: true
date: 2026-02-18T08:31:51.960Z
tags: 
editor: markdown
dateCreated: 2026-02-18T08:08:02.768Z
---

# Two-Factor Authentication

![rs-authentication-2fabutton.webp](/assets/authentication/rs-authentication-2fabutton.webp)

**Two-Factor Authentication (2FA)** has become an industry standard in modern web applications. It adds an extra layer of security by requiring a second form of identification—beyond just a password—to verify the user's identity. This significantly reduces the risk of unauthorized access due to compromised credentials.

RadSystems Studio makes the implementation of this advanced security feature extremely easy. This is a "low-code" feature, meaning while the Studio provides the structure, you will need a basic understanding of coding to finalize the connection to your specific service provider. 

> Because 2FA logic is executed on the server, the code language used in the editor will match your selected backend framework (e.g., PHP for Laravel).
> {.is-info}

### Enabling 2FA

![rs-2fa-enable.png](/assets/authentication/rs-2fa-enable.png)

- **Enable Two Factor Authentication**: Check this box to activate the 2FA layer for your application.
    
- **OTP Duration**: Specify how long the One-Time Password (OTP) remains valid (in minutes) before it expires. The default is set to **5 minutes**.
    

### 2FA via Email

![rs-2fa-email.png](/assets/authentication/rs-2fa-email.png)

- **Send OTP via Email**: Selecting this option opens a server-side code editor pre-populated with a `sendOTPEmail($user)` function.
    
- **Function Logic**: This function automatically generates a random 4-digit number and identifies the recipient's email from the `$user` object.
    
- **Customization**: You must review and modify the `$message` and `$subject` strings to fit your brand. The core mailing logic is handled by the `sendOTPVerificationMail` method, which uses your project's global mail settings.
    

### 2FA via SMS

![rs-2fa-sms.png](/assets/authentication/rs-2fa-sms.png)

- **Send OTP via SMS**: Selecting this option opens the `sendOTPSMS($user)` function in the editor.
    
- **Provider Integration**: Unlike email, SMS requires a third-party gateway (such as Twilio or Nexmo).
    
- **Configuration**: You must modify the `$headers` array to include your specific **apikey** and **apisetcret**.
    
- **Data Payload**: The `$postdata` array is configured to send the OTP to the user's phone number. You will need to adjust the API endpoint and request format to match the documentation of your chosen SMS provider.