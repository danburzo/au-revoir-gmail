# au-revoir-gmail

Notes on migrating away from a gmail.com email address. 

## Introduction

Having your own domain for your email address future-proofs your online presence. You can switch email services, or host your own email server, by simply changing your domain's DNS records.

But: email addresses are widely used as an authentication, identification and account recovery mechanism. As such, deciding to renounce the Gmail address you've been using for years is not as straightforward as, let's say, picking DuckDuckGo instead of Google Search.

It's a gradual process that can span several years, but the feeling of freedom and control can be very gratifying.

## New habits

Some useful things you start doing:

1. __Sign up to all new things using your new email.__ Otherwise you just create more work for yourself in the future. Don't use your Gmail address, and skip _Sign in with Google_.
2. __Set up a password manager__ to collect all your online accounts, new and existing, in one place. (I use, and enjoy, 1Password.)
3. __Forward all mail__ you get on your Gmail address to your new email address (and optionally have it delete the mails after they've been forwarded)
4. __Observe the kinds of mail__ you get on Gmail, and make the necessary changes so you'll get them on your new email address the next time around: collect account information in the password manager, unsubscribe from newsletters and re-subscribe with the new email, etc.

## Notes on specific services

### Signed up with Google

It's easy to skip registration and just sign up with your Google account for things. Luckily, on your [Google Account](https://myaccount.google.com/) page, under <kbd>Security > Signing in to other sites</kbd>, you have a handy list of all websites and apps with which you've used your Google Account. You can go through them one by one and:

* If you don't need the account, delete it;
* If you still need it, switch to user/password authentication, and update your associated email address in the process.

Then revoke access for the website from the overview page.

### Git & GitHub

If you've been working with Git, chances are your Gmail address is embedded in each of your commits. Altering the history of a repository you've shared with other people is not feasible in most cases. What you can do instead is use the new email address going forward.

You can change the email address Git uses with:

```bash
git config --global user.email "you@your-domain.com"
```

In case you've overriden the global config in particular repositories, don't forget to update it there as well.

If you're using GitHub, you'll need to change your primary email address [as described here](https://help.github.com/en/articles/setting-your-commit-email-address). Unfortunately, you'll also need to keep the Gmail address around as a secondary email in GitHub. Otherwise, all commits signed with your Gmail address will be detached from your profile.

> Note that it _is_ possible to rewrite Git history to amend the email address retroactively, but it's usually a very bad idea. For the sake of science, [here's how you'd do it](https://help.github.com/en/articles/changing-author-info).

### Apple ID

> I'll be attempting to change the email address associated with my Apple ID, and will write down any setbacks.

### Software licenses

> You can store all your software licenses in 1Password for easy access.

Some software licenses are a combination of email address and key. Once you've purchased it, you'll probably be able to use the license as usual even if you were to delete your Google account — _as long as you still have the license_. To recover a lost license will possibly require still having access to your Gmail address. 

You can try contacting the software issuer to get a new license associated to your new email address, just in case.

## Further reading

* [The Lobste.rs discussion](https://lobste.rs/s/urxqti/migrating_away_from_entrenched_gmail_com)
* [Bye, bye, Google](https://defn.io/2019/02/04/bye-bye-google/) by Bogdan Popa
* [The simplicity of dropping Google in 2018](https://macwright.org/2018/04/26/leaving-google.html) by Tom MacWright
