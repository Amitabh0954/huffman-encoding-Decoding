Huffman Coding File Compressor
This project implements a Huffman coding algorithm to compress and decompress files.

Overview
Huffman coding is a lossless data compression algorithm. The program reads an input file, generates a Huffman tree based on the frequency of characters, and encodes the file into a compressed format. It can also decompress the encoded file back to its original content.

Features
Compression: Reduces the file size using Huffman coding.
Decompression: Restores the original file from the compressed format.
File Structure
huffman.hpp: Header file containing class definitions and function declarations.
huffman.cpp: Implementation file with method definitions.
encode.cpp: Main file to compress an input file.
decode.cpp: Main file to decompress an encoded file.
How to Compile
Ensure you have g++ installed on your system. Use the following commands to compile the project:

For compression: g++ encode.cpp huffman.cpp -o encode
For decompression: g++ decode.cpp huffman.cpp -o decode
How to Use
Compression
To compress a file, run the following command:

./encode <input_file> <output_file>

Replace <input_file> with the name of the file you want to compress and <output_file> with the desired name for the compressed file.

Example:

./encode input.txt output.huff

Decompression
To decompress a file, run the following command:

./decode <encoded_file> <output_file>

Replace <encoded_file> with the name of the Huffman encoded file and <output_file> with the desired name for the decompressed file.

Example:

./decode output.huff decoded.txt

Example
Given an input.txt file of size 2117 KB, the compressed output.huff file is 1120 KB, demonstrating a significant reduction in file size.

Acknowledgements
Based on the Huffman coding algorithm for data compression.
Developed as a learning project for understanding data compression techniques.
