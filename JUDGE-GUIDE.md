# Check a release in Jira Cloud

Release Proof reads the issues visible to the current Jira user and groups unfinished work, unresolved blocking links and attachment filenames by release. A release lead can open the underlying issue before deciding whether to ship.

Watch the [72-second Jira walkthrough](https://youtu.be/UJHUFseVgnU). The same [MP4 recording](https://raw.githubusercontent.com/LeeJinMing/release-proof-for-jira/main/Release-Proof-Demo.mp4) is available for download. The recording follows three demonstration issues on a development site.

## Install and open the project page

1. Use a Jira Cloud test site where you can install apps. Codegeist reviewers can find the production installation link in the submission's installation field. Select **Get app**, choose your site, review **View Jira issue data** and install for Jira. If the site selector is empty, ask the administrator of your test site to install the app. A site that already has the app can open it from project navigation.
2. Open a Jira project with releases enabled. Create an unreleased version and assign that **Fix version** to each of the three issues below.
3. Open **Release Proof** in project navigation. In a tabbed layout, look under **More** or the extra-tabs menu. Select the test version and click **Check release**.

| Test issue | Setup |
| --- | --- |
| Release story | Set to In Progress and add an “is blocked by” link to the bug. |
| Blocking bug | Set to To Do. |
| Evidence story | Set to Done and attach a small sample file named `delivery-confirmation-test.txt`. |

## Compare two reports

| What to check | Bug to do | Bug moved to Done |
| --- | ---: | ---: |
| Visible work items | 3 | 3 |
| Unfinished or unknown | 2 | 1 |
| Open dependency links | 1 | 0 |
| Issues without attachments | 2 | 2 |

Open the blocking issue from the first report, move it to Done, allow Jira search to reflect the change and rerun the report. The evidence story should show the same attachment filename in both runs. Check the item itself for the contents of the attachment. Users with different issue permissions can see different totals. [Privacy notice](PRIVACY.md).
