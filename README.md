# Leashguard: Privacy Policy

_Last updated: November 2026_

Leashguard is a Forge app for Jira. It checks changes that Rovo agents try to make in Jira against a policy set by project admins: each change is allowed, held for approval, or blocked. Every decision is recorded in a log.

## What Leashguard stores

Leashguard stores data only in Atlassian Forge storage (Forge Key-Value Store). That storage is hosted by Atlassian and kept separately for each site where the app is installed. It stores:

- **Policy settings** for each Jira project: the freeze switch, rate limits, protected priorities and labels, the bulk-change guard, and an optional approver account ID.
- **A decision log** for each project, with a record for each checked change. A record holds the time, the Atlassian account ID of the requester or approver, the issue key, the type of change, a short summary of the change (any text is cut off at 200 characters), the verdict, and the rule that applied. The log keeps at most 500 entries per project, and the oldest entries are dropped first.
- **Pending approvals** for each issue, until they are approved, rejected or withdrawn.
- **Usage counters** that enforce the rate limits, for each project and each Atlassian account ID.

## What Leashguard does not do

- It does not send data outside Atlassian. The app makes no external network calls and has no egress permissions.
- It does not use any third-party analytics, tracking, advertising or AI services of its own.
- It does not store names, email addresses, passwords or API tokens, only Atlassian account IDs.
- It does not sell or share data.

## Permissions

Leashguard asks only for the Jira scopes it needs: to read issues, write the changes it guards, use app storage, and let Rovo call its actions. The current scope list is shown on the install screen.

## Retention and deletion

Data stays in the site's Forge storage while the app is installed. When the app is uninstalled, Atlassian deletes the app's stored data under its standard Forge data-retention rules. A site admin can also clear a project's data by uninstalling the app.

## Data residency

Storage location follows Atlassian's Forge data-residency rules for the installing site.

## Contact

For questions or requests, please open an issue on the Leashguard project page.

## Changes

If this policy changes, we'll update the date at the top of this page.
