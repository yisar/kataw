# Kataw parser test case

## Input

`````js
.0
;
.1
;
.2
;
.3
;
.4
;
.5
;
.6
;
.7
;
.8
;
.9
;
.10
;
.21
;
.32
;
.43
;
.54
;
.65
;
.76
;
.87
;
.98
;
.19
;
.123
;
.456
;
.7890
;
.1234567890
;
.0000
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
                "kind": 201392130,
                "text": 0,
                "rawText": ".0",
                "flags": 96,
                "transformFlags": 0,
                "start": 0,
                "end": 2
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 0,
            "end": 4
        },
        {
            "kind": 120,
            "expression": {
                "kind": 201392130,
                "text": 0.1,
                "rawText": ".1",
                "flags": 97,
                "transformFlags": 0,
                "start": 4,
                "end": 7
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 4,
            "end": 9
        },
        {
            "kind": 120,
            "expression": {
                "kind": 201392130,
                "text": 0.2,
                "rawText": ".2",
                "flags": 97,
                "transformFlags": 0,
                "start": 9,
                "end": 12
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 9,
            "end": 14
        },
        {
            "kind": 120,
            "expression": {
                "kind": 201392130,
                "text": 0.3,
                "rawText": ".3",
                "flags": 97,
                "transformFlags": 0,
                "start": 14,
                "end": 17
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 14,
            "end": 19
        },
        {
            "kind": 120,
            "expression": {
                "kind": 201392130,
                "text": 0.4,
                "rawText": ".4",
                "flags": 97,
                "transformFlags": 0,
                "start": 19,
                "end": 22
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 19,
            "end": 24
        },
        {
            "kind": 120,
            "expression": {
                "kind": 201392130,
                "text": 0.5,
                "rawText": ".5",
                "flags": 97,
                "transformFlags": 0,
                "start": 24,
                "end": 27
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 24,
            "end": 29
        },
        {
            "kind": 120,
            "expression": {
                "kind": 201392130,
                "text": 0.6,
                "rawText": ".6",
                "flags": 97,
                "transformFlags": 0,
                "start": 29,
                "end": 32
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 29,
            "end": 34
        },
        {
            "kind": 120,
            "expression": {
                "kind": 201392130,
                "text": 0.7,
                "rawText": ".7",
                "flags": 97,
                "transformFlags": 0,
                "start": 34,
                "end": 37
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 34,
            "end": 39
        },
        {
            "kind": 120,
            "expression": {
                "kind": 201392130,
                "text": 0.8,
                "rawText": ".8",
                "flags": 97,
                "transformFlags": 0,
                "start": 39,
                "end": 42
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 39,
            "end": 44
        },
        {
            "kind": 120,
            "expression": {
                "kind": 201392130,
                "text": 0.9,
                "rawText": ".9",
                "flags": 97,
                "transformFlags": 0,
                "start": 44,
                "end": 47
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 44,
            "end": 49
        },
        {
            "kind": 120,
            "expression": {
                "kind": 201392130,
                "text": 0.1,
                "rawText": ".10",
                "flags": 97,
                "transformFlags": 0,
                "start": 49,
                "end": 53
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 49,
            "end": 55
        },
        {
            "kind": 120,
            "expression": {
                "kind": 201392130,
                "text": 0.21,
                "rawText": ".21",
                "flags": 97,
                "transformFlags": 0,
                "start": 55,
                "end": 59
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 55,
            "end": 61
        },
        {
            "kind": 120,
            "expression": {
                "kind": 201392130,
                "text": 0.32,
                "rawText": ".32",
                "flags": 97,
                "transformFlags": 0,
                "start": 61,
                "end": 65
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 61,
            "end": 67
        },
        {
            "kind": 120,
            "expression": {
                "kind": 201392130,
                "text": 0.43,
                "rawText": ".43",
                "flags": 97,
                "transformFlags": 0,
                "start": 67,
                "end": 71
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 67,
            "end": 73
        },
        {
            "kind": 120,
            "expression": {
                "kind": 201392130,
                "text": 0.54,
                "rawText": ".54",
                "flags": 97,
                "transformFlags": 0,
                "start": 73,
                "end": 77
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 73,
            "end": 79
        },
        {
            "kind": 120,
            "expression": {
                "kind": 201392130,
                "text": 0.65,
                "rawText": ".65",
                "flags": 97,
                "transformFlags": 0,
                "start": 79,
                "end": 83
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 79,
            "end": 85
        },
        {
            "kind": 120,
            "expression": {
                "kind": 201392130,
                "text": 0.76,
                "rawText": ".76",
                "flags": 97,
                "transformFlags": 0,
                "start": 85,
                "end": 89
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 85,
            "end": 91
        },
        {
            "kind": 120,
            "expression": {
                "kind": 201392130,
                "text": 0.87,
                "rawText": ".87",
                "flags": 97,
                "transformFlags": 0,
                "start": 91,
                "end": 95
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 91,
            "end": 97
        },
        {
            "kind": 120,
            "expression": {
                "kind": 201392130,
                "text": 0.98,
                "rawText": ".98",
                "flags": 97,
                "transformFlags": 0,
                "start": 97,
                "end": 101
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 97,
            "end": 103
        },
        {
            "kind": 120,
            "expression": {
                "kind": 201392130,
                "text": 0.19,
                "rawText": ".19",
                "flags": 97,
                "transformFlags": 0,
                "start": 103,
                "end": 107
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 103,
            "end": 109
        },
        {
            "kind": 120,
            "expression": {
                "kind": 201392130,
                "text": 0.123,
                "rawText": ".123",
                "flags": 97,
                "transformFlags": 0,
                "start": 109,
                "end": 114
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 109,
            "end": 116
        },
        {
            "kind": 120,
            "expression": {
                "kind": 201392130,
                "text": 0.456,
                "rawText": ".456",
                "flags": 97,
                "transformFlags": 0,
                "start": 116,
                "end": 121
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 116,
            "end": 123
        },
        {
            "kind": 120,
            "expression": {
                "kind": 201392130,
                "text": 0.789,
                "rawText": ".7890",
                "flags": 97,
                "transformFlags": 0,
                "start": 123,
                "end": 129
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 123,
            "end": 131
        },
        {
            "kind": 120,
            "expression": {
                "kind": 201392130,
                "text": 0.123456789,
                "rawText": ".1234567890",
                "flags": 97,
                "transformFlags": 0,
                "start": 131,
                "end": 143
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 131,
            "end": 145
        },
        {
            "kind": 120,
            "expression": {
                "kind": 201392130,
                "text": 0,
                "rawText": ".0000",
                "flags": 97,
                "transformFlags": 0,
                "start": 145,
                "end": 151
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 145,
            "end": 151
        }
    ],
    "isModule": false,
    "source": ".0\n;\n.1\n;\n.2\n;\n.3\n;\n.4\n;\n.5\n;\n.6\n;\n.7\n;\n.8\n;\n.9\n;\n.10\n;\n.21\n;\n.32\n;\n.43\n;\n.54\n;\n.65\n;\n.76\n;\n.87\n;\n.98\n;\n.19\n;\n.123\n;\n.456\n;\n.7890\n;\n.1234567890\n;\n.0000",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 151
}
```

### Printed

```javascript
0.0;
0.1;

0.2;

0.3;

0.4;

0.5;

0.6;

0.7;

0.8;

0.9;

0.1;

0.21;

0.32;

0.43;

0.54;

0.65;

0.76;

0.87;

0.98;

0.19;

0.123;

0.456;

0.789;

0.123456789;

0.0;

```

### Diagnostics

```javascript
✔ No errors
```

