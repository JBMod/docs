# Squirrel VScript Reference

JBMod uses the Squirrel scripting language for its VScript system, allowing for powerful server-side and client-side logic without recompiling the engine code.

## Getting Started with Squirrel

Squirrel is a high-level object-oriented programming language, designed to be a light-weight scripting language that fits in the size, memory bandwidth, and real-time requirements of applications like video games.

### Basic Syntax

```squirrel
// This is a comment
local x = 10; // Local variable
global_y <- 20; // Global variable (slot creation)

function Multiply(a, b) {
    return a * b;
}

print(Multiply(x, global_y));
```

## JBMod Bindings

Work in progress.

## Learning Resources

- [Official Squirrel Documentation](http://www.squirrel-lang.org/doc/squirrel3.html)
- [Valve Developer Community: VScript](https://developer.valvesoftware.com/wiki/VScript)
