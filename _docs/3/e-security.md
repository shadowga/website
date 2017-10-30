---
layout: docs
title: 3e. Security
permalink: /docs/3/e-security/
---
As an administrator and member of this server, guarding your information is vital to prevent weak points in our community.
Because the security of your accounts is your responsibility, we recommend both normal members and admins to take this seriously.

## In-game security
The server only accepts premium users so there's always a chance of administrator accounts being hijacked or stolen.
There's often leaks in several account databases, so admins should keep an eye out to make sure their information hasn't been compromised.
Administrators can be removed if they haven't taken the proper action during these situations.

### Account information
Admins must periodically check their e-mail addresses to make sure they weren't included in any recent leaks.
There are many tools capable of effectively doing this, but we recommend [this](https://haveibeenpwned.com/) service for quick lookups.

Passwords should be made as long as possible to prevent a brute-force attack, but it's also important to not use obvious terms (such as your last name, date of birth, or something common like a city name).
GRC provides [Perfect Passwords](https://www.grc.com/passwords.htm), a free service that generates safe passwords.

### Security questions
When it comes to verifying accounts when your password isn't available, Mojang uses a set of three security questions with answers unique to what you've chosen.

Usually the questions asked are common but personal, such as the name of your pet or first school, and it's important not to forget the answers or you'll be locked out of your own account.
Refrain from using a short string of numbers (commonly '1234') or one-word terms (as mentioned above, like the name of a city).

## Website and forum
Depending on your authorization level, your forum account may contain access to admin-only information or important settings.
You don't want other people having access to that, which is why it's even more vital to keep private forum and homepage information away from prying eyes.
If your forum account becomes compromised, you should notify the owner immediately for deactivation.

### Web encryption
Privacy is very important to us, so web encryption is one of our top priorities.
Everything from the website (`https://shadow.ga`) and forum (`https://f.shadow.ga`) goes through Cloudflare.
These two services always use HTTPS (secure HTTP) content with TLS 1.3 through their CDN (content delivery network).
Resources such as HTTPD don't go through this process because they aren't providing or requesting sensitive information.

### Account information
Like in-game security, keeping your e-mail address and password safe is of great importance.
We recommend [ProtonMail](https://protonmail.com/) for secure e-mail.
You can use the same tools mentioned earlier in this page for forum security when it's needed.

When selecting a username, don't use your real name or revealing information such as a birth date.
Because everyone can view your forum handle and username, make it something you'd feel comfortable with.

### Two-factor authentication
The forum has a security feature known as 2FA (or two-factor authentication) that prevents login from only the username and password.
While this layer is optional for members, all admins must have 2FA enabled on their forum account.

Instead of relying on your password and nothing else, an account with two-factor enabled will also ask for an authentication code.
This auth code is stored on your phone or other mobile device.

#### Activating two-factor login
To enable two-factor auth, simply go to your profile's [settings](https://f.shadow.ga/settings).
From there, you can enter the provided code or barcode into the mobile application of your choice. We recommend [Google Authenticator](https://support.google.com/accounts/answer/1066447?co=GENIE.Platform%3DAndroid&hl=en) for retrieving auth codes.
> **Upcoming:** In the future, we also plan to add support for text message (SMS) verification if you don't want to use a TOTP application. Right now it's required for two-factor auth.

Your TOTP application should give you a six-digit token that you can enter into the text box, submit, and receive a short list of one-time backup codes.
Remember to store those backup codes in a safe place, you'll need them if you ever have trouble accessing your account.
> **Note:** If you've linked your forum account to GitHub, you should enable two-factor authentication over there as well. There's a guide on doing that [here](https://help.github.com/articles/securing-your-account-with-two-factor-authentication-2fa/).

### Watching your back
Making a forum account is rather easy, but you still shouldn't give out information like your private e-mail or banking information.
We won't ever ask for personal information in any way, whether that be through mail or text.

If you ever receive a suspicious message bearing our name, [contact us](https://shadow.ga/docs/1/e-support/#direct-support) and we'll take appropriate action from there.
Keep in mind that we only use the `mg.shadow.ga` subdomain for e-mails, so any other address is fake.

## Discord account
Everything said above also applies to the guild and your Discord account.
They even provide two-factor security of their own, and admins must have it enabled—there's a guide for that [here](https://support.discordapp.com/hc/en-us/articles/219576828-Setting-up-Two-Factor-Authentication).

> **Note:** As of now, Discord's process of enabling 2FA is only present on their programme's web and desktop versions. You'll need a desktop machine for this, but it only needs to be done once.

Members of our guild with admin positions won't be able to utilise the service's features without enabling two-factor auth.
If your Discord account is compromised, notify an Executive or the owner so we can temporarily remove your permissions.
