# The 2026-2028 Rust Developer Roadmap

**Goal:** Entry-level Rust Developer by 2028 graduation.
**Pace:** Maximum 2 hours per day. Consistency over intensity.

## The Universal Weekly Routine

Use this template every week. Because you are spending up to 2 hours a day typing code on top of your regular university work and any gaming, **make sure to incorporate short stretch breaks every 45 minutes to protect your wrists from fatigue and repetitive strain.**

| Day | Focus | Activity | Duration |
| :--- | :--- | :--- | :--- |
| **Monday** | **Theory & Core Concepts** | Read documentation, "The Rust Book," or watch technical deep-dives. | 1.5 - 2 Hours |
| **Tuesday** | **Targeted Practice** | Exercises based on Monday's theory (Rustlings, Leetcode, small scripts). | 1.5 - 2 Hours |
| **Wednesday** | **Theory & Core Concepts** | Continue reading documentation or learning new syntax for the week. | 1.5 - 2 Hours |
| **Thursday** | **Targeted Practice** | Write isolated scripts to test concepts. Break the compiler on purpose. | 1.5 - 2 Hours |
| **Friday** | **Project Building** | Apply knowledge to a larger project. No tutorials—just building. | 2 Hours |
| **Saturday** | **Refactor & Review** | Clean up code, run `cargo clippy`, fix warnings, and review struggles. | 1 Hour |
| **Sunday** | **Rest** | Step away from the keyboard entirely. | **0 Hours** |

---

## Phase 1: Core Fundamentals & The Borrow Checker (Months 1-4)
*Focus: Mastering memory, basic syntax, and error handling.*

### Month 1: The Basics & Syntax
| Week | Focus Area | The Rust Book | Rustlings |
| :--- | :--- | :--- | :--- |
| **Week 1** | Installation, Tooling, & Hello World | Chapter 1 | `intro` |
| **Week 2** | First Mini-Project: Guessing Game | Chapter 2 | None |
| **Week 3** | Variables, Mutability, & Data Types | Chapter 3 (3.1-3.2) | `variables`, `primitive_types` |
| **Week 4** | Functions & Control Flow (`if`, `loop`) | Chapter 3 (3.3-3.5) | `functions`, `if` |

### Month 2: The Mental Model Shift (Crucial)
| Week | Focus Area | The Rust Book | Rustlings |
| :--- | :--- | :--- | :--- |
| **Week 5** | The Stack, The Heap, & Ownership Rules | Chapter 4 (4.1) | `move_semantics` (1-3) |
| **Week 6** | References & Borrowing | Chapter 4 (4.2) | `move_semantics` (4-6) |
| **Week 7** | The Slice Type | Chapter 4 (4.3) | Re-do `move_semantics` |
| **Week 8** | Deep Review & Intentional Breakage | Review Ch 4 | Break the compiler intentionally |

### Month 3: Structuring Your Data
| Week | Focus Area | The Rust Book | Rustlings |
| :--- | :--- | :--- | :--- |
| **Week 9** | Defining and Instantiating Structs | Chapter 5 (5.1-5.2)| `structs` |
| **Week 10** | Method Syntax (`impl` blocks) | Chapter 5 (5.3) | Geometry script |
| **Week 11** | Enums & The `Option` Enum | Chapter 6 (6.1) | `enums` |
| **Week 12** | Pattern Matching (`match` & `if let`) | Chapter 6 (6.2-6.3)| Combine `enums` & `structs` |

### Month 4: Collections, Errors, & Phase 1 Capstone
| Week | Focus Area | The Rust Book | Rustlings |
| :--- | :--- | :--- | :--- |
| **Week 13** | Vectors & Strings (Heap-allocated data)| Chapter 8 (8.1-8.2)| `vecs`, `strings` |
| **Week 14** | Hash Maps | Chapter 8 (8.3) | `hashmaps` |
| **Week 15** | Error Handling (`Result`, `panic!`, `?`)| Chapter 9 | `options`, `error_handling` |
| **Week 16** | **Phase 1 Capstone Project** | Review all | Terminal-based To-Do List |

---

## Phase 2: Intermediate Concepts & Tooling (Months 5-8)
*Focus: Idiomatic Rust, multi-file projects, and advanced types.*

