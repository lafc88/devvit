# About Devvit apps

Devvit apps are designed to interact with Reddit communities.

## App lifecycle

Devvit apps go through three stages.

| Stage    | Description                                                                                                                                                                    |
| -------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Private  | When you are building and testing your app, it’s only visible to you, and it can only be installed by you in small subreddits with fewer than 200 subscribers.                 |
| Unlisted | After you publish your app, it is still only visible to you in the Apps directory, but you can install it on larger subreddits.                                                |
| Public   | Once your app review form has been approved by the Developer Platform team, your app is available in the Apps directory and can be installed by mods and admins across Reddit. |

## App accounts

An app account is a separate user account just for your app. It is automatically generated when you upload your app.

Once a mod or admin installs your app, the app account appears as a user in the mod list. When the app is executed, the action comes from the app’s user account. This is helpful for tracking posts and comments.

The app account has the same permissions that are granted to your app.

## App permissions

App permissions help users understand how your app will interact with a subreddit and users.

If your app accesses user data or interacts with the UI, that information is listed in the [Apps](https://developers.reddit.com) directory and in the CLI on installation. Permissions fall into one of three categories.

| **Category**                         | **Description**                                                                                              | **Capabilities involved**                                                                                                                                                             |
| ------------------------------------ | ------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **UI**                               | Permissions your app needs for the UI elements it uses.                                                      | Menu actions, custom posts, or asset use all require UI permissions.                                                                                                                  |
| **User data handling**               | Permissions your app needs for the way it manages user data.                                                 | The specific permissions your app requires will depend on the capabilities you’ve used: app settings, key value store, HTTP fetch, media, Redis, Reddit API, scheduler, and triggers. |
| **Moderator permissions** (required) | Permission your app needs to create a mod account with _everything_ permissions on the installing subreddit. | This permission is required for every app.                                                                                                                                            |

Here’s an example of the permissions displayed on the app detail page in the Developer Portal.

![app permissions](./assets/app_permissions.png)

## App versions

When you update your app, every subreddit that has installed your app has to be **manually updated** to the new version (don’t worry, this won’t last forever). To update your subreddit app installation:

1. Go to [My Communities](https://developers.reddit.com/my/communities) from the profile dropdown in the Developer Portal.
2. Click the community you want to view.
3. When a new version of an app is available for a given subreddit, you will see a blue **Update** button next to the app tile. Click the button and follow the prompts to upgrade each community.

![app update](./assets/app-update.png)
