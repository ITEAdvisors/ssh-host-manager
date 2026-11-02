# Privacy policy: SSH Host Manager

Last updated: 1 November 2026. Published by ITEAdvisors.

## Summary
SSH Host Manager does not collect, store or send personal information to its author or
to any third party. It has no accounts, no analytics, no telemetry, no crash reports, no
advertising and no update checks. It only connects to the servers you add yourself.

## What the app handles, on your computer only
- **Server details you type in:** names, addresses, ports and user names. They are saved
  in your OpenSSH `config` file.
- **Host keys:** the fingerprints of servers you chose to trust. They are saved in your
  OpenSSH `known_hosts` file.
- **Keys:** the app creates a private and a public key for each server. The private key
  stays on your computer in the folder you chose. The public key is sent to the server
  you added, when you tell the app to install it.
- **Passwords and passphrases:** you type them into the terminal window of `ssh`,
  `ssh-keygen` or `ssh-add`, which are part of Windows. The app never receives, shows,
  stores or sends them.
- **The app's own settings:** the folder you picked, which version of the first-start
  notice you accepted, how long you chose to keep keys unlocked, and the file paths of
  keys that must be locked again when the app closes. These are in
  `%LOCALAPPDATA%\SSHHostManager\settings.json`. They contain no key material and no
  passwords.

## What leaves your computer
- Connections from `ssh` to the servers you added, on the port you set. The app also
  opens a plain connection to that address and port to check that it can be reached.
- If you enter a host name instead of an IP address, Windows looks the name up through
  your usual DNS server, as it does for any program.
- If you choose a folder that OneDrive or another sync service watches, that service,
  not this app, copies the files in it.
- Nothing else. The app contains no web client.

## Links
The app has two links, **Support this app** (a voluntary donation page hosted by Stripe)
and **Project page** (GitHub). Each opens in your default web browser only when you click
it. The app does not contact those sites. What they collect is governed by their own
privacy policies.

## Microsoft Store
If you install the app from the Microsoft Store, Microsoft may collect information about
the download and use of apps, as described in Microsoft's own privacy statement. The app
itself adds no data collection.

## Children
The app is a tool for managing SSH access. It is not directed at children and collects
no information from anyone.

## Your control
- **Delete a server** removes it from your `config` and its host key from `known_hosts`.
  You can also delete its key file in the same step.
- **Uninstalling the app** removes the app and its settings file. The keys, `config` and
  `known_hosts` are your files in your `.ssh` folder, so they stay until you delete them.
- You can check the network claims yourself: open Windows Resource Monitor, go to the
  **Network** tab and watch `SSHHostManager.exe` and `ssh.exe`.

## Changes
If this policy changes, the new version is published here with a new date.

## Contact
Open an issue at https://github.com/ITEAdvisors/ssh-host-manager/issues
