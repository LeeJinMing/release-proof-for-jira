# Release Proof for Jira Privacy Notice

Release Proof displays release information inside Jira Cloud. When a user checks a release, the app uses Atlassian Forge to read Jira project and version identifiers, work item summaries, types, statuses, priorities, dependencies, and attachment filenames. Jira controls which information is available to the signed-in user. The app displays filenames and links to Jira work items. It does not open or download attachment contents.

The app processes report data in the Jira page for the current session. It does not keep a separate copy of Jira work item data, write to Jira, or send report content to a service operated by the developer. The app has no account system or developer-operated analytics. Atlassian hosts Jira and Forge and explains its handling of data in the [Atlassian Privacy Policy](https://www.atlassian.com/legal/privacy-policy).

Removing access in Jira limits what the app can read. A Jira site administrator can uninstall the app through Jira's app management screen.

For questions about the app or this notice, use [GitHub Issues](https://github.com/LeeJinMing/release-proof-for-jira/issues). Share diagnostic details only after removing confidential information from screenshots or examples.
