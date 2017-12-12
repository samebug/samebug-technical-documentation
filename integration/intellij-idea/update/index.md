# Update the IntelliJ plugin

JetBrains has a pretty good built-in mechanism for plugin updates. However,
sometimes things just don’t work, so let us give you a complete walk-through on it.

## Prerequisites

We assume you already have the Samebug plugin installed. If you need help with the first installation, click [here](/guide/integration/intellij-idea/install).

## Best case: auto-update

![](https://samebug.io/static/images/docs/update-plugin-popup.png "Plugin update notification in the bottom right corner")

Normally, when Idea notices that a plugin update is available, you’ll see a notification. Just click on the link, and Idea will take care of the rest. Don’t forget that you have to restart the IDE for the update to take effect.

## Manual update

![](https://samebug.io/static/images/docs/settings-plugins.png "Settings window can be opened with Ctrl+Alt+S")

If you've disabled auto-update, you have to update Samebug manually. Open the Settings window by pressing `Ctrl`+`Alt`+`S`, select Plugins and type ‘samebug’ in the search box. If there is a new version, just click on the blue ‘Update’ button. Don’t forget that you have to restart the IDE to make the update take effect.

## Worst case: Manual install

![](https://samebug.io/static/images/docs/settings-plugins-remove.png "The IDE does not detect the new version, no Update button")

It can happen that Idea is unable to detect new plugin versions. In this case, you have to download the new plugin version from the JetBrains plugin repository, remove your previous plugin version and install the new one.

1. Download the latest plugin version from the [repository](https://plugins.jetbrains.com/plugin/8174-samebug)
2. Open the Settings window by pressing `Ctrl`+`Alt`+`S`, select Plugins and type ‘samebug’ in the search box. Click ‘Uninstall’. Shed your tears. Restart the IDE.
3. Open the Plugins settings again, and click ‘Install plugin from disk…’ in the bottom right corner. Select the zip file you downloaded in the first step and, again, restart the IDE.
