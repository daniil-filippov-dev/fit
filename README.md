# FIT

A minimalist File gIT (FIT) to sync your files across mobile and desktop devices using GitHub.
This plugin is designed to be as simple as possible, enabling one-click sync that works universally across mobile and desktop.

### Relevant plugins
There are other community plugins with more advanced git features, if you need features such as branching of your repo, [Git](https://github.com/denolehov/obsidian-git) is a nice plugin to check out. This plugin focuses on making the core git feature (push and pull) available across devices (mobile and desktop). To achieve this, this repo implements a simple git system with pure typescript and utilizes [Octokit/core.js](https://github.com/octokit/core.js/) which supports all modern browsers to interface with GitHub REST API.

**Note:** This plugin is still in alpha, please backup your vault before using this plugin.

# How to use

### One click sync

### Pull and push separately



https://github.com/joshuakto/fit/assets/34743132/863d0241-a528-495a-b6f8-717a519cdc11




# Setup
1. Create a repo on GitHub
2. Create a personal access token (refers to [Github: creating a personal access token](https://docs.github.com/en/enterprise-server@3.9/authentication/keeping-your-account-and-data-secure/managing-your-personal-access-tokens#creating-a-personal-access-token))
3. Enters the created token along with other relevant GitHub information on the Fit settings tab.
<img width="1113" alt="Screenshot 2024-03-02 at 6 17 24 PM" src="https://github.com/joshuakto/fit/assets/34743132/c6679d4e-fd7f-476a-a9cc-43dfd732b534">

# Roadmap
1. Enable integration with existing vault (current setup only works for empty vault synced with empty repo from the start)
2. Improve user notification
   - allow user to opt in to get list of file changes in Notice
3. Allow users to resolve conflicting file changes

# Acknowledgements
 - This plugin is built using [Obsidian Sample Plugin](https://github.com/obsidianmd/obsidian-sample-plugin) as a template.
 - This plugin uses [Octokit](https://github.com/octokit/core.js/) to interface with github rest api across devices.

<!--- 
## Releasing new releases

- Update your `manifest.json` with your new version number, such as `1.0.1`, and the minimum Obsidian version required for your latest release.
- Update your `versions.json` file with `"new-plugin-version": "minimum-obsidian-version"` so older versions of Obsidian can download an older version of your plugin that's compatible.
- Create new GitHub release using your new version number as the "Tag version". Use the exact version number, don't include a prefix `v`. See here for an example: https://github.com/obsidianmd/obsidian-sample-plugin/releases
- Upload the files `manifest.json`, `main.js`, `styles.css` as binary attachments. Note: The manifest.json file must be in two places, first the root path of your repository and also in the release.
- Publish the release.

> You can simplify the version bump process by running `npm version patch`, `npm version minor` or `npm version major` after updating `minAppVersion` manually in `manifest.json`.
> The command will bump version in `manifest.json` and `package.json`, and add the entry for the new version to `versions.json`

## Adding your plugin to the community plugin list

- Check https://github.com/obsidianmd/obsidian-releases/blob/master/plugin-review.md
- Publish an initial version.
- Make sure you have a `README.md` file in the root of your repo.
- Make a pull request at https://github.com/obsidianmd/obsidian-releases to add your plugin.
  
## Manually installing the plugin

- Copy over `main.js`, `styles.css`, `manifest.json` to your vault `VaultFolder/.obsidian/plugins/your-plugin-id/`.
--->
