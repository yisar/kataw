# Kataw parser test case

## Input

`````js
var let;

var foo, let;

try { } catch (let) { }

function let() { }

(function let() { })

function foo(let) { }

function foo(bar, let) { }

let = 1;

var foo = let = 1;

let * 2;

++let;

let++;

(function f() { let: 34 });

function let(let) { let: let(let + let(0)); }

({ let: 1 })

({ get let() { 1 } })

let(100)

L: let
x

L: let
{x}
`````

## Output

### CST

```javascript
{
    "kind": 122,
    "directives": [],
    "statements": [
        {
            "kind": 155,
            "declareKeyword": null,
            "varKeyword": {
                "kind": 37757002,
                "flags": 80,
                "transformFlags": 0,
                "start": 0,
                "end": 3
            },
            "declarationList": {
                "kind": 156,
                "declarations": [
                    {
                        "kind": 157,
                        "binding": {
                            "kind": 134299649,
                            "text": "let",
                            "rawText": "let",
                            "flags": 96,
                            "transformFlags": 0,
                            "start": 3,
                            "end": 7
                        },
                        "type": null,
                        "initializer": null,
                        "flags": 16,
                        "transformFlags": 4224,
                        "start": 3,
                        "end": 7
                    }
                ],
                "flags": 16,
                "transformFlags": 0,
                "start": 3,
                "end": 7
            },
            "flags": 16,
            "transformFlags": 0,
            "start": 0,
            "end": 8
        },
        {
            "kind": 155,
            "declareKeyword": null,
            "varKeyword": {
                "kind": 37757002,
                "flags": 81,
                "transformFlags": 0,
                "start": 8,
                "end": 13
            },
            "declarationList": {
                "kind": 156,
                "declarations": [
                    {
                        "kind": 157,
                        "binding": {
                            "kind": 134299649,
                            "text": "foo",
                            "rawText": "foo",
                            "flags": 96,
                            "transformFlags": 0,
                            "start": 13,
                            "end": 17
                        },
                        "type": null,
                        "initializer": null,
                        "flags": 16,
                        "transformFlags": 4224,
                        "start": 13,
                        "end": 17
                    },
                    {
                        "kind": 157,
                        "binding": {
                            "kind": 134299649,
                            "text": "let",
                            "rawText": "let",
                            "flags": 96,
                            "transformFlags": 0,
                            "start": 18,
                            "end": 22
                        },
                        "type": null,
                        "initializer": null,
                        "flags": 16,
                        "transformFlags": 4224,
                        "start": 18,
                        "end": 22
                    }
                ],
                "flags": 16,
                "transformFlags": 0,
                "start": 13,
                "end": 22
            },
            "flags": 16,
            "transformFlags": 0,
            "start": 8,
            "end": 23
        },
        {
            "kind": 159,
            "tryKeyword": {
                "kind": 37757027,
                "flags": 81,
                "transformFlags": 0,
                "start": 23,
                "end": 28
            },
            "block": {
                "kind": 124,
                "block": {
                    "kind": 249,
                    "statements": [],
                    "flags": 16,
                    "transformFlags": 0,
                    "start": 30,
                    "end": 30
                },
                "flags": 16,
                "transformFlags": 0,
                "start": 28,
                "end": 32
            },
            "catchClause": {
                "kind": 173,
                "catchKeyword": {
                    "kind": 4202575,
                    "flags": 80,
                    "transformFlags": 0,
                    "start": 32,
                    "end": 38
                },
                "catchParameter": {
                    "kind": 134299649,
                    "text": "let",
                    "rawText": "let",
                    "flags": 96,
                    "transformFlags": 0,
                    "start": 40,
                    "end": 43
                },
                "block": {
                    "kind": 124,
                    "block": {
                        "kind": 249,
                        "statements": [],
                        "flags": 16,
                        "transformFlags": 0,
                        "start": 46,
                        "end": 46
                    },
                    "flags": 16,
                    "transformFlags": 0,
                    "start": 44,
                    "end": 48
                },
                "flags": 80,
                "transformFlags": 0,
                "start": 32,
                "end": 48
            },
            "finallyKeyword": null,
            "finallyBlock": null,
            "flags": 16,
            "transformFlags": 0,
            "start": 23,
            "end": 48
        },
        {
            "kind": 176,
            "declareKeyword": null,
            "asyncKeyword": null,
            "functionKeyword": {
                "kind": 37822554,
                "flags": 65,
                "transformFlags": 0,
                "start": 48,
                "end": 58
            },
            "asteriskToken": null,
            "name": {
                "kind": 134299649,
                "text": "let",
                "rawText": "let",
                "flags": 96,
                "transformFlags": 0,
                "start": 58,
                "end": 62
            },
            "typeParameters": null,
            "formalParameterList": {
                "kind": 214,
                "formalParameters": [],
                "trailingComma": false,
                "flags": 32,
                "transformFlags": 0,
                "start": 63,
                "end": 63
            },
            "contents": {
                "kind": 216,
                "functionStatementList": {
                    "kind": 217,
                    "directives": [],
                    "statements": [],
                    "flags": 32,
                    "transformFlags": 0,
                    "start": 66,
                    "end": 66
                },
                "flags": 32,
                "transformFlags": 0,
                "start": 64,
                "end": 68
            },
            "returnType": null,
            "flags": 16,
            "transformFlags": 0,
            "start": 48,
            "end": 68
        },
        {
            "kind": 120,
            "expression": {
                "kind": 121,
                "expression": {
                    "kind": 177,
                    "asyncKeyword": null,
                    "functionKeyword": {
                        "kind": 37822554,
                        "flags": 64,
                        "transformFlags": 0,
                        "start": 71,
                        "end": 79
                    },
                    "asteriskToken": null,
                    "name": {
                        "kind": 134299649,
                        "text": "let",
                        "rawText": "let",
                        "flags": 96,
                        "transformFlags": 0,
                        "start": 79,
                        "end": 83
                    },
                    "typeParameters": null,
                    "formalParameterList": {
                        "kind": 214,
                        "formalParameters": [],
                        "trailingComma": false,
                        "flags": 32,
                        "transformFlags": 0,
                        "start": 84,
                        "end": 84
                    },
                    "contents": {
                        "kind": 216,
                        "functionStatementList": {
                            "kind": 217,
                            "directives": [],
                            "statements": [],
                            "flags": 32,
                            "transformFlags": 0,
                            "start": 87,
                            "end": 87
                        },
                        "flags": 32,
                        "transformFlags": 0,
                        "start": 85,
                        "end": 89
                    },
                    "returnType": null,
                    "flags": 32,
                    "transformFlags": 0,
                    "start": 71,
                    "end": 89
                },
                "flags": 33,
                "transformFlags": 0,
                "start": 68,
                "end": 90
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 68,
            "end": 90
        },
        {
            "kind": 176,
            "declareKeyword": null,
            "asyncKeyword": null,
            "functionKeyword": {
                "kind": 37822554,
                "flags": 65,
                "transformFlags": 0,
                "start": 90,
                "end": 100
            },
            "asteriskToken": null,
            "name": {
                "kind": 134299649,
                "text": "foo",
                "rawText": "foo",
                "flags": 96,
                "transformFlags": 0,
                "start": 100,
                "end": 104
            },
            "typeParameters": null,
            "formalParameterList": {
                "kind": 214,
                "formalParameters": [
                    {
                        "kind": 134299649,
                        "text": "let",
                        "rawText": "let",
                        "flags": 96,
                        "transformFlags": 0,
                        "start": 105,
                        "end": 108
                    }
                ],
                "trailingComma": false,
                "flags": 32,
                "transformFlags": 0,
                "start": 105,
                "end": 108
            },
            "contents": {
                "kind": 216,
                "functionStatementList": {
                    "kind": 217,
                    "directives": [],
                    "statements": [],
                    "flags": 32,
                    "transformFlags": 0,
                    "start": 111,
                    "end": 111
                },
                "flags": 32,
                "transformFlags": 0,
                "start": 109,
                "end": 113
            },
            "returnType": null,
            "flags": 16,
            "transformFlags": 0,
            "start": 90,
            "end": 113
        },
        {
            "kind": 176,
            "declareKeyword": null,
            "asyncKeyword": null,
            "functionKeyword": {
                "kind": 37822554,
                "flags": 65,
                "transformFlags": 0,
                "start": 113,
                "end": 123
            },
            "asteriskToken": null,
            "name": {
                "kind": 134299649,
                "text": "foo",
                "rawText": "foo",
                "flags": 96,
                "transformFlags": 0,
                "start": 123,
                "end": 127
            },
            "typeParameters": null,
            "formalParameterList": {
                "kind": 214,
                "formalParameters": [
                    {
                        "kind": 134299649,
                        "text": "bar",
                        "rawText": "bar",
                        "flags": 96,
                        "transformFlags": 0,
                        "start": 128,
                        "end": 131
                    },
                    {
                        "kind": 134299649,
                        "text": "let",
                        "rawText": "let",
                        "flags": 96,
                        "transformFlags": 0,
                        "start": 132,
                        "end": 136
                    }
                ],
                "trailingComma": false,
                "flags": 32,
                "transformFlags": 0,
                "start": 128,
                "end": 136
            },
            "contents": {
                "kind": 216,
                "functionStatementList": {
                    "kind": 217,
                    "directives": [],
                    "statements": [],
                    "flags": 32,
                    "transformFlags": 0,
                    "start": 139,
                    "end": 139
                },
                "flags": 32,
                "transformFlags": 0,
                "start": 137,
                "end": 141
            },
            "returnType": null,
            "flags": 16,
            "transformFlags": 0,
            "start": 113,
            "end": 141
        },
        {
            "kind": 120,
            "expression": {
                "kind": 125,
                "left": {
                    "kind": 134299649,
                    "text": "let",
                    "rawText": "let",
                    "flags": 97,
                    "transformFlags": 0,
                    "start": 141,
                    "end": 146
                },
                "operatorToken": {
                    "kind": 4125,
                    "flags": 96,
                    "transformFlags": 0,
                    "start": 146,
                    "end": 148
                },
                "right": {
                    "kind": 201392130,
                    "text": 1,
                    "rawText": "1",
                    "flags": 96,
                    "transformFlags": 0,
                    "start": 148,
                    "end": 150
                },
                "flags": 0,
                "transformFlags": 128,
                "start": 141,
                "end": 150
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 141,
            "end": 151
        },
        {
            "kind": 155,
            "declareKeyword": null,
            "varKeyword": {
                "kind": 37757002,
                "flags": 81,
                "transformFlags": 0,
                "start": 151,
                "end": 156
            },
            "declarationList": {
                "kind": 156,
                "declarations": [
                    {
                        "kind": 157,
                        "binding": {
                            "kind": 134299649,
                            "text": "foo",
                            "rawText": "foo",
                            "flags": 96,
                            "transformFlags": 0,
                            "start": 156,
                            "end": 160
                        },
                        "type": null,
                        "initializer": {
                            "kind": 125,
                            "left": {
                                "kind": 134299649,
                                "text": "let",
                                "rawText": "let",
                                "flags": 96,
                                "transformFlags": 0,
                                "start": 162,
                                "end": 166
                            },
                            "operatorToken": {
                                "kind": 4125,
                                "flags": 96,
                                "transformFlags": 0,
                                "start": 166,
                                "end": 168
                            },
                            "right": {
                                "kind": 201392130,
                                "text": 1,
                                "rawText": "1",
                                "flags": 96,
                                "transformFlags": 0,
                                "start": 168,
                                "end": 170
                            },
                            "flags": 0,
                            "transformFlags": 128,
                            "start": 162,
                            "end": 170
                        },
                        "flags": 16,
                        "transformFlags": 4224,
                        "start": 156,
                        "end": 170
                    }
                ],
                "flags": 16,
                "transformFlags": 0,
                "start": 156,
                "end": 170
            },
            "flags": 16,
            "transformFlags": 0,
            "start": 151,
            "end": 171
        },
        {
            "kind": 120,
            "expression": {
                "kind": 198,
                "left": {
                    "kind": 134299649,
                    "text": "let",
                    "rawText": "let",
                    "flags": 97,
                    "transformFlags": 0,
                    "start": 171,
                    "end": 176
                },
                "operatorToken": {
                    "kind": 201360950,
                    "flags": 96,
                    "transformFlags": 32,
                    "start": 176,
                    "end": 178
                },
                "right": {
                    "kind": 201392130,
                    "text": 2,
                    "rawText": "2",
                    "flags": 96,
                    "transformFlags": 0,
                    "start": 178,
                    "end": 180
                },
                "flags": 97,
                "transformFlags": 5120,
                "start": 171,
                "end": 180
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 171,
            "end": 181
        },
        {
            "kind": 120,
            "expression": {
                "kind": 128,
                "operandToken": {
                    "kind": 196635,
                    "flags": 97,
                    "transformFlags": 0,
                    "start": 181,
                    "end": 185
                },
                "operand": {
                    "kind": 134299649,
                    "text": "let",
                    "rawText": "let",
                    "flags": 96,
                    "transformFlags": 0,
                    "start": 185,
                    "end": 188
                },
                "flags": 32,
                "transformFlags": 16384,
                "start": 181,
                "end": 188
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 181,
            "end": 189
        },
        {
            "kind": 120,
            "expression": {
                "kind": 127,
                "operandToken": {
                    "kind": 196635,
                    "flags": 96,
                    "transformFlags": 0,
                    "start": 194,
                    "end": 196
                },
                "operand": {
                    "kind": 134299649,
                    "text": "let",
                    "rawText": "let",
                    "flags": 97,
                    "transformFlags": 0,
                    "start": 189,
                    "end": 194
                },
                "flags": 32,
                "transformFlags": 0,
                "start": 189,
                "end": 196
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 189,
            "end": 197
        },
        {
            "kind": 120,
            "expression": {
                "kind": 121,
                "expression": {
                    "kind": 177,
                    "asyncKeyword": null,
                    "functionKeyword": {
                        "kind": 37822554,
                        "flags": 64,
                        "transformFlags": 0,
                        "start": 200,
                        "end": 208
                    },
                    "asteriskToken": null,
                    "name": {
                        "kind": 134299649,
                        "text": "f",
                        "rawText": "f",
                        "flags": 96,
                        "transformFlags": 0,
                        "start": 208,
                        "end": 210
                    },
                    "typeParameters": null,
                    "formalParameterList": {
                        "kind": 214,
                        "formalParameters": [],
                        "trailingComma": false,
                        "flags": 32,
                        "transformFlags": 0,
                        "start": 211,
                        "end": 211
                    },
                    "contents": {
                        "kind": 216,
                        "functionStatementList": {
                            "kind": 217,
                            "directives": [],
                            "statements": [
                                {
                                    "kind": 163,
                                    "label": {
                                        "kind": 134299649,
                                        "text": "let",
                                        "rawText": "let",
                                        "flags": 96,
                                        "transformFlags": 0,
                                        "start": 214,
                                        "end": 218
                                    },
                                    "colonToken": {
                                        "kind": 21,
                                        "flags": 64,
                                        "transformFlags": 0,
                                        "start": 218,
                                        "end": 219
                                    },
                                    "statement": {
                                        "kind": 120,
                                        "expression": {
                                            "kind": 201392130,
                                            "text": 34,
                                            "rawText": "34",
                                            "flags": 96,
                                            "transformFlags": 0,
                                            "start": 219,
                                            "end": 222
                                        },
                                        "flags": 16,
                                        "transformFlags": 4096,
                                        "start": 219,
                                        "end": 222
                                    },
                                    "flags": 16,
                                    "transformFlags": 0,
                                    "start": 214,
                                    "end": 222
                                }
                            ],
                            "flags": 32,
                            "transformFlags": 0,
                            "start": 214,
                            "end": 222
                        },
                        "flags": 32,
                        "transformFlags": 0,
                        "start": 212,
                        "end": 224
                    },
                    "returnType": null,
                    "flags": 32,
                    "transformFlags": 0,
                    "start": 200,
                    "end": 224
                },
                "flags": 33,
                "transformFlags": 0,
                "start": 197,
                "end": 225
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 197,
            "end": 226
        },
        {
            "kind": 176,
            "declareKeyword": null,
            "asyncKeyword": null,
            "functionKeyword": {
                "kind": 37822554,
                "flags": 65,
                "transformFlags": 0,
                "start": 226,
                "end": 236
            },
            "asteriskToken": null,
            "name": {
                "kind": 134299649,
                "text": "let",
                "rawText": "let",
                "flags": 96,
                "transformFlags": 0,
                "start": 236,
                "end": 240
            },
            "typeParameters": null,
            "formalParameterList": {
                "kind": 214,
                "formalParameters": [
                    {
                        "kind": 134299649,
                        "text": "let",
                        "rawText": "let",
                        "flags": 96,
                        "transformFlags": 0,
                        "start": 241,
                        "end": 244
                    }
                ],
                "trailingComma": false,
                "flags": 32,
                "transformFlags": 0,
                "start": 241,
                "end": 244
            },
            "contents": {
                "kind": 216,
                "functionStatementList": {
                    "kind": 217,
                    "directives": [],
                    "statements": [
                        {
                            "kind": 163,
                            "label": {
                                "kind": 134299649,
                                "text": "let",
                                "rawText": "let",
                                "flags": 96,
                                "transformFlags": 0,
                                "start": 247,
                                "end": 251
                            },
                            "colonToken": {
                                "kind": 21,
                                "flags": 64,
                                "transformFlags": 0,
                                "start": 251,
                                "end": 252
                            },
                            "statement": {
                                "kind": 120,
                                "expression": {
                                    "kind": 131,
                                    "expression": {
                                        "kind": 134299649,
                                        "text": "let",
                                        "rawText": "let",
                                        "flags": 96,
                                        "transformFlags": 0,
                                        "start": 252,
                                        "end": 256
                                    },
                                    "argumentList": {
                                        "kind": 256,
                                        "elements": [
                                            {
                                                "kind": 198,
                                                "left": {
                                                    "kind": 134299649,
                                                    "text": "let",
                                                    "rawText": "let",
                                                    "flags": 96,
                                                    "transformFlags": 0,
                                                    "start": 257,
                                                    "end": 260
                                                },
                                                "operatorToken": {
                                                    "kind": 99634,
                                                    "flags": 96,
                                                    "transformFlags": 0,
                                                    "start": 260,
                                                    "end": 262
                                                },
                                                "right": {
                                                    "kind": 131,
                                                    "expression": {
                                                        "kind": 134299649,
                                                        "text": "let",
                                                        "rawText": "let",
                                                        "flags": 96,
                                                        "transformFlags": 0,
                                                        "start": 262,
                                                        "end": 266
                                                    },
                                                    "argumentList": {
                                                        "kind": 256,
                                                        "elements": [
                                                            {
                                                                "kind": 201392130,
                                                                "text": 0,
                                                                "rawText": "0",
                                                                "flags": 96,
                                                                "transformFlags": 0,
                                                                "start": 267,
                                                                "end": 268
                                                            }
                                                        ],
                                                        "trailingComma": false,
                                                        "flags": 32,
                                                        "transformFlags": 0,
                                                        "start": 267,
                                                        "end": 268
                                                    },
                                                    "flags": 32,
                                                    "transformFlags": 1,
                                                    "start": 262,
                                                    "end": 269
                                                },
                                                "flags": 96,
                                                "transformFlags": 5120,
                                                "start": 257,
                                                "end": 269
                                            }
                                        ],
                                        "trailingComma": false,
                                        "flags": 32,
                                        "transformFlags": 0,
                                        "start": 257,
                                        "end": 269
                                    },
                                    "flags": 32,
                                    "transformFlags": 1,
                                    "start": 252,
                                    "end": 270
                                },
                                "flags": 16,
                                "transformFlags": 4096,
                                "start": 252,
                                "end": 271
                            },
                            "flags": 16,
                            "transformFlags": 0,
                            "start": 247,
                            "end": 271
                        }
                    ],
                    "flags": 32,
                    "transformFlags": 0,
                    "start": 247,
                    "end": 271
                },
                "flags": 32,
                "transformFlags": 0,
                "start": 245,
                "end": 273
            },
            "returnType": null,
            "flags": 16,
            "transformFlags": 0,
            "start": 226,
            "end": 273
        },
        {
            "kind": 120,
            "expression": {
                "kind": 131,
                "expression": {
                    "kind": 121,
                    "expression": {
                        "kind": 220,
                        "propertyList": {
                            "kind": 218,
                            "properties": [
                                {
                                    "kind": 219,
                                    "asteriskToken": null,
                                    "left": {
                                        "kind": 134299649,
                                        "text": "let",
                                        "rawText": "let",
                                        "flags": 96,
                                        "transformFlags": 0,
                                        "start": 277,
                                        "end": 281
                                    },
                                    "right": {
                                        "kind": 201392130,
                                        "text": 1,
                                        "rawText": "1",
                                        "flags": 96,
                                        "transformFlags": 0,
                                        "start": 282,
                                        "end": 284
                                    },
                                    "flags": 32,
                                    "transformFlags": 128,
                                    "start": 277,
                                    "end": 284
                                }
                            ],
                            "trailingComma": false,
                            "flags": 16,
                            "transformFlags": 0,
                            "start": 277,
                            "end": 284
                        },
                        "flags": 48,
                        "transformFlags": 8,
                        "start": 276,
                        "end": 286
                    },
                    "flags": 35,
                    "transformFlags": 0,
                    "start": 273,
                    "end": 287
                },
                "argumentList": {
                    "kind": 256,
                    "elements": [
                        {
                            "kind": 220,
                            "propertyList": {
                                "kind": 218,
                                "properties": [
                                    {
                                        "kind": 351,
                                        "asyncKeyword": null,
                                        "asteriskToken": null,
                                        "getKeyword": {
                                            "kind": 16498,
                                            "flags": 96,
                                            "transformFlags": 0,
                                            "start": 291,
                                            "end": 295
                                        },
                                        "setKeyword": null,
                                        "method": {
                                            "kind": 209,
                                            "name": {
                                                "kind": 134299649,
                                                "text": "let",
                                                "rawText": "let",
                                                "flags": 96,
                                                "transformFlags": 0,
                                                "start": 295,
                                                "end": 299
                                            },
                                            "typeParameters": null,
                                            "formalParameterList": {
                                                "kind": 214,
                                                "formalParameters": [],
                                                "trailingComma": false,
                                                "flags": 1056,
                                                "transformFlags": 0,
                                                "start": 300,
                                                "end": 301
                                            },
                                            "returnType": null,
                                            "contents": {
                                                "kind": 216,
                                                "functionStatementList": {
                                                    "kind": 217,
                                                    "directives": [],
                                                    "statements": [
                                                        {
                                                            "kind": 120,
                                                            "expression": {
                                                                "kind": 201392130,
                                                                "text": 1,
                                                                "rawText": "1",
                                                                "flags": 96,
                                                                "transformFlags": 0,
                                                                "start": 303,
                                                                "end": 305
                                                            },
                                                            "flags": 16,
                                                            "transformFlags": 4096,
                                                            "start": 303,
                                                            "end": 305
                                                        }
                                                    ],
                                                    "flags": 32,
                                                    "transformFlags": 0,
                                                    "start": 303,
                                                    "end": 305
                                                },
                                                "flags": 32,
                                                "transformFlags": 0,
                                                "start": 301,
                                                "end": 307
                                            },
                                            "flags": 1056,
                                            "transformFlags": 0,
                                            "start": 299,
                                            "end": 307
                                        },
                                        "flags": 32,
                                        "transformFlags": 0,
                                        "start": 291,
                                        "end": 307
                                    }
                                ],
                                "trailingComma": false,
                                "flags": 16,
                                "transformFlags": 0,
                                "start": 291,
                                "end": 307
                            },
                            "flags": 48,
                            "transformFlags": 8,
                            "start": 290,
                            "end": 309
                        }
                    ],
                    "trailingComma": false,
                    "flags": 33,
                    "transformFlags": 0,
                    "start": 290,
                    "end": 309
                },
                "flags": 33,
                "transformFlags": 1,
                "start": 273,
                "end": 310
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 273,
            "end": 310
        },
        {
            "kind": 120,
            "expression": {
                "kind": 131,
                "expression": {
                    "kind": 134299649,
                    "text": "let",
                    "rawText": "let",
                    "flags": 97,
                    "transformFlags": 0,
                    "start": 310,
                    "end": 315
                },
                "argumentList": {
                    "kind": 256,
                    "elements": [
                        {
                            "kind": 201392130,
                            "text": 100,
                            "rawText": "100",
                            "flags": 96,
                            "transformFlags": 0,
                            "start": 316,
                            "end": 319
                        }
                    ],
                    "trailingComma": false,
                    "flags": 32,
                    "transformFlags": 0,
                    "start": 316,
                    "end": 319
                },
                "flags": 32,
                "transformFlags": 1,
                "start": 310,
                "end": 320
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 310,
            "end": 320
        },
        {
            "kind": 163,
            "label": {
                "kind": 134299649,
                "text": "L",
                "rawText": "L",
                "flags": 97,
                "transformFlags": 0,
                "start": 320,
                "end": 323
            },
            "colonToken": {
                "kind": 21,
                "flags": 64,
                "transformFlags": 0,
                "start": 323,
                "end": 324
            },
            "statement": {
                "kind": 120,
                "expression": {
                    "kind": 134299649,
                    "text": "let",
                    "rawText": "let",
                    "flags": 96,
                    "transformFlags": 0,
                    "start": 324,
                    "end": 328
                },
                "flags": 16,
                "transformFlags": 4096,
                "start": 324,
                "end": 328
            },
            "flags": 17,
            "transformFlags": 0,
            "start": 320,
            "end": 328
        },
        {
            "kind": 120,
            "expression": {
                "kind": 134299649,
                "text": "x",
                "rawText": "x",
                "flags": 97,
                "transformFlags": 0,
                "start": 328,
                "end": 330
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 328,
            "end": 330
        },
        {
            "kind": 163,
            "label": {
                "kind": 134299649,
                "text": "L",
                "rawText": "L",
                "flags": 97,
                "transformFlags": 0,
                "start": 330,
                "end": 333
            },
            "colonToken": {
                "kind": 21,
                "flags": 64,
                "transformFlags": 0,
                "start": 333,
                "end": 334
            },
            "statement": {
                "kind": 120,
                "expression": {
                    "kind": 134299649,
                    "text": "let",
                    "rawText": "let",
                    "flags": 96,
                    "transformFlags": 0,
                    "start": 334,
                    "end": 338
                },
                "flags": 16,
                "transformFlags": 4096,
                "start": 334,
                "end": 338
            },
            "flags": 17,
            "transformFlags": 0,
            "start": 330,
            "end": 338
        },
        {
            "kind": 124,
            "block": {
                "kind": 249,
                "statements": [
                    {
                        "kind": 120,
                        "expression": {
                            "kind": 134299649,
                            "text": "x",
                            "rawText": "x",
                            "flags": 96,
                            "transformFlags": 0,
                            "start": 340,
                            "end": 341
                        },
                        "flags": 16,
                        "transformFlags": 4096,
                        "start": 340,
                        "end": 341
                    }
                ],
                "flags": 16,
                "transformFlags": 0,
                "start": 340,
                "end": 341
            },
            "flags": 17,
            "transformFlags": 0,
            "start": 338,
            "end": 342
        }
    ],
    "isModule": false,
    "source": "var let;\n\nvar foo, let;\n\ntry { } catch (let) { }\n\nfunction let() { }\n\n(function let() { })\n\nfunction foo(let) { }\n\nfunction foo(bar, let) { }\n\nlet = 1;\n\nvar foo = let = 1;\n\nlet * 2;\n\n++let;\n\nlet++;\n\n(function f() { let: 34 });\n\nfunction let(let) { let: let(let + let(0)); }\n\n({ let: 1 })\n\n({ get let() { 1 } })\n\nlet(100)\n\nL: let\nx\n\nL: let\n{x}",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 342
}
```

### Printed

```javascript
var let;
var foo, let;

try {} catch (let) {}

function let() {}

(function let() {});

function foo(let) {}

function foo(bar, let) {}

let = 1;

var foo = let = 1;

let * 2;

++ let;

let++;

(function f() {
    let:  34;
  });

function let(let) {
  let:  let(let + let(0));
}

({ let: 1 })({ get let() {
    1;
  } });

let(100);

L:  let;

x;

L:  let;

{
  x;
}

```

### Diagnostics

```javascript
✔ No errors
```

