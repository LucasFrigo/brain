#rust
#programming


`fn` declares a function.

Here's a void function:

```rust
fn greet() {
	println!("Hello world!");
}
```

And here's a function that returns a 32-bit signed integer. The arrow indicates its return type:

```rust
fn fair_dice_roll() -> i32 {
	4
}
```

Code blocks `{}` are also expressions, which means they evaluate to a value. For instance:
```rust
let x = 42;
// is equal to 
let x = { 42 };
```

Inside a block you can have multiple statements, and the last one is called the `tail` , where if you omit the semicolon it will treat as the same as returning:

```rust
let x = {
	let y = 1;
	let z = 2;
	y + z // this is the same as returning y+z, since the ; is omitted
}
```

```rust
fn dice_roll() -> i32 {
	return 4;
}
// is the same as
fn dice_roll() -> i32 {
	4
}
```

