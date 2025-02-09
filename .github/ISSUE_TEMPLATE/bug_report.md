---
Name: Bug Report - Password Reset Not Working
About: Users are unable to reset their password through the Forgot Password feature
Title: "[Bug]: Password Reset Not Working"
labels: bug, high-priority
assignees: ''

---

## **Describe the Bug**
Users who try to reset their password receive an error message stating "Invalid Token" or do not receive a password reset email.

## **Steps to Reproduce**
1. Go to the **Login Page**.
2. Click on **Forgot Password**.
3. Enter a registered email address and submit.
4. Check the email inbox for the reset link.
5. Click the link and attempt to set a new password.
6. The page either shows an "Invalid Token" error or does not update the password.

## **Expected Behavior**
Users should receive a valid password reset link that allows them to securely change their password.

## **Screenshots (if applicable)**
_Attach screenshots here if applicable._

## **Device Information**
- **Device**: Desktop & Mobile
- **Browser**: Chrome, Firefox
- **OS**: Windows 10, macOS

## **Possible Causes**
- The token used for password reset expires too quickly.
- The backend is not correctly verifying the reset token.
- The email system is failing to send the reset link.

## **Suggested Fix**
- Extend the password reset token expiry time.
- Debug the token verification process.
- Check email delivery logs for failures.

## **Additional Context**
This issue is affecting multiple users, preventing them from accessing the platform.

