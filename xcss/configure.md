## `./configure.jsonc`

```json
{
  "proxymap": [
    {
      "source": "compiled",
      "target": "tutorial",
      "stylesheet": "styles.css",
      "extensions": {
        "html": [
          "id",
          "class"
        ],
        "md": [
          "id",
        ]
      }
    }
  ],
  "vendors": "none",
  "environment": "browser",
}
```

- **`vendors`**  
Specifies vendor prefixing behavior.  
Accepts `"none"` or a Url of a vendor-source.

- **`proxymap`**  
Defines proxy compilation behavior for source-to-target transformation.
    
	- **`source`**  
    Path to the original source directory containing raw project files.
    
	- **`target`**  
    Proxy output directory. Acts as a working compilation target for the source folder.
	
    - **`stylesheet`**  
    Stylesheet appended to the final compiled output. Located within the target directory.
        
	- **`extensions`**  
	    
    Maps file types to attributes where symbolic classes will be injected.  
    `"html": ["class"]` targets HTML files and mapped array contains list of watching tag attributes.
    > Watching attributes will be discussed later in [../tutorial/1.operators.md](../tutorial/1.operators.md)

- **`environment`**  
Used by Editor extention for standerd css completion in compilation blocks.  
Refer Extention walkthorugh to see in action at [../tutorial/0.extention.md](../tutorial/0.extention.md).

### Developer Options
 
- Documented there itself, and will be mentioned in instances when its used.
- Additional options will be present w.r.t. the flavour you are using.

---

- Checkout file: [./#at-rules.css](./#at-rules.css)
- Next Chapter: [./#constants.md](./#constants.md)
