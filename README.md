# java-project
A java project built using concept of File I/O.
Project Name = File Packer Unpacker.


# 📦 File Packer & Unpacker

A simple **Java-based utility** that can **pack** multiple files into a single file and **unpack** them back to their original form.  
This project is split into **two separate programs**:  
- `Packer.java` → Packs files together.  
- `Unpacker.java` → Extracts files from a packed file.

---

## 🚀 Features
- Pack multiple files into a single binary file.
- Unpack and restore original files.
- Easy to use via command line.
- Supports any file type (`.txt`, `.jpg`, `.pdf`, etc.).
- File size & name metadata stored for accurate unpacking.

---

## 📂 Project Structure
```

File-Packer-Unpacker/
│── Packer.java     # Program to pack files
│── Unpacker.java   # Program to unpack files
│── README.md       # Documentation
│── sample\_files/   # Example files to pack
│── output/         # Packed and unpacked files

````

---

## ⚙️ How It Works
1. **Packer**
   - Reads each file.
   - Stores its name and size.
   - Writes file content into a single `.pack` file.
   
2. **Unpacker**
   - Reads the `.pack` file.
   - Extracts files using stored metadata.
   - Writes them back into the destination folder.

---

## 🖥️ Usage

### 1️⃣ Compile
```bash
javac Packer.java
javac Unpacker.java
````

### 2️⃣ Pack Files

```bash
java Packer <source_directory> <packed_file_name>
```

Example:

```bash
java Packer sample_files packed_data.pack
```

### 3️⃣ Unpack Files

```bash
java Unpacker <packed_file_name> <destination_directory>
```

Example:

```bash
java Unpacker packed_data.pack output
```

---

## 📝 Example

If you have:

```
sample_files/
  file1.txt
  file2.jpg
```

Running:

```bash
java Packer sample_files data.pack
```

Creates:

```
data.pack
```

Then:

```bash
java Unpacker data.pack output
```

Restores:

```
output/file1.txt
output/file2.jpg
```

---

## 📌 Requirements

* Java 8 or above
* Basic knowledge of file I/O in Java

---

## 📜 License

This project is open-source and free to use.








