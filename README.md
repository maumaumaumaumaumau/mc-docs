
# mau-code
---
Made by maumaumaumaumaumau,
mau-code is a 'programming language' made in lua wich has a different but similar syntax to lua & javascript.



# Install
---
## Warning
The interpreter is not open-source yet, you'll have to wait until it is open.


# Getting started
---

mau-code is not complex overall, here is a small documentation talking about the basics.

## Global Environment
---

Unlike old mau-code, the new version has a global environment wich holds variables and functions defined by the user and defined by the system.

### Upvalues

mau-code has upvalues wich are variables defined on the main environment or the last environment in wich a function was made. Editing those will also affect the environment overwriting the original values.


---

## Syntax

---
As said above, the syntax will be similar to lua and js. Function enclosements are with {}, if statements don't require () unlike javascript.
Two examples of the syntax are here.

```
# Hello world program.
print("Hello World!")
```
---
```
# Functions with return.
a = function(b,c){ # valid
return b+c
} 
function d(e,f){ # valid too 
return e+f
}
print(a(1,2)) # 3
print(d(1,2)) # 3
```

---

## Keywords
---
mau-code has some keywords for  statements & functions, those are:

### function

Defines a function on the environment.
Arguments:
```
name (optional)
arguments (optional)
```

### return

Returns a value or results of a function call.
Arguments:
```
variant
```

---
