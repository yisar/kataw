# Kataw parser test case

## Options

`````js
{ jsx: true, disableWebCompat: true, module: true }
`````

## Input

`````js
import 'x' assert {,}
`````

## Output

### CST

```javascript
{
    "kind": 122,
    "directives": [],
    "statements": [
        {
            "kind": 263,
            "importKeyword": {
                "kind": 37814364,
                "flags": 80,
                "transformFlags": 0,
                "start": 0,
                "end": 6
            },
            "typeKeyword": null,
            "typeofKeyword": null,
            "fromClause": null,
            "moduleSpecifier": {
                "kind": 201392131,
                "text": "x",
                "rawText": "'x'",
                "flags": 4194400,
                "transformFlags": 0,
                "start": 6,
                "end": 10
            },
            "importClause": null,
            "flags": 80,
            "transformFlags": 0,
            "start": 0,
            "end": 10
        },
        {
            "kind": 120,
            "expression": {
                "kind": 134299649,
                "text": "assert",
                "rawText": "assert",
                "flags": 96,
                "transformFlags": 0,
                "start": 10,
                "end": 17
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 10,
            "end": 17
        },
        {
            "kind": 124,
            "block": {
                "kind": 249,
                "statements": [],
                "flags": 16,
                "transformFlags": 0,
                "start": 19,
                "end": 19
            },
            "flags": 16,
            "transformFlags": 0,
            "start": 17,
            "end": 19
        }
    ],
    "isModule": true,
    "source": "import 'x' assert {,}",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 21
}
```

### Printed

```javascript

```

### Diagnostics

```javascript
✖ '; ' is not allowed here. Did you mean ';'? - start: 10, end: 17
✖ '{' is not allowed here. Did you mean ';'? - start: 17, end: 19
✖ The parser expected to find a '}' to match the '{' token here - start: 19, end: 20
✖ Declaration or statement expected - start: 20, end: 21

```

