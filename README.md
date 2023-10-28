## Vectors

***Definition*** - In simple terms, vectors in Rust are like **dynamic lists** that can hold **multiple pieces of data**. They allow you to store and manage a collection of items, and you can **add** or **remove** elements as needed. Vectors are flexible and **can grow** or **shrink** in size as you use them. They're a handy tool for working with a variable number of items in your programs.

```rust
fn main() -> () {
   let shows = ["Violet Evergarden", "Tengoku no Daimakyou", "Kokoro Connect"];
    
    // .iter() -> Prevents 'shows''s ownership from being moved to the for..loop
    // This will allow 'shows' to be accessible outside the for..loop
    // .enumerate() -> Allows us to access/preview the index
    
    for (index, s) in shows.into_iter().enumerate() {
        if index == 1 {
            println!("Output: {} {:?}", index, s);      
        }
    }
}
```
