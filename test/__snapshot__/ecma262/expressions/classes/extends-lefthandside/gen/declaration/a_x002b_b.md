# Auto-generated test cases ( Kataw )
- From: kataw/test/__snapshot__/ecma262/expressions/classes/extends-lefthandside/autogen.md
- Path: kataw/test/__snapshot__/ecma262/expressions/classes/extends-lefthandside/gen/declaration
> :: test: declaration
> :: case: a + b
## Options

`````js
{}
`````
## Input

`````js
class A extends a + b {}
`````
## Output

### CST

```javascript
{
    "kind": 122,
    "directives": [],
    "statements": [
        {
            "kind": 178,
            "declareKeyword": null,
            "decorators": null,
            "classKeyword": {
                "kind": 37822544,
                "flags": 80,
                "transformFlags": 0,
                "start": 0,
                "end": 5
            },
            "name": {
                "kind": 134299649,
                "text": "A",
                "rawText": "A",
                "flags": 96,
                "transformFlags": 0,
                "start": 5,
                "end": 7
            },
            "typeParameters": null,
            "tail": {
                "kind": 277,
                "classHeritage": {
                    "kind": 279,
                    "extendsKeyword": {
                        "kind": 4194391,
                        "flags": 80,
                        "transformFlags": 0,
                        "start": 7,
                        "end": 15
                    },
                    "expression": {
                        "kind": 134299649,
                        "text": "a",
                        "rawText": "a",
                        "flags": 96,
                        "transformFlags": 0,
                        "start": 15,
                        "end": 17
                    },
                    "typeParameter": null,
                    "flags": 16,
                    "transformFlags": 0,
                    "start": 15,
                    "end": 17
                },
                "body": {
                    "kind": 303,
                    "elements": [],
                    "flags": 32,
                    "transformFlags": 0,
                    "start": 7,
                    "end": 7
                },
                "flags": 7,
                "transformFlags": 0,
                "start": 32,
                "end": 7
            },
            "flags": 16,
            "transformFlags": 0,
            "start": 0,
            "end": 17
        },
        {
            "kind": 120,
            "expression": {
                "kind": 126,
                "operandToken": {
                    "kind": 99634,
                    "flags": 96,
                    "transformFlags": 0,
                    "start": 17,
                    "end": 19
                },
                "operand": {
                    "kind": 134299649,
                    "text": "b",
                    "rawText": "b",
                    "flags": 96,
                    "transformFlags": 0,
                    "start": 19,
                    "end": 21
                },
                "flags": 32,
                "transformFlags": 16384,
                "start": 17,
                "end": 21
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 17,
            "end": 21
        },
        {
            "kind": 124,
            "block": {
                "kind": 249,
                "statements": [],
                "flags": 16,
                "transformFlags": 0,
                "start": 23,
                "end": 23
            },
            "flags": 16,
            "transformFlags": 0,
            "start": 21,
            "end": 24
        }
    ],
    "isModule": false,
    "source": "class A extends a + b {}",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 24
}
```

### Printed

```javascript

```

### Diagnostics

```javascript
✖ Missing an opening brace - '{ - start: 18, end: 19
✖ '{' is not allowed here. Did you mean ';'? - start: 21, end: 23

```

