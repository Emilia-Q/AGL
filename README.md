AGL (A good language) is my first attempt at fully implementing a language, I alreayd have most of the design laid out. It will be implemented using LLVM and C/C++

The goal of this language is to have a superset of C like C++ etc, but one that is still easily knowable. With modern syntax, and features to maximize readablity and ease of use. Its syntax largely takes inspiration from Kotlin, Swift, Python, C, C++, and Rust.

The end goal is to also make a dependancy management/build tool inspired by cargo which will work with both C and AGL.

How AGL works
```
// Types:
int.8,  int.u8
int.16, int.u16
int.32, int.u32
int.64, int.u64
int/int.ap

float.16, float.u16
float.32, float.u32
float.64, float.u64
float/float.ap

string
string.char

boolean

// Variables:
var name: type = value
val name: type = value
dynamic name:= value

array[length] name: type = {}
vector[height, width] name: type = {}
list name:= {}
map name: type, type = {}
tuple name: type, type = {}

// Data Structures:
stack name: type
queue name: type
pqueue name: type, type
pstack name: type, type
graph name: type, type
set name: {}

// Functions:
func name() -> type {
    return value
}

sub name {
    reutrn _[1]
}

// Loops:

func loop_example() -> void {
    while(condition) {
        //body
    }
    for(def; condition; action) {
        //body
    }
    for(enumerable_value) {
        //body
    }
}

// Conditionals:
func consitional_examples() -> void {
    if(condition) {
    } elif(conditoin) {
    } else { }

    when(value) {
        is(0) {}
        is(1) {}
        else {}
    }
}
```
