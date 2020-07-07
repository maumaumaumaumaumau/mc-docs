
# mau-code
---
Made by maumaumaumaumaumau,
mau-code is a 'programming language' made in lua wich has a different but similar syntax to lua & javascript.



# Install
---
## Warning
The interpreter is not open-source yet, you'll have to wait until it is open.


# Documentation
---

mau-code is not complex overall, here is the small documentation talking about the everything.

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

**Example:**
```
function name(arg1,arg2){

}
```

### return

Returns a value and finishes evaluation either on a function call or the main code.
Arguments:
```
variant
```

**Example:**
```
function a(b,c){
return b+c # Use of return
}
print(a(1,2)) # 3
```

### dog, null

Not much of a keyword but a non existant value. Attempting to set it will result in an error.

**Example**
```
a = "b"
print(a) # b
a = null
a = dog
print(a) # null
```

### if

Used for statements, runs code if the given condition is true.
Arguments:
```
variant (condition)
```

**Example**

```
if 1 < 2 { # valid
print("1 is less than 2")
}

if 1 < 2 then # valid too, but will only execute first instruction. example on next line
print("1 is less than 2")

if 1 > 2 then print("1 is higher than 2, but how?") print("i was called after!") 
# "i was called after!"
```
#### else
Runs code if given condition wasn't true on if

**Example**
```
if 1 > 2 {
print("1 is higher than 2, but how?")
} else {
print("1 is less than 2, logically.")
}
#" 1 is less than 2, logically."
```


---

### true, false

Represents a boolean being true or false.

---

## Global functions
---
mau-code has 8 primitive functions that are built-in, this section has all of these.

### print

Logs given arguments to the console.
Arguments:

```
tuple (multiple arguments)
```

### type

Returns the datatype of the given obect.
Arguments:

```
variant (1 argument)
```

### concatfunc

Returns a string containing the source of a function (by abstract syntax tree). (may not be completely accurate)
Arguments:

```
function (1 argument)
```

### error

Errors to the console & stops code execution.
Arguments:

```
string (1 argument)
```

### fac

Returns the factorial of the given number.
Arguments:
```
number (1 argument)
```
### sin

Returns the sine of the given number.
Arguments:
```
number (1 argument)
```

### cos

Returns the cosine of an angle.
Arguments:
```
number (1 argument)
```

### time

Returns how many seconds have passed since the unix epoch.
This function requires no arguments.


---
