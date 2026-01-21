# 🔐 Simple Encryptor Challenge - Rust 

This project is a solution to a simple encryptor challenge using **Rust**.  
It demonstrates reading a binary file, extracting a seed, and processing the remaining encrypted data.


## 📂 Project Structure

simple_encryptor/
├── src/
│   ├── main.rs        ← Rust code
│   └── rng.c          ← C file for srand(), rand()
├── Cargo.toml         ← Rust project manifest
├── build.rs           ← Compile rng.c
├── flag.enc           ← Encrypted flag
└── encrypt            ← optional


## ⚡ Features > ⚠️ Spoiler alert: don't read the code until you try decrypting yourself!

- Reads the first 4 bytes as a **little-endian seed**
- Reads the rest of the encrypted file safely
- Written in **idiomatic Rust**
- Handles errors properly


## 🛠️ How to Run

1. Make sure Rust is installed: [https://www.rust-lang.org/tools/install](https://www.rust-lang.org/tools/install)
2. Make sure you have a C compiler installed (gcc/clang) to build rng.c
3. Put your encrypted file `flag.enc` in the project root
4. Run:
```bash
    cargo run
```
5. You should see : 
    HTB{-------}


## 👨‍💻 Author

MOSSAAB ;)
