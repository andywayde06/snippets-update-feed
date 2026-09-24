# snippets-update-feed
Snippets Update Feed

This repository hosts the update metadata used by the Snippets desktop application.

The app checks the published version.json file to determine whether a newer version is available.

Example:

{
  "latest": "0.4.1",
  "download_url": "https://github.com/USERNAME/snippets/releases/download/v0.4.1/SnippetsSetup-0.4.1.exe",
  "release_notes": "Bug fixes and stability improvements."
}

The update feed is intended to be served over HTTPS using GitHub Pages.

Updating the feed

When releasing a new version of Snippets:

Publish the new installer.
Update latest in version.json.
Set download_url to the new installer.
Update the release notes.
Commit and push the changes.

The Snippets application will detect the new version the next time the user checks for updates.
