# Super Script Compiler  
**The AI Language**

---

## Overview

**Super Script Compiler** is a powerful automation tool designed to streamline your file processing workflows with the help of AI. This tool leverages advanced AI capabilities to convert pseudo-code into functional Python scripts. Whether you're dealing with regular files or AI-generated instructions, Super Script Compiler automates file handling, code generation, and change tracking, ensuring that you always stay efficient and productive.

With built-in file hash tracking, the Super Script Compiler ensures only modified or new files are processed, reducing redundancy and optimizing performance.

---

## Features

- **AI-Powered Code Generation**: Automatically converts `.ai` files containing pseudo-code into functional Python scripts.
- **Intelligent File Tracking**: Uses file hashing to detect and process only modified or new files, saving time and resources.
- **Progress Monitoring**: Visual progress bars provide real-time feedback during file processing.
- **Automatic Cleanup**: Unused files in the source directory are automatically removed if they no longer exist in the build directory.

---

## Installation

1. **Download the Binary**  
   Download the latest binary from [the provided link](https://github.com/Reconfigure-In/SuperScript/releases/tag/Alpha) and place it in your desired directory.
   Link: [github.com/Reconfigure-In/SuperScript/releases/tag/Alpha](https://github.com/Reconfigure-In/SuperScript/releases/tag/Alpha)

3. **Make the Binary Executable**  
   Ensure the binary has executable permissions by running:

   ```bash
   chmod +x ./SuperScript
   ```

---

## Usage

### Folder Structure

Before running the Super Script Compiler, ensure that your project structure includes the following directories:

- **`build/`**: Place all the files you want to process in this directory. AI-related files should have a `.ai` extension.
- **`src/`**: This directory will be automatically created (if not already present) and will contain the processed files. Any pseudo-code converted by the AI will be saved here as `.py` files.

### Running the Compiler

1. Ensure the **`build`** directory contains the files you want to process.
   
2. Execute the Super Script Compiler:

   ```bash
   ./SuperScript
   ```

3. The script will process all the files in the `build` directory and output the results to the `src` directory. You'll see progress bars and logging output in the console, showing what’s being processed, skipped, or removed.

---

## How It Works

1. **Place Files**: Add your source files (e.g., `.ai`, `.txt`, `.py`) in the `build` directory.
   
2. **Run the Compiler**: Upon running, the compiler processes all files:
   - It converts `.ai` files into Python code using AI assistance.
   - Non-AI files are copied directly to the `src` directory.
   - Unchanged files are skipped to save time.

3. **Check Output**: The processed files are stored in the `src` directory. AI-generated content is saved as `.py` files, while unchanged or non-AI files are copied as they are.

4. **Automated Cleanup**: Any files in the `src` directory that no longer exist in the `build` directory are automatically deleted.

---

## Sample Workflow

1. **Add Pseudo-Code**  
   Create a file in the `build/` directory named `example.ai` with some pseudo-code:

   ```pseudo
   # Pseudo-code example
   Define a function that adds two numbers
   ```

2. **Run Super Script Compiler**  
   Execute the binary and let the AI generate Python code for the pseudo-code:

   ```bash
   ./SuperScript
   ```

3. **Output**  
   The `example.ai` file will be converted and saved as `example.py` in the `src/` directory:

   ```python
   # Generated Python code
   def add_numbers(a, b):
       return a + b
   ```

---

## Error Handling

- **Missing Build Directory**: If the `build` directory is not found, the script will terminate with an error message.
- **Empty AI Files**: Any `.ai` file that is empty will be skipped, and a warning will be logged.
- **Unchanged Files**: Files that haven't changed since the last run are skipped, reducing unnecessary reprocessing.

---

## Conclusion

Super Script Compiler is a versatile tool designed to enhance developer productivity by seamlessly integrating AI into your workflow. Whether you're managing a large project or a small script repository, this tool automates the process, ensuring efficiency with every file processed.

Start using **Super Script Compiler** today and let the AI handle the heavy lifting for you!
