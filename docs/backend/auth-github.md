---
title: GitHub Authentication
---

# GitHub App and Authentication

Dev.to allows you to authenticate using Github. To use this authentication method in local development, you will need to set up a GitHub App and retrieves keys. Then you'll need to provide theses keys to the Rails application.

1. [Sign in](https://github.com/settings/applications/new) in your GitHub account.

2. Fill in the form with an application name, descriptions and URLs `http://localhost:3000/`. Replace the `3000` port if you run DEV on other port.
   ![github-1](https://user-images.githubusercontent.com/22895284/51085500-877a6c00-173a-11e9-913a-0dccad234cf3.png)

3. You will be redirected in the app's **Developer settings**. Here you will find the keys. Change them accordingly (name of Github key -> name of our `ENV` variable):

   ```
   Client ID -> GITHUB_KEY
   Client Secret -> GITHUB_SECRET
   ```

   ![github-2](https://user-images.githubusercontent.com/22895284/51085862-49337b80-173f-11e9-8503-f8251d07f458.png)

4. You will need a personal token as well. From the same dashboard, navigate to **Personal access tokens** and generate a new token.
   ![github-3](https://user-images.githubusercontent.com/22895284/51085863-49337b80-173f-11e9-81bf-1c1e38035a7a.png)
5. Fill in the token description and generate the token.

6. Be sure that you copy the token right away, because it is the only time you will see it. Change it accordingly.

   ```
   Personal access tokens -> GITHUB_TOKEN
   ```

   ![github-4](https://user-images.githubusercontent.com/22895284/51085865-49cc1200-173f-11e9-86a8-7e7e1db408a0.png)

7. Done.
