# NavigationViewToggleButtonReproApp

Bug: The toggle pane button of a navigation view control has incorrect width/styling on startup.

This is the same issue as discussed in this old open bug on github: [Pane toggle button is clipped in NavigationView · Issue #5854](https://github.com/microsoft/microsoft-ui-xaml/issues/5854)

Expected behavior: toggle button's width should be the correct size at all times and remain consistent.

Workarounds: causing the pane to collapse (by resizing the window or manually closing and reopening the pane) and changing the Pane title. Looking into the source code, this seems to cause the button to recalculate its width to the correct one.
