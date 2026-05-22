# AppOf Language Specification v1.0

## Overview
**AppOf** is a simple, device-agnostic programming language designed for fast learning and easy interpretation across all platforms.

## Core Syntax

### 1. Variables
```
SET variableName TO value
SET counter TO 0
SET message TO "Hello"
SET pi TO 3.14
```

### 2. Output
```
PRINT "text here"
PRINT variableName
```

### 3. Input
```
INPUT variableName
```

### 4. Math Operations
```
MATH result = x + y
MATH area = length * width
MATH doubled = number * 2
```

### 5. Arithmetic
```
ADD number TO variable
SET counter TO counter + 1
SUBTRACT 5 FROM variable
MULTIPLY variable BY 2
DIVIDE variable BY 3
```

### 6. Conditionals
```
IF condition THEN
    PRINT "condition is true"
END

IF x EQUALS 5 THEN
    PRINT "x is 5"
ELSE
    PRINT "x is not 5"
END
```

### 7. Comparisons
```
x EQUALS 5
x GREATER_THAN 10
x LESS_THAN 20
x GREATER_OR_EQUAL 15
x LESS_OR_EQUAL 8
x NOT_EQUALS 0
```

### 8. Logic
```
AND condition1 condition2
OR condition1 condition2
NOT condition
```

### 9. Loops
```
LOOP 5 TIMES DO
    PRINT "repeating"
END

WHILE x LESS_THAN 10 DO
    ADD 1 TO x
    PRINT x
END
```

### 10. Functions
```
FUNCTION greet
    PRINT "Hello!"
END

CALL greet

FUNCTION add x y
    SET result TO x + y
    RETURN result
END
```

### 11. Arrays
```
SET array TO [1, 2, 3, 4, 5]
SET item TO array[0]
APPEND value TO array
```

### 12. Comments
```
// This is a comment
// Code explanation here
```

## Example Programs

### Hello World
```appof
PRINT "Hello, World!"
```

### Counter
```appof
SET counter TO 0
LOOP 5 TIMES DO
    ADD 1 TO counter
    PRINT counter
END
```

### Grade Calculator
```appof
INPUT score
IF score GREATER_OR_EQUAL 90 THEN
    PRINT "Grade: A"
ELSE
    IF score GREATER_OR_EQUAL 80 THEN
        PRINT "Grade: B"
    ELSE
        PRINT "Grade: C"
    END
END
```

## Interpreter Requirements

All AppOf interpreters must support:
- ✅ Variable storage and retrieval
- ✅ Basic arithmetic operations
- ✅ String handling
- ✅ Conditional logic (IF/ELSE)
- ✅ Loop structures (LOOP/WHILE)
- ✅ Function definitions and calls
- ✅ Console I/O (PRINT/INPUT)

## File Extension
- `.appof` - AppOf source code files

## Design Philosophy
- **Simplicity** - Easy syntax anyone can learn
- **Clarity** - Code reads like English
- **Portability** - Same code runs everywhere
- **Accessibility** - Works on any device

## Universal Interpreter Checklist
For any language to support AppOf, implement:

1. Lexer (tokenizer)
2. Parser (syntax reader)
3. Variable storage (dictionary/map)
4. Expression evaluator
5. Statement executor
6. Input/Output handler

---
**Version**: 1.0  
**Created**: 2026-05-22  
**Status**: Active Development