### Month 5: Modules and Generics
* **Weeks 17-18:** Managing Growing Projects with Packages, Crates, and Modules (Chapter 7). `rustlings: modules`
* **Weeks 19-20:** Generic Data Types and extracting functions (Chapter 10.1). `rustlings: generics`

### Month 6: Traits and Lifetimes
* **Weeks 21-22:** Traits - Defining Shared Behavior (Chapter 10.2). `rustlings: traits`
* **Weeks 23-24:** Validating References with Lifetimes (Chapter 10.3). *Spend extra time here.* `rustlings: lifetimes`

### Month 7: Functional Features
* **Weeks 25-26:** Closures - Anonymous Functions that Capture their Environment (Chapter 13.1).
* **Weeks 27-28:** Processing a Series of Items with Iterators (Chapter 13.2). `rustlings: iterators`

### Month 8: Smart Pointers & Phase 2 Capstone
* **Weeks 29-30:** Smart Pointers (`Box<T>`, `Rc<T>`, `RefCell<T>`) (Chapter 15). `rustlings: smart_pointers`
* **Weeks 31-32:** **Phase 2 Capstone Project.** Build a custom, multi-file CLI tool (like a fast `grep` or directory crawler) using the `clap` crate.

---

## Phase 3: The Async Ecosystem & Backend (Months 9-15)
*Focus: Asynchronous programming, APIs, and databases. (Moving away from The Book, focusing on external documentation).*

### Months 9-10: Async Foundations
* **Weeks 33-36:** Understand `Future` trait, `async`/`await` syntax. Read the "Asynchronous Programming in Rust" online book.
* **Weeks 37-40:** Master the `tokio` runtime. Spawning tasks, async I/O, channels (`mpsc`).

### Months 11-12: Serialization & Web Frameworks
* **Weeks 41-44:** Learn `serde` and `serde_json` for data serialization.
* **Weeks 45-48:** Pick a web framework (`axum` recommended). Learn routing, extractors, and middleware. Build simple "Hello World" endpoints.

### Months 13-14: Databases & State Management
* **Weeks 49-52:** Learn `sqlx`. Write compile-time checked SQL queries against a PostgreSQL database.
* **Weeks 53-56:** Manage application state (sharing database pools across async web routes using `Arc`).

### Month 15: Phase 3 Capstone
* **Weeks 57-60:** **Phase 3 Capstone Project.** Build a robust Concurrent REST API (e.g., a blogging engine backend) with user authentication, CRUD operations, and PostgreSQL integration.

---

## Phase 4: Niche Skills & Infrastructure (Months 16-19)
*Focus: Expanding beyond the backend, deployment, and performance.*

### Month 16: WebAssembly (WASM)
* **Weeks 61-64:** Use `wasm-bindgen` to compile Rust for the browser. Build a small front-end counter or calculator powered by Rust logic.

### Month 17: Containerization
* **Weeks 65-68:** Write Dockerfiles for Rust. Learn multi-stage builds to compile in one container and run the binary in a tiny `scratch` or `alpine` container.

### Month 18: CI/CD Pipelines
* **Weeks 69-72:** Set up GitHub Actions. Automate `cargo test`, `cargo fmt`, and `cargo clippy` to run on every commit.

### Month 19: Phase 4 Capstone
* **Weeks 73-76:** **Phase 4 Capstone Project.** Build a Browser & Cloud Deployment project. A WASM-powered web tool, fully containerized and automatically tested via GitHub Actions.

---

## Phase 5: The Capstone & Open Source (Months 20-24)
*Focus: Building a resume-worthy portfolio and industry readiness.*

### Months 20-21: Open Source Contributions
* **Weeks 77-84:** Find "good first issues" on GitHub. Contribute documentation fixes, minor bug fixes, or tests to crates you've used (like `axum`, `clap`, or `tokio`).

### Months 22-24: The Final Distributed Capstone
* **Weeks 85-104:** Dedicate these final three months to your massive portfolio piece. Architect a complex system from scratch.
* **Project Ideas:** * A distributed Key-Value store.
    * A real-time WebSocket chat server handling thousands of concurrent connections.
    * A custom network protocol parser.