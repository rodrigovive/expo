---
title: Programmatic Access
---


## Programmatic Access

When setting up CI or writing a script to help manage your projects, we recommend avoiding using your username and password to authenticate. With these credentials, anyone would be able to log in and use your account.

Instead of providing credentials, you can generate tokens that will allow you to manage each integration point separately. Anyone who has access to these tokens will be able to perform actions against your account. Please treat them with the same care as a user password. In case something is leaked, you can revoke these tokens to block access.

### Personal Account: Personal Access Tokens

You can create Personal Access Tokens from the [Access Tokens page](https://expo.dev/settings/access-tokens) on your dashboard. Anyone with this token can perform actions on your behalf. That applies to all content on your Personal Account, as well as any Personal Accounts or Organizations that you have been granted access to.

### Organizations: Bot Users & Access Tokens

Organizations can create Bot Users to take actions on resources owned by the Organization.  Bot Users can be assigned [a role](/working-together) to limit the actions they are authorized to perform.  Bot users cannot sign in to any Expo products, cannot own any projects themselves, and can only authenticate via an access token.

### Using Access Tokens

You can use any tokens you have created to perform actions with the Expo CLI (other than signing in and out). To use tokens, you need to define an environment variable, like `EXPO_TOKEN="token"`, before running commands.

If you are using Github Actions, [you can configure the `expo-token` property](https://github.com/expo/expo-github-action#configuration-options) to include this environment variable in all of the job steps.

Common situations where access tokens are useful:

- Publish or build from CI without providing your Expo username and password
- Renew a token to keep it as secure as possible; no need to reset your password and sign out of all sessions
- Give someone (or a script) one-time access to your project with limited permissions

### Revoking Access Tokens

In case a token was accidentally leaked, you can revoke it without changing your username and password. When you revoke the access token, you block all access to your account using this token. To do this, go to the [Access Token page](https://expo.dev/settings/access-tokens) on your dashboard and delete the token you want to revoke.
