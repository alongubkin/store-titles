store-titles
============

### Description
Store module that allows players to buy custom titles in the store. Titles are chat tags that are added to your name when you send a chat message.

### Requirements

* [Store](https://forums.alliedmods.net/showthread.php?t=207157)
* [Simple Chat Processor (Redux)](http://forums.alliedmods.net/showthread.php?t=198501) 
* [SMJansson](https://forums.alliedmods.net/showthread.php?t=184604)

### Features

* **Compatibility** - This plugin doesn't break other plugins that add tags or change colors, as long as they use Simple Chat Processor.
* **Cross game support** - Each title has 2 versions: Source 2009 version, and other games version. This allows you to use more colors in games like TF2 and CS:S.

### Installation

Download the `store-titles.zip` archive from the plugin thread and extract to your `sourcemod` folder intact. Then, navigate to `configs/store/sql-init-scripts/` and execute `titles.sql` in your database.

### Adding More Titles

Until the web panel for the store will be ready, you'll need to update the database directly to add more items. To do that, open your phpMyAdmin and duplicate one of the existing titles you have. Change `name`, `display_name`, `description` and `attrs` to customize the new title. 

The attrs field should look like:

    {
        "text": "{green}Sir",
        "colorful_text": "{fullred}Sir"
    }
