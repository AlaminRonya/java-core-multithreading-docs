# 🧠 CPU — কম্পিউটারের মস্তিষ্ক

---

# 🔰 CPU কী?

CPU (Central Processing Unit) হলো কম্পিউটারের **Brain বা মস্তিষ্ক**।  
কম্পিউটারের সমস্ত Instruction Process করা, Calculation করা এবং Hardware Control করার কাজ CPU করে।

📌 সহজভাবে:
> মানুষ যেমন মস্তিষ্ক দিয়ে চিন্তা করে,  
কম্পিউটার তেমনি CPU দিয়ে কাজ করে।

---

# 🏗️ CPU এর প্রধান অংশসমূহ

## ১️⃣ ALU (Arithmetic Logic Unit)

এটি গাণিতিক ও লজিক্যাল অপারেশন সম্পন্ন করে।

### উদাহরণ:
- Addition (+)
- Subtraction (-)
- Comparison (>, <, ==)

📌 Example:
```text
10 + 20 = 30
```

---

## Control Unit (CU)

Control Unit পুরো CPU এর কাজ নিয়ন্ত্রণ করে।

### কাজ:
- Instruction নিয়ন্ত্রণ
- Data Flow নিয়ন্ত্রণ
- কোন কাজ কখন হবে তা নির্ধারণ

---

## Registers

Registers হলো CPU এর ভিতরের খুব ছোট কিন্তু অত্যন্ত দ্রুতগতির Memory।

### ব্যবহার:
- Temporary Data Store
- Current Instruction Store

📌 RAM থেকেও অনেক দ্রুত।

---

## Cache Memory

Cache Memory হলো CPU এর High-Speed Memory।

এটি Frequently Used Data সংরক্ষণ করে।

📌 উদ্দেশ্য:
RAM Access কমিয়ে CPU Speed বাড়ানো।

---

# 🔄 CPU কীভাবে কাজ করে?

CPU একটি নির্দিষ্ট Cycle অনুসরণ করে কাজ করে:

# ✅ Fetch → Decode → Execute Cycle

```text
Fetch → Decode → Execute → Repeat
```

---

## Fetch

CPU RAM থেকে Instruction নিয়ে আসে।

📌 Example:
```java
int a = 10 + 20;
```

---

## Decode

CPU Instruction এর অর্থ বুঝে।

📌 যেমন:
```text
Addition করতে হবে
```

---

## Execute

Instruction অনুযায়ী কাজ সম্পন্ন হয়।

📌 Result:
```text
30
```

---

# 📊 Flow Diagram

```text
+---------+
| Fetch   |
+---------+
     ↓
+---------+
| Decode  |
+---------+
     ↓
+---------+
| Execute |
+---------+
     ↓
 Repeat Again
```

---

# 🧩 CPU Core কী?

Core হলো CPU এর ভিতরের Processing Unit।

একটি CPU তে একাধিক Core থাকতে পারে।

---

# 🖥️ CPU vs Core

| CPU | Core |
|---|---|
| পুরো Processor | Processor এর ভিতরের Unit |
| সব Core কে ধারণ করে | Instruction Execute করে |

---

# 💻 Single Core Processor

একটি মাত্র Core থাকে।

### বৈশিষ্ট্য:
- এক সময়ে একটি Task ভালোভাবে করে
- Multitasking দুর্বল

---

# 🚀 Multi Core Processor

একাধিক Core থাকে।

### উদাহরণ:
- Dual Core → 2 Core
- Quad Core → 4 Core
- Octa Core → 8 Core

### সুবিধা:
✅ Fast Performance  
✅ Better Multitasking  
✅ Parallel Processing

---

# 🔄 Single Core CPU তে Multitasking

Single Core CPU খুব দ্রুত Task পরিবর্তন করে।

এটিকে বলে:

- Time Slicing
- Context Switching

---

# ⏳ Time Slicing

CPU প্রতিটি Process কে অল্প সময় দেয়।

📌 Example:

```text
Chrome → 5ms
VS Code → 5ms
Music Player → 5ms
```

