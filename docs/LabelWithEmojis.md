# Using Emojis in RichTextLabel

Example code of using emojis in **RichTextLabel** (included in addon: *res://addons/emojis-for-godot/examples/LabelWithEmojis.gd*):
```gdscript
@tool
extends RichTextLabel

@export_multiline
var text_with_emojis: String:
	set(value):
		if !is_node_ready():
			return

		text_with_emojis = value
		bbcode_enabled = true
		text = EmojisDB.parse_emojis(value)
	
	get: return text_with_emojis

func _ready() -> void:
	if !Engine.is_editor_hint():
		bbcode_enabled = true
		text = EmojisDB.parse_emojis(text_with_emojis)
```

This is the result of the above code, with `text_with_emojis = "Cool Label :smiling_face_with_sunglasses:  :smiling_face_with_sunglasses, 72:"`
![RichTextLabel Example Screen Shot][LabelWithEmojis-screenshot]

[LabelWithEmojis-screenshot]:assets/label-with-emojis.png
