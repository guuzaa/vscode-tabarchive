# Tab Archive Documentation

## Settings

### `tabarchive.activation`

Can be one of two values:

- `everywhere-except-excluded`: the extension will automatically archive unused tabs in all workspaces, except the ones present in the `Excluded` list;
- `nowhere-except-included`: the extension will automatically archive unused tabs only in the workspaces present in the `Included` list.

The default value is `everywhere-except-excluded`.

> Note: this way of activating tab auto-archiving allows you to do it on a per project/workspace basis, without relying on a project's `.vscode/settings.json` file, as this file is often committed and shared with collaborators.

### `tabarchive.excludedWorkspaces`

> This setting is only used when `tabarchive.activation` is equal to `everywhere-except-excluded`.

List of workspaces in which the extension will not automatically archive unused tabs.

To add a workspace to this list, use the command `Tab Archive: Deactivate automatic archiving of unused tabs for this workspace`.

### `tabarchive.includedWorkspaces`

> This setting is only used when `tabarchive.activation` is equal to `nowhere-except-included`.

List of workspaces in which the extension will automatically archive unused tabs.

To add a workspace to this list, use the command `Tab Archive: Activate automatic archiving of unused tabs for this workspace`.

### `tabarchive.numberOfTabsInGroup`

Unused tabs will be archived only if the number of tabs in the group is greater than this number; enter `0` to archive all unused tabs.

The default value is `5`.

### `tabarchive.tabAgeForAutomaticArchiving`

Number of hours after which an unused tab is automatically archived.

The default value is `12`.

### `tabarchive.yoloMode`

When enabled, unused tabs will be closed without being archived for later retrieval. This means you won't be able to access these tabs from the archived tabs list.

The name comes from "You Only Live Once" - reflecting that tabs are permanently closed rather than saved for later access.

The default value is `false`.
