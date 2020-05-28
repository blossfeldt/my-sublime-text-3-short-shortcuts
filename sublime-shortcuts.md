# Sublime Text 3 - My short Shortcuts

## Navigation

| Shortcut | Description |
| ---------| ----------- |
| <kbd>Ctrl</kbd>+<kbd>Shift</kbd>+<kbd>P</kbd> | command prompt |
| <kbd>Ctrl</kbd>+<kbd>P</kbd> | go to file |
| <kbd>Ctrl</kbd>+<kbd>G</kbd> | go to line |
| <kbd>Ctrl</kbd>+<kbd>R</kbd> | go to methods |
| <kbd>Ctrl</kbd>+<kbd>Shift</kbd>+<kbd>R</kbd> | go to methods in project |
| <kbd>Ctrl</kbd>+<kbd>y</kbd> | find next occurrence of current word [custom sc] |
| <kbd>Alt</kbd>+<kbd>y</kbd> | select all occurrences of current word for multiple editing [custom sc]|
| <kbd>Ctrl</kbd>+<kbd>Shift</kbd>+<kbd>F</kbd> | find in files |

## Selection

| Shortcut | Description |
| ---------| ----------- |
| <kbd>Ctrl</kbd>+<kbd>L</kbd> | select line (repeat select next lines) |
| <kbd>Ctrl</kbd>+<kbd>D</kbd> | select word (repeat select others occurrences in context for multiple editing) |
| <kbd>Ctrl</kbd>+<kbd>Shift</kbd>+<kbd>M</kbd> | select content within brackets |
| <kbd>Ctrl</kbd>+<kbd>Shift</kbd>+<kbd>A</kbd> | select content within tag |
| <kbd>Ctrl</kbd>+<kbd>M</kbd> | jump to matching brackets |

## Editing

| Shortcut | Description |
| ---------| ----------- |
| <kbd>Ctrl</kbd>+<kbd>Shift</kbd>+<kbd>Enter</kbd> | insert line before |
| <kbd>Ctrl</kbd>+<kbd>Enter</kbd> | insert line after |
| <kbd>Ctrl</kbd>+<kbd>Shift</kbd>+<kbd>K</kbd> | delete line |
| <kbd>Ctrl</kbd>+<kbd>K</kbd><kbd>K</kbd> | delete from cursor to end of line |
| <kbd>Ctrl</kbd>+<kbd>K</kbd><kbd>Backspace</kbd> | delete from cursor to start of line |
| <kbd>Ctrl</kbd>+<kbd>Shift</kbd>+<kbd>D</kbd> | duplicate line(s) |
| <kbd>Ctrl</kbd>+<kbd>J</kbd> | join lines |
| <kbd>Ctrl</kbd>+<kbd><</kbd> | comment line [custom sc]|
| <kbd>Ctrl</kbd>+<kbd>Shift</kbd>+<kbd><</kbd> | block comment [custom sc]|
| <kbd>Alt</kbd>+<kbd><</kbd> | autocomplete dropdown suggestions [custom sc] |
| <kbd>Alt</kbd>+<kbd>.</kbd> | close tag |
| <kbd>Ctrl</kbd>+<kbd>H</kbd> | find and replace |

## Split Views / Tabs

| Shortcut | Description |
| ---------| ----------- |
| <kbd>Alt</kbd>+<kbd>Shift</kbd>+<kbd>1</kbd> | single column |
| <kbd>Alt</kbd>+<kbd>Shift</kbd>+<kbd>2</kbd> | two columns |
| <kbd>Alt</kbd>+<kbd>Shift</kbd>+<kbd>5</kbd> | grid (4 groups) |
| <kbd>Ctrl</kbd>+[1,2,3...] | focus group |
| <kbd>Ctrl</kbd>+<kbd>Shift</kbd>+[1,2,3...] | move file to group |
| <kbd>Alt</kbd>+[1,2,3...] | select tab |

## Bookmarks

| Shortcut | Description |
| ---------| ----------- |
| <kbd>Ctrl</kbd>+<kbd>F2</kbd> | toggle bookmark |
| <kbd>F2</kbd> | next bookmark |
| <kbd>Shift</kbd>+<kbd>F2</kbd> | previous bookmark |
| <kbd>Ctrl</kbd>+<kbd>Shift</kbd>+<kbd>F2</kbd> | clear bookmarks |

## Autocomplete <kbd>Tab</kbd>

| Autocomplete |
| ---------|
| htmltag.classname |
| htmltag#ID |
| link |
| script | 

## Sublime Custom Shortcuts Settings

```

[
	{ "keys": ["alt+<"], "command": "auto_complete" },
	{ "keys": ["alt+<"], "command": "replace_completion_with_auto_complete", "context":
		[
			{ "key": "last_command", "operator": "equal", "operand": "insert_best_completion" },
			{ "key": "auto_complete_visible", "operator": "equal", "operand": false },
			{ "key": "setting.tab_completion", "operator": "equal", "operand": true }
		]
	},
	{ "keys": ["ctrl+y"], "command": "find_under" },
	{ "keys": ["alt+y"], "command": "find_all_under" },
	{ "keys": ["ctrl+<"], "command": "toggle_comment", "args": { "block": false } },
	{ "keys": ["ctrl+shift+<"], "command": "toggle_comment", "args": { "block": true } }
]
```
