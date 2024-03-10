# Emojis for Godot

![addon-in-action]

Addon for easy using Emojis in Godot UI.
- is compatible with emojis Unicode 15.1
- uses [Google Noto Emojis Color font][noto-emoji]
- uses [json data generated using python][emoji-json]

## How to use

## Nodes

- [EmojiIcon]: A node that displays an Emoji.
- [EmojiButton]: A node that displays an Emoji as a button.

## Singletons

- [EmojisDB]: singleton for easy use of emojis anywhere in your project.

## Examples

- [Using Emojis in RichTextLabel]

[Using Emojis in RichTextLabel]:LabelWithEmojis.md
[EmojisDB]:emojis.md
[EmojiIcon]:EmojiIcon.md
[EmojiButton]:EmojiButton.md
[addon-in-action]:assets/addon-in-action.png
[noto-emoji]:https://github.com/googlefonts/noto-emoji/tree/main/png
[emoji-json]:https://github.com/rakugoteam/Emojis-For-Godot/tree/godot-4/addons/emojis-for-godot/emojis/gen_json.py
