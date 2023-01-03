# Custom Shield Icons

[![img.shield.io](https://img.shields.io/endpoint?url=https%3A%2F%2Fraw.githubusercontent.com%2FNewSpectrum%2FFree-and-Fancy-Assets%2Fmain%2FShields%2FJSON%2Freferences%2Fshields-provider.json)](https://img.shield.io/)

<br />

---

# JSON Schema

[![Tool](https://img.shields.io/badge/Create-from%20JSON-orange)](https://shields.io/endpoint#:~:text=Customize%20and%20Test)

## Endpoint URL Scheme

For the sake of easy-to-see syntax highlighting, I've setup the following using a __Bash-Styled Code Block__. This way it's easy to spot the __Variables__ even within the __URL Strings__.

```bash
URL="$jsonFile"
STYLE="flat"

Endpoint="https://img.shields.io/endpoint?url=${URL}&style${STYLE}"
```

### The `${URL}`

__IMPORTANT:__

- Be sure to use the __[Raw File URL]__, which starts with:
	- `https://raw.githubusercontent.com/...`
- Should you choose to setup your __Endpoint URL__ manually rather than using the __[Create from JSON](https://shields.io/endpoint#:~:text=Customize%20and%20Test)__ tool, you need to *replace the following characters* with their __[HTML Codes]__
	- __[Embedded URI Characters]__
		- Colon `:`
		- Forward-Slash `/`
		- Back-Slash `\` (from Windows file paths)
			- *Hard time remembering which is which? [Click Here](https://github.com/NewSpectrum/NewSpectrum-Home/wiki)*

| Character | Validity | HTML Code |
| :---:     | :---     | :---:     |
| Colon `:` | :warning: URL<br />:x: Embeded URI | `%3A` |



![Test](url)

```json
{
	"schemaVersion": 1,
	"label": "Provided by",
	"labelColor": "hsl(40,100%,60%)",
	"message": "img.shield.io",
	"color": "hsl(205,75%,35%)",
	"style": "flat"
}
```

## Schema Breakdown


### `schemaVersion`
- [x] __Required__

The __Schema Version__ is __*Always*__ the number `1`

```json
{
	"schemaVersion": 1,
}
```

### `label`
- [x] __Required__

The text contained within the __Left Text Box__. You can leave this blank to omit the left side of the badge entirely.

*This can be overridden by the __[Query String]__.*

### `item`
- [x] __Required__

Description.