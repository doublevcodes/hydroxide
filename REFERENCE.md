# Reference

## Hello World

```rust
func main() {
    print("Hello, world!");
}
```

## Variables and Mutability

### Immutability by default

```rust
func main() {
    x: num = 5;
    print(x);       // prints `5`
    x: num = 6;     // ImmutabilityError!
    print(x);       // program won't compile this far
}
```

### Mutable variables

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
    a: num = 5;
    b: float = 5.0; 
    c: bool = true;
    d: str = "Hello, world!";
}
```

### Numeric operations

```rust
func main() {
    a: num = 5 + 5;  // addition
    b: num = 5 - 5;  // subtraction
    c: num = 5 * 5;  // multiplication
    d: num = 5 / 5;  // division
    e: num = 5 % 5;  // modulus
}
```

## Compound types

```rust
func main() {
    a: (num, num, str) = (3, 6, "Lithium");
    b: [5: num * 3];  // [5, 5, 5]
    c: mut [num] = [1, 2, 3, 4]
}