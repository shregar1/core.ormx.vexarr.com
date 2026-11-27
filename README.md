# ORMX Core 🦀

[![Language: Rust](https://img.shields.io/badge/Language-Rust-orange.svg)](https://www.rust-lang.org/)
[![License: MIT / Apache-2.0](https://img.shields.io/badge/License-MIT_|_Apache_2.0-blue.svg)](LICENSE)

**ORMX Core** is a lightweight, zero-allocation database engine and migration framework built in Rust. It serves as the foundational core powering the entire polyglot ORMX ecosystem (Node.js, Python, Rust, Java).

---

## ⚡ Highlights

* **Zero-Allocation Query Compilation:** Pre-compiles SQL ASTs into parameterized native queries without heap reallocations.
* **Automated Migration Discovery:** Topologically sorts SQL migration scripts, diffs target DDL against actual live schema, and executes atomic rollback transactions.
* **Cross-Language FFI:** Exposes C-compatible dynamic interfaces for high-level language bindings (Node.js via N-API, Python via PyO3, Java via JNI).
* **High-Throughput Benchmarks:** In production benchmarks, `ormx-node` outperforms Prisma by **4.1x on SELECT queries** and ties raw `postgres.js`.

---

## 🚀 Usage

Add to your `Cargo.toml`:
```toml
[dependencies]
ormx-core = { git = "https://github.com/shregar1/core.ormx.vexarr.com.git" }
```

---

## 📜 License
Licensed under MIT or Apache-2.0.
