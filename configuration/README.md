---
description: The appsettings configuration options
---

# Configuration

You can configure the package from within the appsettings.json file using the options below (defaults shown):

<pre class="language-json"><code class="lang-json"><strong>"UmbHostCloudflarePurge": {
</strong>  "ZoneId": "",
  "EmailAddress": "",
  "AuthKey": "",
  "AuthType": 0,
  "Disabled": false,
  "NotificationHandlers": {
    "ContentDeletedNotificationEnabled": true,
    "ContentPublishedNotificationEnabled": true,
    "ContentUnpublishedNotificationEnabled": true,
    "MediaDeletedNotificationEnabled": true,
    "MediaSavedNotificationEnabled": true
  },
  "TreeMenuItems": {
    "TreeMenuItemsEnabled": true,
    "ContentTreeMenuItemEnabled": true,
    "MediaFolderTreeMenuItemEnabled": true,
    "MediaItemTreeMenuItemEnabled": true
  }
}
</code></pre>



| Key                                         | Value                                                                     |
| ------------------------------------------- | ------------------------------------------------------------------------- |
| ZoneId (Required)                           | The Cloudflare Zone id                                                    |
| EmailAddress (Required with Global API Key) | The Cloudflare account email address                                      |
| AuthKey (Required)                          |  The Cloudflare "Global API Key" or "API Token"                           |
| AuthType (Required)                         | <p>0 -> API Token<br>1 -> Global API Key</p>                              |
| Disabled                                    | Set to `true` to globally disable the package                             |
| ContentDeletedNotificationEnabled           | Set to `false` to disable purging on the ContentDeletedNotification       |
| ContentPublishedNotificationEnabled         | Set to `false` to disable purging on the `ContentPublishedNotification`   |
| ContentUnpublishedNotificationEnabled       | Set to `false` to disable purging on the `ContentUnpublishedNotification` |
| MediaDeletedNotificationEnabled             | Set to `false` to disable purging on the `MediaDeletedNotification`       |
| MediaSavedNotificationEnabled               | Set to `false` to disable purging on the `MediaSavedNotification`         |
| TreeMenuItemsEnabled                        | Set to `false` to disable the content and media tree menus                |
| ContentTreeMenuItemEnabled                  | Set to `false` to disable the content tree menu                           |
| MediaFolderTreeMenuItemEnabled              | Set to `false` to disable the media folder tree menu                      |
| MediaItemTreeMenuItemEnabled                | Set to `false` to disable the media item tree menu                        |

