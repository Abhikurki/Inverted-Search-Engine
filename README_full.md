# 🔍 Inverted Search Engine (C Project)

## 📌 Project Description

This project implements an **Inverted Search Engine** using C
programming. It reads multiple text files, processes words, and creates
a database that maps each word to the files in which it appears. It uses
hashing and linked lists for efficient storage and fast retrieval.

------------------------------------------------------------------------

## 📂 Project Files & Description

### 1. main.c

-   Entry point of the program\
-   Handles user menu and function calls\
-   Takes file names as command-line arguments

### 2. createdatabase.c

-   Reads input files\
-   Breaks content into words\
-   Stores words into hash table

### 3. displaydatabase.c

-   Displays the entire database\
-   Shows words, file count, and occurrences

### 4. searchdatabase.c

-   Searches for a given word\
-   Displays files where the word is found

### 5. savedatabase.c

-   Saves database into a file\
-   Helps reuse data without rebuilding

### 6. updatedatabase.c

-   Updates existing database from saved file\
-   Avoids rebuilding from scratch

### 7. inverted_search.h

-   Header file\
-   Contains structure definitions and function declarations

------------------------------------------------------------------------

## ⚙️ How to Compile

``` bash
gcc *.c -o search_engine
```

## ▶️ How to Run

``` bash
./search_engine file1.txt file2.txt
```

------------------------------------------------------------------------

## 🧭 How to Use

1.  Run the program with input files\
2.  Choose options from menu:
    -   Create Database\
    -   Display Database\
    -   Search Word\
    -   Save Database\
    -   Update Database\
3.  Enter required input when prompted

------------------------------------------------------------------------

## 📥 Sample Output

    1. Create Database
    2. Display Database
    3. Search
    4. Save Database
    5. Update Database
    Enter your choice: 1

    Database created successfully!

    Enter your choice: 3
    Enter word to search: data

    Word found!
    File: file1.txt -> Count: 3
    File: file2.txt -> Count: 1

    Enter your choice: 2

    Word      File Count    Occurrences
    data      2             file1.txt(3), file2.txt(1)
    code      1             file1.txt(2)

------------------------------------------------------------------------

## 🚀 Key Concepts Used

-   Hashing\
-   Linked Lists\
-   File Handling\
-   Data Structures

------------------------------------------------------------------------

## 👨‍💻 Author

Abhishek Y
