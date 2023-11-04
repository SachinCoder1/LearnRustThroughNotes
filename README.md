# Rust Notes with Interview Questions
This repository serves as a personal knowledge base, documenting the journey from beginner to advanced Rustacean, and is intended as a quick reference guide for Rust concepts. This Repo Also Contains Potential **Interview Questions** 

## Basics of Rust
Basics of rust contains topics like variables, rust definition, syntax, etc.

### 1. What is Rust?
Rust is a relatively new programming language which had its 1.0 release in 2015:

   1. Rust is a statically compiled language in a similar role as C++
   2. Rust Compiler uses LLVM as its backend.
   3. Rust supports many platforms and architectures like:
        - x86, ARM, WebAssembly, etc
        - Linux, Mac, Windows, etc

### 2. Rust Important Points to Remember:
   - Functions are introduced with fn.
   - Blocks are delimited by curly braces like in C and C++.
   - The main function is the entry point of the program.
   - Rust has hygienic macros, println! is an example of this.
   - Rust strings are UTF-8 encoded and can contain any Unicode character.

### 3. In What Devices Rust can be Used? 
Rust is used for a wide range of devices:
   - firmware and boot loaders,
   - smart displays,
   - mobile phones,
   - desktops,
   - servers.

### 4. What is rustc?
**rustc**: the Rust compiler which turns .rs files into binaries and other intermediate formats.
  > rustc uses LLVM as its backend

### 5. Why Use Rust?
   - Compile time memory safety.
      -  No uninitialized variables.
      - No memory leaks (mostly, see notes).
      - No double-frees.
      - No use-after-free.
      - No NULL pointers.
      - No forgotten locked mutexes.
      - No data races between threads.
      - No iterator invalidation.

   - No undefined behavior at runtime.
      - Array access is bounds checked.
      - Integer overflow is defined (panic or wrap-around).

   - Modern language features.
     Rust is built with all the experience gained in the last decades.
      - Enums and pattern matching.
      - Generics.
      - No overhead FFI.
      - Zero-cost abstractions.
    

### Scalar Types

|                        	|              Types             	|       Literals         	|
|:----------------------:	|:------------------------------:	|------------------------	|
| Signed integers        	| i8, i16, i32, i64, i128, isize 	| -10, 0, 1_000, 123_i64 	|
| Unsigned integers      	| u8, u16, u32, u64, u128, usize 	| 0, 123, 10_u16         	|
| Floating point numbers 	| f32, f64                       	| 3.14, -10.0e20, 2_f32  	|
| Strings                	| &str                           	| "foo", "two\nlines"    	|
| Unicode scalar values  	| char                           	| 'a', 'α', '∞'          	|
| Booleans               	| bool                           	| true, false            	|

