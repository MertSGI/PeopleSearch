
# People Search Program 🕵️‍♂️

This Kotlin program allows you to search for people in a dataset based on various matching strategies (ALL, ANY, NONE). It uses an inverted index for efficient searches.

---

## 🚀 Features

- **Search by Matching Strategy**:
  - **ALL**: Find entries that match all search terms.
  - **ANY**: Find entries that match at least one search term.
  - **NONE**: Exclude entries that match any search term.
- **Inverted Index**: Efficiently maps words to their occurrences in the dataset.
- **Menu-Driven Interface**: Provides an intuitive interface for search and display operations.

---

## 🛠️ How to Use

1. **Run the Program**  
   Compile and run the program using Kotlin:
   ```bash
   kotlinc people_search.kt -include-runtime -d people_search.jar
   java -jar people_search.jar --data <filename>
   ```

2. **Provide Input File**  
   The program expects a text file containing one entry per line. Example file contents:
   ```
   John Doe johndoe@example.com
   Jane Smith janesmith@example.com
   ```

3. **Use the Menu**  
   The program provides the following options:
   ```
   === Menu ===
   1. Find a person
   2. Print all people
   0. Exit
   ```

4. **Search with Strategies**  
   Select a matching strategy (ALL, ANY, NONE) and enter your search query.

---

## 📖 Example Usage

### Input File
```
John Doe johndoe@example.com
Jane Smith janesmith@example.com
Alice Johnson alicej@example.com
```

### Example Commands
- **ALL Strategy**:
  - Search Query: `John Doe`
  - Output:
    ```
    John Doe johndoe@example.com
    ```

- **ANY Strategy**:
  - Search Query: `Jane John`
  - Output:
    ```
    John Doe johndoe@example.com
    Jane Smith janesmith@example.com
    ```

- **NONE Strategy**:
  - Search Query: `Doe`
  - Output:
    ```
    Jane Smith janesmith@example.com
    Alice Johnson alicej@example.com
    ```

---

## 🛠️ Requirements

- Kotlin Compiler
- JVM (Java Virtual Machine)

---

## 📬 Contributing

Contributions are welcome! If you find any issues or have ideas for new features, feel free to create an issue or submit a pull request.

---

## 📜 License

This project is licensed under the MIT License.

---

### Thank you for using the People Search Program! 😊
