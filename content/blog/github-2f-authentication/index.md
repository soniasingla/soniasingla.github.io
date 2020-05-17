---
title: How to access GitHub using two-factor authentication?
date: "2019-07-30"
description: "Two-factor authentication, or 2FA is the most significant solution used to protect users data and adds security while logging into browser, app or any website."
---

##What is two-factor authentication, or 2FA and the need to implement it ?

Two-factor authentication, or 2FA is the most significant solution used to protect users data and adds security while logging into browser, app or any website. It adds extra layer in the logging process by asking the user about authentication code that only the user could have access.

Some users might choose weak or poor passwords, might apply the same password for multiple different sites. Many of the users have bad habit of writing and saving their username and password from where they could fetch with ease. Just by entering username and password `even if the password chosen is strong enough`, the second person can access all the data, even without using any kind of sophisticated hacking.

To secure the users data, two-factor authentication solution has been generated. One-time code is being generated and the user is supposed to enter the code within minimum time possible.

##How to make git clone work with and without 2FA?

**Without 2FA :**

```
$ git clone https://github.com/mozilla/addons-frontend.git

>> Username : your_username

>> Password : your_password
```

**With 2FA :**

For using 2 factor authentication, initially we need to know how to set up the access token for command line and after that, the same generated token is used as your password.

Here, are the steps written sequentially to know about generating tokens for command line in detail :

1. Click on your `profile` icon and then go to `settings`.

2. On the left side menu bar, you will see `Developer Settings`, click on it.

3. Then `personal access tokens`. After that, click on `Generate new token` :

4. Make sure to copy the tokens we have generated to access the GitHub API. Personal access tokens work like ordinary OAuth access tokens. They can be used instead of a password for Git over HTTPS or can be used to authenticate to the API over basic authentication.

Use the generated token as password when we authenticate it via command line.

```
$ git clone https://github.com/mozilla/addons-frontend.git

>> Username : your_username

>> Password : your_access_token
```

---
Have a great weekend 😉
---