
Extention connects tries connecting to languages in the following fallback order.
- Directory Installation Instance
- Global Installation instance
- Integeated instance in extention

## Status bar Widget

- Available botom right of VS code window. 
- Displays if focused editor file is being watched and error count.
- Hover to find Sandbox-Url.
- Click on widget to see essential links and and Cli commands.

## Shortcuts

Use this code block as your workspace to try out features.

```html
<summon 
demo$button="
	= tfx$duration-200 tx$weight-600 border-none cursor-pointer;
	--button_radius: 0.75em;
	--button_color: #e8e8e8;
	--button_outline_color: #000000;
	font-size: 17px;
	border-radius: var(--button_radius);
	background: var(--button_outline_color);
	& > span {
		= d-flex px-6 py-4 -mod$translate-y-1 -mod$translate-y-1;
		box-sizing: border-box;
		border: 2px solid var(--button_outline_color);
		border-radius: var(--button_radius);
		background: var(--button_color);
		color: var(--button_outline_color);
	}
	&:hover, & > span {
		transform: translateY(-0.33em);
	}
	&:active, & > span {
		transform: translateY(0);
	}
	&[x-preset-]& {
		&[1] {
			--button_color: #ffe17d;
			--button_outline_color: #491505;
		}
		&[2] {
			--button_color: #b3fff9;
			--button_outline_color: #495f7a;
		}
	}
" x-preset-1
> 
    <span> Click Me </span>
</summon>
```
Inspiration: https://uiverse.io/Voxybuns/lucky-fireant-71

### SandBox

- Put cursor on a symclass here `demo$buttom` instance and click on [`Ctrl` + `Alt` + `X`]

### Formating

- Format XCSS-Composition Block of focused file

## Language support

- Files of extentions `.xcss` is treated as markdown.
- Support for `@--attach` and `@--assign` directives css files.
- Block recognitions and syntax highliting on XCSS Embbded syntax.