# Edge

> Please note that Edge here refers to the Chromium based version, not the
Trident/MSHTML/whatever based one which is now dead.

## Tab Discarding

Tab Discarding is a feature of Chromium-based browsers where the browser unloads
a tab which has not been focused by the user for a certain amount of time and
reloads it upon entry when the user focuses the tab again.

It is intended to save system memory and improve performance on low-powered
hardware.

In my experience, it is extremely annoying, as it will unload web-based versions
of resource-intensive (read: unoptimized) applications such as Slack, Teams,
Outlook etc.

On top of that, it does not save that much memory and will lose page state with
potentially unsaved changes in it. It's a pain in the ass and an anti-feature
from my point of view, so I am always eager to disable it on all my devices
running Chromium-based browsers.

To disable it, go to:

`edge://flags/#automatic-tab-discarding`

Switch the value to *Disabled* and restart Edge.

To verify this feature is actually disabled, you can go to `edge://discards` at
any time and consult the *Discard Count* column.

## <kbd>Alt+Tab</kbd> Interference

Windows > Settings > System > Multitasking > Alt+Tab > Open Windows Only

## To-Do

### Test out the hack to disabled Restore Pages

https://www.laptopmag.com/articles/edge-browser-stop-tab-restore

Hopefully that message can be turned off, because Edge asks it every time it is
not closed explicitly, but instead by restarting the computer etc. The problem
is it restores even pinned tabs, so every time this modal is accepted, the tabs
that are pinned and already open, double up so you have twice the amount of
pinned tabs. That's too annoying to keep this feature turned on.

https://microsoft.visualstudio.com/Edge/_workitems/edit/32212309
