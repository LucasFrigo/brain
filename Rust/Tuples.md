#rust
#programming 

Rust has tuples, which you can think of as "fixed-length collections of values of different types".
You can access tuples values by `TUPLE.INDEX` :
```rust
let pair = ('a', 17);
pair.0; // this is 'a'
pair.1; // this is 17
```

You can also annotate the type of a tuple like this:
```rust
let pair: (char, i32l) = ('a', 17);
```

Tuples can be _destructured_ when doing an assignment, which means they're broken down into their individual fields:
```rust
let (some_char, some_int) = ('a', 17);
// now some_char ias 'a' and 'some_int' is 17
```