# Kataw parser test case

## Input

`````js
( x = y ) => {
  'use strict';
}

( { x}  ) => {
  'use strict';
}
`````

## Output

### CST

```javascript
{
    "kind": 122,
    "directives": [],
    "statements": [
        {
            "kind": 120,
            "expression": {
                "kind": 271,
                "asyncKeyword": null,
                "typeParameters": null,
                "arrowPatameterList": {
                    "kind": 342,
                    "parameters": [
                        {
                            "kind": 281,
                            "ellipsisToken": null,
                            "left": {
                                "kind": 134299649,
                                "text": "x",
                                "rawText": "x",
                                "flags": 96,
                                "transformFlags": 0,
                                "start": 1,
                                "end": 3
                            },
                            "optionalToken": null,
                            "type": null,
                            "right": {
                                "kind": 134299649,
                                "text": "y",
                                "rawText": "y",
                                "flags": 96,
                                "transformFlags": 0,
                                "start": 5,
                                "end": 7
                            },
                            "flags": 32,
                            "transformFlags": 4096,
                            "start": 0,
                            "end": 7
                        }
                    ],
                    "trailingComma": false,
                    "flags": 34,
                    "transformFlags": 0,
                    "start": 1,
                    "end": 9
                },
                "returnType": null,
                "arrowToken": {
                    "kind": 10,
                    "flags": 64,
                    "transformFlags": 0,
                    "start": 9,
                    "end": 12
                },
                "contents": {
                    "kind": 216,
                    "functionStatementList": {
                        "kind": 217,
                        "directives": [
                            {
                                "kind": 201392131,
                                "text": "use strict",
                                "rawText": "'use strict'",
                                "flags": 4194401,
                                "transformFlags": 0,
                                "start": 14,
                                "end": 29
                            }
                        ],
                        "statements": [],
                        "flags": 4194337,
                        "transformFlags": 0,
                        "start": 14,
                        "end": 30
                    },
                    "flags": 32,
                    "transformFlags": 0,
                    "start": 12,
                    "end": 32
                },
                "flags": 34,
                "transformFlags": 0,
                "start": 0,
                "end": 32
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 0,
            "end": 32
        },
        {
            "kind": 120,
            "expression": {
                "kind": 271,
                "asyncKeyword": null,
                "typeParameters": null,
                "arrowPatameterList": {
                    "kind": 342,
                    "parameters": [
                        {
                            "kind": 212,
                            "propertyList": {
                                "kind": 213,
                                "properties": [
                                    {
                                        "kind": 134299649,
                                        "text": "x",
                                        "rawText": "x",
                                        "flags": 96,
                                        "transformFlags": 0,
                                        "start": 37,
                                        "end": 39
                                    }
                                ],
                                "trailingComma": false,
                                "flags": 32,
                                "transformFlags": 0,
                                "start": 37,
                                "end": 39
                            },
                            "flags": 48,
                            "transformFlags": 0,
                            "start": 35,
                            "end": 40
                        }
                    ],
                    "trailingComma": false,
                    "flags": 35,
                    "transformFlags": 0,
                    "start": 35,
                    "end": 43
                },
                "returnType": null,
                "arrowToken": {
                    "kind": 10,
                    "flags": 64,
                    "transformFlags": 0,
                    "start": 43,
                    "end": 46
                },
                "contents": {
                    "kind": 216,
                    "functionStatementList": {
                        "kind": 217,
                        "directives": [
                            {
                                "kind": 201392131,
                                "text": "use strict",
                                "rawText": "'use strict'",
                                "flags": 4194401,
                                "transformFlags": 0,
                                "start": 48,
                                "end": 63
                            }
                        ],
                        "statements": [],
                        "flags": 4194337,
                        "transformFlags": 0,
                        "start": 48,
                        "end": 64
                    },
                    "flags": 32,
                    "transformFlags": 0,
                    "start": 46,
                    "end": 66
                },
                "flags": 35,
                "transformFlags": 0,
                "start": 32,
                "end": 66
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 32,
            "end": 66
        }
    ],
    "isModule": false,
    "source": "( x = y ) => {\n  'use strict';\n}\n\n( { x}  ) => {\n  'use strict';\n}",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 66
}
```

### Printed

```javascript

```

### Diagnostics

```javascript
✖ 'use strict' directive cannot be used with non-simple parameter list. - start: 29, end: 30
✖ 'use strict' directive cannot be used with non-simple parameter list. - start: 63, end: 64

```

