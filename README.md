# Huffman Coding Compression and Decompression

This project implements Huffman Coding, a popular algorithm for lossless data compression. The code provides functionalities to compress and decompress text files using Huffman Coding.

## Features

- **Compression:** Reads a text file, generates Huffman codes, and writes the compressed data to an output file.
- **Decompression:** Reads the compressed file, decodes it using the stored Huffman codes, and writes the original text to a decompressed file.

## How It Works

1. **Character Frequency Count:** Reads the input file and counts the frequency of each character.
2. **Min-Heap Construction:** Builds a min-heap (priority queue) of nodes where each node represents a character and its frequency.
3. **Huffman Tree Construction:** Constructs the Huffman tree by repeatedly merging the two nodes with the smallest frequencies.
4. **Huffman Code Generation:** Generates the Huffman codes for each character by traversing the Huffman tree.
5. **Compression:** Encodes the input text using the generated Huffman codes and writes the encoded data along with the Huffman codes to an output file.
6. **Decompression:** Reads the compressed file, reconstructs the Huffman codes, decodes the encoded data, and writes the original text to a decompressed file.

## How to Use

### Prerequisites

- Ensure you have a C++ compiler installed, such as `g++`.

### Steps to Use

1. **Clone the Repository:**

    ```sh
    git clone https://github.com/chaman-yadav/file-compressor.git
    cd file-compressor
    ```

2. **Compile the Program:**

    ```sh
    g++ -o file-compressor code.cpp
    ```

3. **Run the Program:**

    ```sh
    ./file-compressor
    ```

4. **Choose an Option from the Menu:**

    - Enter `1` to compress a file.
    - Enter `2` to decompress a file.

5. **Follow the Prompts:**

    - For compression, enter the filename of the text file you want to compress. The compressed output will be saved as `output.txt`.
    - For decompression, enter the filename of the compressed file (e.g., `output.txt`). The decompressed output will be saved as `decompressed.txt`.

### Notes

- Ensure the file to be compressed or decompressed is in the same directory as the compiled program.
- The compressed file (`output.txt`) contains the Huffman codes and the encoded text.
- The decompressed file (`decompressed.txt`) will contain the original text.

### Repository

Find the complete code and additional details in the [file-compressor](https://github.com/chaman-yadav/file-compressor) repository on GitHub.
