//This is a modified project project from the previuosly existing ones. This project aims to compress files using Huffman Compression Algorithm, where the code is built in C programming language.

Title: Huffman Coding: Efficient Data Compression Algorithm

Introduction:
Huffman coding, named after David A. Huffman, is a widely used algorithm for data compression. It provides a lossless compression technique that reduces the size of data files without compromising the original information. This project aims to implement Huffman coding, and showcase its efficiency in compressing and decompressing textual data.

Overview of Huffman Coding:
Huffman coding is a variable-length prefix coding algorithm. It assigns shorter codes to frequently occurring characters and longer codes to less common ones, resulting in a compact representation of the input data. The algorithm constructs a binary tree, known as the Huffman tree, based on the frequency of characters in the input file. The tree is then used to generate unique codes for each character.

Building the Huffman Tree:
To build the Huffman tree, the project first reads the input file and calculates the frequency of each character present. This information is used to create nodes for each character, forming a forest of single-node trees. The project then combines the two trees with the lowest frequency into a single tree until a single tree remains, representing the Huffman tree.

Generating Huffman Codes:
Once the Huffman tree is constructed, the project traverses the tree to assign codes to each character. Starting from the root, a left traversal represents a '0' bit, while a right traversal represents a '1' bit. These codes are stored in a lookup table for efficient encoding and decoding.

Compressing Data:
With the Huffman codes generated, the project proceeds to compress the input text file. It reads the input file character by character and replaces each character with its corresponding Huffman code. The compressed data is then written to an output file, along with the necessary metadata required for decompression.

Decompressing Data:
To decompress the compressed data, the project reads the compressed file and rebuilds the Huffman tree using the metadata. It then traverses the tree using the encoded bits and retrieves the original characters. The decompressed data is then written to an output file, restoring the original text.

Evaluation and Performance:
The project includes an evaluation of the compression ratio achieved by Huffman coding compared to the original file size. Additionally, it measures the time taken for compression and decompression processes, highlighting the algorithm's efficiency. The results are displayed and compared, demonstrating the effectiveness of Huffman coding in reducing file sizes.

Conclusion:
Huffman coding is a powerful data compression algorithm widely used in various applications. This project showcases the implementation of Huffman coding in the C programming language, enabling efficient compression and decompression of text files. Through this project, you can gain a deeper understanding of Huffman coding's inner workings, its benefits, and its role in modern data compression techniques.
