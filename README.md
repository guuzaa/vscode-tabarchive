# Tab Archive 🎉

- **Automatically archives tabs that have not been used for a defined length of time** — 12 hours, by default.

- **Only archives tabs if the group contains more than a defined number of tabs** — 5, by default.

- **Doesn't archive tabs that have changes, tabs that are pinned, and the active tab** of each group.

The age of the opened tabs is persisted when the workspace is closed, and resumes incrementing when the workspace is reopened.

## Commands

In addition to automatically archiving unused tabs, the extension provides the following commands.

### `Tab Archive: Archive As Many Tabs As Possible`

Archive all tabs except the 5 (by default) most recently used ones, in each group. (It also doesn't archive tabs with changes, pinned tabs, and the active one.)

### `Tab Archive: List Recently Archived Tabs`

List the tabs that have been automatically archived since the workspace was opened. Use it to adjust the `tabarchive.numberOfTabsInGroup` and `tabarchive.tabAgeForAutomaticArchiving` settings if you find that tabs are archived more/less often than you wish.

### `Tab Archive: Clear All Archived Tabs`

Clear all archived tabs from memory and storage. This is useful when you want to start fresh and remove all previously archived tabs.

### `Tab Archive: Close All Diff Tabs`

Close all diff tabs in all tab groups. This is useful when you want to quickly clean up after reviewing multiple file changes.

### `Tab Archive: Close All Deleted File Tabs`

Close all tabs that reference files that no longer exist on disk. This is useful when you want to clean up tabs for files that have been deleted outside of VS Code.

## Configuration

For detailed information about all available settings, please see the [documentation](docs.md).

## Downloads

It's live on [VSCode Extension Market](https://marketplace.visualstudio.com/items?itemName=guza.tabarchive) and [Open-VSX](https://open-vsx.org/extension/guza/tabarchive).
