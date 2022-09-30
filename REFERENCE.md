## Hello World

```rust
func main() {
    print("Hello, world!");
}
```

## Variables and Mutability

```rust
func main() {
    x: num = 5;
    print(x);       // prints `5`
    x: num = 6;     // ImmutabilityError!
    print(x);       // program won't compile this far
}
```

## Mutable variables

```rust
func main() {
    x: mut num = 5;
    print(x);  // prints `5`
    x = 6;     // no error!
    print(x);  // prints `6`
}
```

## Data Types

```rust
func main() {
    a: num = 5;  // defaults to signed num32
    b: unsigned num8 = 5;
    c: unsigned num16 = 5;
    d: unsigned num32 = 5;
    e: unsigned num64 = 5;
    f: unsigned num128 = 5;
    g: signed num = -5;
    h: signed num8 = -5;
    i: signed num16 = -5;
    j: signed num32 = -5;
    k: signed num64 = -5;
    l: signed num128 = -5;

    // If data ends up exceeding the limits of it's
    // data type, an OverflowError will be raised

    s: float = 5.0;  // defaults to 64 bit float
    t: float32 = 5.0; // 32 bit float

    y: bool = true;
    z: str = "Hello, world!";
}
```

## Numeric Operations

```rust
func main() {
    // Arithmetic
    a: num = 5 + 5;  // addition
    b: num = 5 - 5;  // subtraction
    c: num = 5 * 5;  // multiplication
    d: num = 5 / 5;  // division
    e: num = 5 % 5;  // modulus
    f: num = 5 ** 5; // exponentiation

    // Bitwise
    g: num = 5 & 5;  // bitwise AND
    h: num = 5 | 5;  // bitwise OR
    i: num = 5 ^ 5;  // bitwise XOR
    j: num = ~5;     // bitwise NOT
    j: num = 5 << 5; // left shift
    k: num = 5 >> 5; // right shift

}