# minigrep
This repository, **minigrep**, is a simple command-line tool implemented in Rust that mimics basic functionality of the `grep` command. It allows you to search for a specified query within a text file, with options for case-sensitive and case-insensitive searches. 

### Key Features
- **File Reading**: Reads contents from a specified file, provided through the command line.
- **Case Sensitivity Control**: Case-sensitive by default; environment variable `CASE_INSENSITIVE=1` enables case-insensitive search.
- **Configurable Queries**: Accepts a search query and filename as command-line arguments.
- **Error Handling**: Handles missing or invalid arguments and file read errors gracefully using the `Result` type and Rust’s `?` operator.

### Code Overview
- **`run` Function**: Core function that executes the search logic and displays matching lines.
- **`Config` Struct**: Manages command-line arguments, including filename, query, and case sensitivity, with input validation.
- **Search Functions**: 
  - `search` for case-sensitive search.
  - `search_case_insensitive` for case-insensitive search by converting both query and contents to lowercase.

### Tests
Includes tests for both search modes, ensuring accurate results across case variations. This tool demonstrates core Rust principles like error handling, ownership, and test-driven development (TDD). 

