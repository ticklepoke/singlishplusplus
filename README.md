# Singlish++

The official language spec for the singlish++ language. Inspired by everyday Singaporean phrases.

## Line Termination

Rather than using semicolons, singlish++ uses the quintessential Singlish phrase ` la`:

```
1+1 la
```

## Variable Declarations

```
CHOPE x = 1 la
```

## Functions

Functions are prefixed with `SAIKANG`.

Return statements are prefixed with `GIVE_YOU_BACK`.

```
SAIKANG addTwoNumbers(x, y) {
    GIVE_YOU_BACK x + y la
}
```

## Import Statements

Functions, variables and classes can be imported from other files using `STENG`.

```
STENG { add } from "./math.spp"
```

## Control Flow

### If - Else

```
SEKALI (x == 1) {
    // do something when x equals 1
} NEHMIND {
    // do something if x doesnt equal 1
}
```

### Loops

```
CHIONG (CHOPE x = 1; x < 10; x++) {
    SEKALI (x == 5) {
        PANGKANG la
    }
}
```

## Exception Handling

### Throwing Errors

```
JIBAI(errorMessage) la
```

### Try - Catch

```
TAHAN {
    JIBAI("Array out of bounds!") la
} DIE_LIAO(error) {
    // Do something with the error
}
```

## Std Lib

Some functions in the std lib.

### Logging

Print to stdout using `BAO_TOH`

```
BAO_TOH("Some message") la
```

### Input

To read from stdin, use `SIMI_SAI`

```
CHOPE x = SIMI_SAI() la
```

### Pseudo Random Number

Get a random integer between two ranges

```
YAYA_PAPAYA(0, 10) la
```

### Assertions

```
POFMA(1+1, 2) la // true

POFMA("abc", "bcd") la // false
```
