# Edge

> Please note that Edge here refers to the Chromium based version, not the
Trident/MSHTML/whatever based one which is now dead.

## Tab Discarding

Tab Discarding is a feature of Chromium-based browsers where the browser unloads
a tab which has not been focused by the user for a certain amount of time and reloads
it upon entry when the user focuses the tab again.

It is intended to save system memory and improve performance on low-powered hardware.

In my experience, it is extremely annoying, as it will unload web-based versions of
resource-intensive (read: unoptimized) applications such as Slack, Teams, Outlook etc.

On top of that, it does not save that much memory and will lose page state with potentially
unsaved changes in it. It's a pain in the ass and an anti-feature from my point of view,
so I am always eager to disable it on all my devices running Chromium-based browsers.

To disable it, go to:

`edge://flags/#automatic-tab-discarding`

Switch the value to *Disabled* and restart Edge.

To verify this feature is actually disabled, you can go to `edge://discards` at any time
and consult the *Discard Count* column.

## <kbd>Alt+Tab</kbd> Interference

Windows > Settings > System > Multitasking > Alt+Tab > Open Windows Only
