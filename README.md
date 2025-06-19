# MULTITHREADED-FILE-COMPRESSION-TOOL

*COMPANY* : CODTECH IT SOLUTIONS

*NAME* : RAGINI KUMARI

*INTERN ID* : CT04DN1698

*DOMAIN NMAE* : C++ PROGRAMMING

*DURATION* : 4 WEEKS

*MENTOR* : Neela Santhosh Kumar

## DESCRIPTION ##

*Multithreaded File Compression Tool – C++ Project*

*Introduction*

This project is a File Compression and Decompression Tool written in C++ using the Run-Length Encoding (RLE) algorithm. It allows users to compress large sequences of repeated characters into a smaller form, and later decompress them back into their original format. This tool reads content from a text file, performs compression or decompression based on user input, and saves the result to an output file. Though the current version is single-threaded, it lays the groundwork for a multithreaded extension for higher performance with large datasets.

The program is designed for a command-line environment and is built using Visual Studio Code with the g++ compiler (MinGW) on Windows. It showcases not only fundamental file I/O operations but also highlights the potential of basic compression techniques in real-world scenarios.

*How It Works*

*1. Compression (compressRLE)*

  . Compresses the input using Run-Length Encoding by counting the number of repeated characters and replacing them with a number followed by the character.

  . Example: AAAAAAAAAABBBBCCCCDDDDDDDDDDDDDEEEE becomes 10A4B4C13D4E.

*2. Decompression (decompressRLE)*

  . Decodes the RLE string by expanding each character based on its preceding number.

.  Handles validation for incorrect formats.

*3. File Handling*

  . Reads from input.txt for compression and writes the result to compressed.txt.

  . Reads from compressed.txt for decompression and writes to decompressed.txt.

*4. User Input

  . Asks the user whether to compress (c) or decompress (d).

  . Handles invalid options gracefully.

*Use Cases and Applications* 

Though simple in logic, this compression tool is quite versatile and can be applied in various scenarios:

*. Log File Archiving:* Compress large server or application logs to save disk space and improve archival efficiency.

*. Data Transmission:* Use compression to reduce data size before sending files over a network.

*. Embedded Systems:* In low-memory environments, RLE is useful for compressing repetitive data like sensor logs or configuration strings.

*. Backup Systems:* Compress plain-text backups for lightweight storage.

*. Educational Purpose:* This project serves as an excellent introduction to file compression algorithms, file I/O, exception handling, and modular programming in C++.

*. Foundation for Larger Tools:* It can be expanded into a full-fledged file compression utility by supporting more formats (e.g., Huffman, LZW) or binary file support.

*Multithreading Potential*

To evolve this into a Multithreaded File Compression Tool, the file can be divided into chunks, and each chunk can be compressed or decompressed independently by separate threads. This can significantly reduce processing time for large files.

For example:

. Split the input into multiple strings or file segments.

. Launch threads using std::thread or thread pools.

. Perform parallel compression on each segment.

. Join the threads and concatenate the results.

This design can be extended to handle multiple files or real-time compression pipelines.

*Development Environment*

. Language: C++

. Editor: Visual Studio Code

. Compiler: g++ (MinGW)

. Platform: Windows 10/11

. Libraries Used: <iostream>, <fstream>, <string>, <cctype>, and (for multithreaded version) <thread>

*How to Compile and Run*

1. Save the file as rle_tool.cpp.

2. Open terminal in VS Code.

3. Compile using:

g++ rle_tool.cpp -o rle_tool

4. Run the program:

./rle_tool

5. Input c to compress or d to decompress.

*Conclusion*

This File Compression Tool is a functional and educational example of how simple algorithms like Run-Length Encoding can be applied in real-world applications. By reading from and writing to files, it bridges file I/O with algorithmic logic. With potential multithreading enhancements, the tool can be made scalable and much faster for larger datasets.

Whether you're a student learning about compression, a developer building file utilities, or someone looking to reduce file size, this project provides a solid foundation and plenty of room for further development.

#OUTPUT

![Image](https://github.com/user-attachments/assets/324f5403-3d3c-4da4-b013-067442a6d378)

