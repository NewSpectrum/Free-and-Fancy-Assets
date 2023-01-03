# Custom Shield Icons

[![img.shield.io](image)](https://img.shield.io/)

<br />

---

# JSON Schema

```json
{
	"schemaVersion": 1,
	"label": "Provided by",
	"labelColor": "hsl(45, 100%, 60%)"
	"message": "img.shield.io",
	"color": "hsl(205, 75%, 45%)",
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