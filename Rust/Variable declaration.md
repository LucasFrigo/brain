#rust
#programming

`let` introduces a variable.
```rust
let x;
x = 42;

// OR

let x = 42;
```

You can specify the variable type explicitly with a `:` , that's a type annotation
```rust
let x: i32; // signed 32-bit integer
x = 42;
// OR
let x: i32 = 42;
```


The underscore `_` is a special name - or rather, a "lack of name". It basically means to throw away something:

```rust
// this does *nothing* because 42 is a constant_
let _ = 42;

// this calls `get_thing` but throws away its result_
let _ = get_thing();
````

Names that _start_ with an underscore are regular names, it's just that the compiler won't warn about them being unused:
```rust
// we may use `_x` eventually, but our code is a work-in-progress_
// and we just wanted to get rid of a compiler warning for now._
let _x = 42;
```

Separate bindings with the same name can be introduced - you can _shadow_ a variable binding:
```rust
let x = 13;
let x = x + 3;
// using `x` after that line only refers to the second `x`,
// the first `x` no longer exists.
```

