# Kataw parser test case

## Input

`````js
a + b;
a - b;
a * b;
a / b;
a % b;
a ** b;
a & b;
a | b;
a ^ b;
a << b;
a >> b;
a >>> b;
a === b;
a !== b;
a == b;
a != b;
a, b;

a + '' == b;

typeof a == b + '';

typeof a == 'b';
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
                "kind": 198,
                "left": {
                    "kind": 134299649,
                    "text": "a",
                    "rawText": "a",
                    "flags": 96,
                    "transformFlags": 0,
                    "start": 0,
                    "end": 1
                },
                "operatorToken": {
                    "kind": 99634,
                    "flags": 96,
                    "transformFlags": 0,
                    "start": 1,
                    "end": 3
                },
                "right": {
                    "kind": 134299649,
                    "text": "b",
                    "rawText": "b",
                    "flags": 96,
                    "transformFlags": 0,
                    "start": 3,
                    "end": 5
                },
                "flags": 96,
                "transformFlags": 5120,
                "start": 0,
                "end": 5
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 0,
            "end": 6
        },
        {
            "kind": 120,
            "expression": {
                "kind": 198,
                "left": {
                    "kind": 134299649,
                    "text": "a",
                    "rawText": "a",
                    "flags": 97,
                    "transformFlags": 0,
                    "start": 6,
                    "end": 8
                },
                "operatorToken": {
                    "kind": 134318643,
                    "flags": 96,
                    "transformFlags": 0,
                    "start": 8,
                    "end": 10
                },
                "right": {
                    "kind": 134299649,
                    "text": "b",
                    "rawText": "b",
                    "flags": 96,
                    "transformFlags": 0,
                    "start": 10,
                    "end": 12
                },
                "flags": 97,
                "transformFlags": 5120,
                "start": 6,
                "end": 12
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 6,
            "end": 13
        },
        {
            "kind": 120,
            "expression": {
                "kind": 198,
                "left": {
                    "kind": 134299649,
                    "text": "a",
                    "rawText": "a",
                    "flags": 97,
                    "transformFlags": 0,
                    "start": 13,
                    "end": 15
                },
                "operatorToken": {
                    "kind": 201360950,
                    "flags": 96,
                    "transformFlags": 32,
                    "start": 15,
                    "end": 17
                },
                "right": {
                    "kind": 134299649,
                    "text": "b",
                    "rawText": "b",
                    "flags": 96,
                    "transformFlags": 0,
                    "start": 17,
                    "end": 19
                },
                "flags": 97,
                "transformFlags": 5120,
                "start": 13,
                "end": 19
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 13,
            "end": 20
        },
        {
            "kind": 120,
            "expression": {
                "kind": 198,
                "left": {
                    "kind": 134299649,
                    "text": "a",
                    "rawText": "a",
                    "flags": 97,
                    "transformFlags": 0,
                    "start": 20,
                    "end": 22
                },
                "operatorToken": {
                    "kind": 35640,
                    "flags": 96,
                    "transformFlags": 32,
                    "start": 22,
                    "end": 24
                },
                "right": {
                    "kind": 134299649,
                    "text": "b",
                    "rawText": "b",
                    "flags": 96,
                    "transformFlags": 0,
                    "start": 24,
                    "end": 26
                },
                "flags": 97,
                "transformFlags": 5120,
                "start": 20,
                "end": 26
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 20,
            "end": 27
        },
        {
            "kind": 120,
            "expression": {
                "kind": 198,
                "left": {
                    "kind": 134299649,
                    "text": "a",
                    "rawText": "a",
                    "flags": 97,
                    "transformFlags": 0,
                    "start": 27,
                    "end": 29
                },
                "operatorToken": {
                    "kind": 35639,
                    "flags": 96,
                    "transformFlags": 32,
                    "start": 29,
                    "end": 31
                },
                "right": {
                    "kind": 134299649,
                    "text": "b",
                    "rawText": "b",
                    "flags": 96,
                    "transformFlags": 0,
                    "start": 31,
                    "end": 33
                },
                "flags": 97,
                "transformFlags": 5120,
                "start": 27,
                "end": 33
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 27,
            "end": 34
        },
        {
            "kind": 120,
            "expression": {
                "kind": 198,
                "left": {
                    "kind": 134299649,
                    "text": "a",
                    "rawText": "a",
                    "flags": 97,
                    "transformFlags": 0,
                    "start": 34,
                    "end": 36
                },
                "operatorToken": {
                    "kind": 35897,
                    "flags": 96,
                    "transformFlags": 0,
                    "start": 36,
                    "end": 39
                },
                "right": {
                    "kind": 134299649,
                    "text": "b",
                    "rawText": "b",
                    "flags": 96,
                    "transformFlags": 0,
                    "start": 39,
                    "end": 41
                },
                "flags": 97,
                "transformFlags": 5120,
                "start": 34,
                "end": 41
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 34,
            "end": 42
        },
        {
            "kind": 120,
            "expression": {
                "kind": 198,
                "left": {
                    "kind": 134299649,
                    "text": "a",
                    "rawText": "a",
                    "flags": 97,
                    "transformFlags": 0,
                    "start": 42,
                    "end": 44
                },
                "operatorToken": {
                    "kind": 134252103,
                    "flags": 96,
                    "transformFlags": 0,
                    "start": 44,
                    "end": 46
                },
                "right": {
                    "kind": 134299649,
                    "text": "b",
                    "rawText": "b",
                    "flags": 96,
                    "transformFlags": 0,
                    "start": 46,
                    "end": 48
                },
                "flags": 97,
                "transformFlags": 5120,
                "start": 42,
                "end": 48
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 42,
            "end": 49
        },
        {
            "kind": 120,
            "expression": {
                "kind": 198,
                "left": {
                    "kind": 134299649,
                    "text": "a",
                    "rawText": "a",
                    "flags": 97,
                    "transformFlags": 0,
                    "start": 49,
                    "end": 51
                },
                "operatorToken": {
                    "kind": 134251592,
                    "flags": 96,
                    "transformFlags": 0,
                    "start": 51,
                    "end": 53
                },
                "right": {
                    "kind": 134299649,
                    "text": "b",
                    "rawText": "b",
                    "flags": 96,
                    "transformFlags": 0,
                    "start": 53,
                    "end": 55
                },
                "flags": 97,
                "transformFlags": 5120,
                "start": 49,
                "end": 55
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 49,
            "end": 56
        },
        {
            "kind": 120,
            "expression": {
                "kind": 198,
                "left": {
                    "kind": 134299649,
                    "text": "a",
                    "rawText": "a",
                    "flags": 97,
                    "transformFlags": 0,
                    "start": 56,
                    "end": 58
                },
                "operatorToken": {
                    "kind": 134251849,
                    "flags": 96,
                    "transformFlags": 0,
                    "start": 58,
                    "end": 60
                },
                "right": {
                    "kind": 134299649,
                    "text": "b",
                    "rawText": "b",
                    "flags": 96,
                    "transformFlags": 0,
                    "start": 60,
                    "end": 62
                },
                "flags": 97,
                "transformFlags": 5120,
                "start": 56,
                "end": 62
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 56,
            "end": 63
        },
        {
            "kind": 120,
            "expression": {
                "kind": 198,
                "left": {
                    "kind": 134299649,
                    "text": "a",
                    "rawText": "a",
                    "flags": 97,
                    "transformFlags": 0,
                    "start": 63,
                    "end": 65
                },
                "operatorToken": {
                    "kind": 35140,
                    "flags": 96,
                    "transformFlags": 64,
                    "start": 65,
                    "end": 68
                },
                "right": {
                    "kind": 134299649,
                    "text": "b",
                    "rawText": "b",
                    "flags": 96,
                    "transformFlags": 0,
                    "start": 68,
                    "end": 70
                },
                "flags": 97,
                "transformFlags": 5120,
                "start": 63,
                "end": 70
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 63,
            "end": 71
        },
        {
            "kind": 120,
            "expression": {
                "kind": 198,
                "left": {
                    "kind": 134299649,
                    "text": "a",
                    "rawText": "a",
                    "flags": 97,
                    "transformFlags": 0,
                    "start": 71,
                    "end": 73
                },
                "operatorToken": {
                    "kind": 35141,
                    "flags": 96,
                    "transformFlags": 64,
                    "start": 73,
                    "end": 76
                },
                "right": {
                    "kind": 134299649,
                    "text": "b",
                    "rawText": "b",
                    "flags": 96,
                    "transformFlags": 0,
                    "start": 76,
                    "end": 78
                },
                "flags": 97,
                "transformFlags": 5120,
                "start": 71,
                "end": 78
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 71,
            "end": 79
        },
        {
            "kind": 120,
            "expression": {
                "kind": 198,
                "left": {
                    "kind": 134299649,
                    "text": "a",
                    "rawText": "a",
                    "flags": 97,
                    "transformFlags": 0,
                    "start": 79,
                    "end": 81
                },
                "operatorToken": {
                    "kind": 35142,
                    "flags": 96,
                    "transformFlags": 64,
                    "start": 81,
                    "end": 85
                },
                "right": {
                    "kind": 134299649,
                    "text": "b",
                    "rawText": "b",
                    "flags": 96,
                    "transformFlags": 0,
                    "start": 85,
                    "end": 87
                },
                "flags": 97,
                "transformFlags": 5120,
                "start": 79,
                "end": 87
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 79,
            "end": 88
        },
        {
            "kind": 120,
            "expression": {
                "kind": 198,
                "left": {
                    "kind": 134299649,
                    "text": "a",
                    "rawText": "a",
                    "flags": 97,
                    "transformFlags": 0,
                    "start": 88,
                    "end": 90
                },
                "operatorToken": {
                    "kind": 34620,
                    "flags": 96,
                    "transformFlags": 16,
                    "start": 90,
                    "end": 94
                },
                "right": {
                    "kind": 134299649,
                    "text": "b",
                    "rawText": "b",
                    "flags": 96,
                    "transformFlags": 0,
                    "start": 94,
                    "end": 96
                },
                "flags": 97,
                "transformFlags": 5120,
                "start": 88,
                "end": 96
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 88,
            "end": 97
        },
        {
            "kind": 120,
            "expression": {
                "kind": 198,
                "left": {
                    "kind": 134299649,
                    "text": "a",
                    "rawText": "a",
                    "flags": 97,
                    "transformFlags": 0,
                    "start": 97,
                    "end": 99
                },
                "operatorToken": {
                    "kind": 34621,
                    "flags": 96,
                    "transformFlags": 16,
                    "start": 99,
                    "end": 103
                },
                "right": {
                    "kind": 134299649,
                    "text": "b",
                    "rawText": "b",
                    "flags": 96,
                    "transformFlags": 0,
                    "start": 103,
                    "end": 105
                },
                "flags": 97,
                "transformFlags": 5120,
                "start": 97,
                "end": 105
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 97,
            "end": 106
        },
        {
            "kind": 120,
            "expression": {
                "kind": 198,
                "left": {
                    "kind": 134299649,
                    "text": "a",
                    "rawText": "a",
                    "flags": 97,
                    "transformFlags": 0,
                    "start": 106,
                    "end": 108
                },
                "operatorToken": {
                    "kind": 34622,
                    "flags": 96,
                    "transformFlags": 16,
                    "start": 108,
                    "end": 111
                },
                "right": {
                    "kind": 134299649,
                    "text": "b",
                    "rawText": "b",
                    "flags": 96,
                    "transformFlags": 0,
                    "start": 111,
                    "end": 113
                },
                "flags": 97,
                "transformFlags": 5120,
                "start": 106,
                "end": 113
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 106,
            "end": 114
        },
        {
            "kind": 120,
            "expression": {
                "kind": 198,
                "left": {
                    "kind": 134299649,
                    "text": "a",
                    "rawText": "a",
                    "flags": 97,
                    "transformFlags": 0,
                    "start": 114,
                    "end": 116
                },
                "operatorToken": {
                    "kind": 34623,
                    "flags": 96,
                    "transformFlags": 16,
                    "start": 116,
                    "end": 119
                },
                "right": {
                    "kind": 134299649,
                    "text": "b",
                    "rawText": "b",
                    "flags": 96,
                    "transformFlags": 0,
                    "start": 119,
                    "end": 121
                },
                "flags": 97,
                "transformFlags": 5120,
                "start": 114,
                "end": 121
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 114,
            "end": 122
        },
        {
            "kind": 120,
            "expression": {
                "kind": 132,
                "expressions": [
                    {
                        "kind": 134299649,
                        "text": "a",
                        "rawText": "a",
                        "flags": 97,
                        "transformFlags": 0,
                        "start": 122,
                        "end": 124
                    },
                    {
                        "kind": 134299649,
                        "text": "b",
                        "rawText": "b",
                        "flags": 96,
                        "transformFlags": 0,
                        "start": 125,
                        "end": 127
                    }
                ],
                "flags": 32,
                "transformFlags": 1024,
                "start": 122,
                "end": 127
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 122,
            "end": 128
        },
        {
            "kind": 120,
            "expression": {
                "kind": 198,
                "left": {
                    "kind": 134299649,
                    "text": "a",
                    "rawText": "a",
                    "flags": 97,
                    "transformFlags": 0,
                    "start": 128,
                    "end": 131
                },
                "operatorToken": {
                    "kind": 99634,
                    "flags": 96,
                    "transformFlags": 0,
                    "start": 131,
                    "end": 133
                },
                "right": {
                    "kind": 198,
                    "left": {
                        "kind": 201392131,
                        "text": "",
                        "rawText": "''",
                        "flags": 4194400,
                        "transformFlags": 0,
                        "start": 133,
                        "end": 136
                    },
                    "operatorToken": {
                        "kind": 34622,
                        "flags": 96,
                        "transformFlags": 16,
                        "start": 136,
                        "end": 139
                    },
                    "right": {
                        "kind": 134299649,
                        "text": "b",
                        "rawText": "b",
                        "flags": 96,
                        "transformFlags": 0,
                        "start": 139,
                        "end": 141
                    },
                    "flags": 4194400,
                    "transformFlags": 5120,
                    "start": 136,
                    "end": 141
                },
                "flags": 97,
                "transformFlags": 5120,
                "start": 128,
                "end": 141
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 128,
            "end": 142
        },
        {
            "kind": 120,
            "expression": {
                "kind": 198,
                "left": {
                    "kind": 198,
                    "left": {
                        "kind": 126,
                        "operandToken": {
                            "kind": 138477613,
                            "flags": 97,
                            "transformFlags": 0,
                            "start": 142,
                            "end": 150
                        },
                        "operand": {
                            "kind": 134299649,
                            "text": "a",
                            "rawText": "a",
                            "flags": 96,
                            "transformFlags": 0,
                            "start": 150,
                            "end": 152
                        },
                        "flags": 32,
                        "transformFlags": 16384,
                        "start": 142,
                        "end": 152
                    },
                    "operatorToken": {
                        "kind": 34622,
                        "flags": 96,
                        "transformFlags": 16,
                        "start": 152,
                        "end": 155
                    },
                    "right": {
                        "kind": 134299649,
                        "text": "b",
                        "rawText": "b",
                        "flags": 96,
                        "transformFlags": 0,
                        "start": 155,
                        "end": 157
                    },
                    "flags": 32,
                    "transformFlags": 5120,
                    "start": 142,
                    "end": 157
                },
                "operatorToken": {
                    "kind": 99634,
                    "flags": 96,
                    "transformFlags": 0,
                    "start": 157,
                    "end": 159
                },
                "right": {
                    "kind": 201392131,
                    "text": "",
                    "rawText": "''",
                    "flags": 4194400,
                    "transformFlags": 0,
                    "start": 159,
                    "end": 162
                },
                "flags": 32,
                "transformFlags": 5120,
                "start": 142,
                "end": 162
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 142,
            "end": 163
        },
        {
            "kind": 120,
            "expression": {
                "kind": 198,
                "left": {
                    "kind": 126,
                    "operandToken": {
                        "kind": 138477613,
                        "flags": 97,
                        "transformFlags": 0,
                        "start": 163,
                        "end": 171
                    },
                    "operand": {
                        "kind": 134299649,
                        "text": "a",
                        "rawText": "a",
                        "flags": 96,
                        "transformFlags": 0,
                        "start": 171,
                        "end": 173
                    },
                    "flags": 32,
                    "transformFlags": 16384,
                    "start": 163,
                    "end": 173
                },
                "operatorToken": {
                    "kind": 34622,
                    "flags": 96,
                    "transformFlags": 16,
                    "start": 173,
                    "end": 176
                },
                "right": {
                    "kind": 201392131,
                    "text": "b",
                    "rawText": "'b'",
                    "flags": 4194400,
                    "transformFlags": 0,
                    "start": 176,
                    "end": 180
                },
                "flags": 32,
                "transformFlags": 5120,
                "start": 163,
                "end": 180
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 163,
            "end": 181
        }
    ],
    "isModule": false,
    "source": "a + b;\na - b;\na * b;\na / b;\na % b;\na ** b;\na & b;\na | b;\na ^ b;\na << b;\na >> b;\na >>> b;\na === b;\na !== b;\na == b;\na != b;\na, b;\n\na + '' == b;\n\ntypeof a == b + '';\n\ntypeof a == 'b';",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 181
}
```

### Printed

```javascript
a + b;
a - b;

a * b;

a / b;

a % b;

a ** b;

a & b;

a | b;

a ^ b;

a << b;

a >> b;

a >>> b;

a === b;

a !== b;

a == b;

a != b;

a, b;

a + "''" == b;

typeof a == b + "''";

typeof a == "'b'";

```

### Diagnostics

```javascript
✔ No errors
```