---

# 🔁 Context Switching

CPU যখন এক Process থেকে অন্য Process এ যায়:

- Current State Save করে
- নতুন Process Load করে

এটিই Context Switching।

---

# 🧠 OS Scheduler এর ভূমিকা

Operating System এর Scheduler সিদ্ধান্ত নেয়:

✅ কোন Process চলবে  
✅ কখন চলবে  
✅ কতক্ষণ চলবে  

---

# 📊 Scheduler Flow

```text
Process Queue
     ↓
+----------------+
| OS Scheduler   |
+----------------+
     ↓
      CPU
```

---

# ⚡ CPU Bound Task vs I/O Bound Task

| CPU Bound | I/O Bound |
|---|---|
| বেশি Calculation করে | বেশি Waiting করে |
| CPU Intensive | Disk/Network নির্ভর |
| Example: Rendering | Example: Download |

---

# 🧵 Hardware Level Single-threaded Core

এক সময়ে একটি Thread Execute করে।

📌 Performance কম হতে পারে।

---

# 🚀 Multi-threaded Core

একাধিক Thread Handle করতে পারে।

### উদাহরণ:
- Intel Hyper Threading
- SMT (Simultaneous Multithreading)

---

# 🧱 Process কী?

Process হলো একটি Running Program।

📌 Example:
- Chrome
- VS Code
- Spotify

---

# 🧵 Thread কী?

Thread হলো Process এর ছোট Execution Unit।

একটি Process এর ভিতরে Multiple Thread থাকতে পারে।

---

# 📊 Process vs Thread

| Process | Thread |
|---|---|
| Heavyweight | Lightweight |
| আলাদা Memory | Shared Memory |
| Slow Creation | Fast Creation |

---

# 📌 Diagram

```text
Process
 ├── Thread-1
 ├── Thread-2
 └── Thread-3
```

---

# ⚔️ Concurrency vs Parallelism

# 🔄 Concurrency

একাধিক Task একসাথে Progress করে।

📌 Single Core CPU তেও সম্ভব।

---

# ⚡ Parallelism

একাধিক Task একই সময়ে Execute হয়।

📌 Multi-Core CPU প্রয়োজন।

---

# 📊 Example

| Concurrency | Parallelism |
|---|---|
| Task Switching | True Simultaneous Execution |
| Single Core Possible | Multi-Core Required |

---

# 🧠 CPU Cache

CPU Cache হলো Ultra Fast Memory।

RAM এর তুলনায় অনেক দ্রুত।

---

# 📚 Cache Levels

| Cache | Speed | Size |
|---|---|---|
| L1 Cache | Fastest | Smallest |
| L2 Cache | Faster | Medium |
| L3 Cache | Slower | Largest |

---

# 📊 Cache Hierarchy Diagram

```text
CPU
 ↓
L1 Cache
 ↓
L2 Cache
 ↓
L3 Cache
 ↓
RAM
```

---

# 🎯 গুরুত্বপূর্ণ Interview Questions

## ❓ CPU কী?

CPU হলো কম্পিউটারের Central Processing Unit যা সমস্ত Instruction Execute করে।

---

## ❓ Core এবং CPU এর পার্থক্য কী?

CPU পুরো Processor Chip আর Core হলো Processing Unit।

---

## ❓ Context Switching কী?

এক Process থেকে অন্য Process এ Switch করার সময় State Save/Restore করাকে Context Switching বলে।

---

## ❓ Concurrency এবং Parallelism এর পার্থক্য কী?

Concurrency = একসাথে Progress  
Parallelism = একই সময়ে Execute

---

# ✅ Summary

এই অধ্যায়ে আমরা শিখলাম:

✅ CPU Basics  
✅ CPU Components  
✅ Fetch Decode Execute Cycle  
✅ CPU Core  
✅ Single vs Multi Core  
✅ Multitasking  
✅ OS Scheduler  
✅ Time Slicing  
✅ Context Switching  
✅ Process vs Thread  
✅ Concurrency vs Parallelism  
✅ CPU Cache Hierarchy  

