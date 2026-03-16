# 06 - Software Basics

Software is the set of instructions that tells hardware what to do. At the lowest level, all software is just a series of numbers represented in binary.

---

## 🔢 Data Representation & Encoding
Computers only understand two states: **on** (1) and **off** (0). Every piece of data—from a photo to a text message—is stored using these bits.

### Number Systems
* **Binary (Base-2)**: The fundamental language of computers (0-1).
* **Hexadecimal (Base-16)**: Groups 4 bits into one digit (0-9, A-F). Used for memory addresses and color codes.
* **Octal (Base-8)**: Groups 3 bits into one digit (0-7). Commonly used for Linux file permissions.

### Character Encoding
Encoding is the agreed-upon mapping between numbers and characters.
* **ASCII**: Early 7-bit standard for English characters (0-127).
* **Unicode**: The universal standard that assigns a unique "code point" to every character in every language, including emojis.
* **UTF-8**: The most common web encoding; it is variable-length (1-4 bytes) and backward compatible with ASCII.

---

## 🎨 Digital Colors (RGB Model)
Colors are represented by combining different intensities of Red, Green, and Blue. 
* **24-bit Color**: Each color (R, G, B) is assigned 1 byte (8 bits), allowing for 256 levels of intensity per color.
* **Total Combinations**: $256 \times 256 \times 256$ = 16.7 million colors.



---

## 💻 The Three Pillars of Programming
Whether you are using Python or JavaScript, almost all imperative programming relies on three core concepts:

1.  **Variables**: Named storage for data that can change (e.g., `let score = 0`).
2.  **Conditionals**: Decision-making logic (`if`, `else if`, `else`).
3.  **Loops**: Repeating a block of code as long as a condition is true (`while`, `for`).

### Logic Comparison: Python vs. JavaScript
| Feature | Python | JavaScript |
| :--- | :--- | :--- |
| **Logic** | `if guess == secret:` | `if (guess === secret) {` |
| **Print** | `print("Hello")` | `console.log("Hello")` |
| **Input** | `input("Guess:")` | `rl.question("Guess:")` |

> [!NOTE]
> **Security Context (Programming)**:
> Always use **Strict Equality** (`===`) in JavaScript to prevent "type coercion" errors, which can lead to logical vulnerabilities in authentication systems.

---

## 🗄️ Database Fundamentals (SQL)
Databases store information in structured **Tables** consisting of **Rows** (records) and **Columns** (attributes).

### Common SQL Keywords
* **SELECT**: Choose the columns to display.
* **FROM**: Specify the table to query.
* **WHERE**: Filter the results based on a condition.
* **ORDER BY**: Sort the results (e.g., `DESC` for highest to lowest).

---

## 🔗 Original Resources
* [THM Room: Data Representation](https://tryhackme.com/room/datarepresentation)
* [THM Room: Data Encoding](https://tryhackme.com/room/dataencoding)
* [THM Room: Python Simple Demo](https://tryhackme.com/room/pythonsimpledemo)
* [THM Room: JavaScript Simple Demo](https://tryhackme.com/room/javascriptsimpledemo)
* [THM Room: Database SQL Basics](https://tryhackme.com/room/databasesqlbasics)

---
*Next Module: [Attacks and Defenses](./07-attacks-and-defenses.md)*