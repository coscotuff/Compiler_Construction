# Compiler_Construction

- This is the github repository for a working compiler for a unique C-like langauge, _ErPlag_. The custom design specifics of the language have been mentioned in the _language_specifications.pdf_ file. The project has been made for the purposes of the 2022-2023 offering of the course CS-F363 (Compiler Construction) at BITS Pilani under instructor Vandana Agarwal. This project includes the implementation of all of the theoretical modules of a compiler: lexical analyser, syntax analyser (parser), semantic analyser, and code generator.

The language supports features such as:
    - Arithmetic and boolean expressions
    - Strongly typed language
    - Returning multiple values from a function
    - Static scoping of variables
    - Assignment, I/O, Declarative, Iterative, Conditional, Function call statements


## _Note: All files on this repository are for educational purpose solely._

## How to run?

The compiler can be run by following the following steps:

    - Open the project directory on a Linux terminal, and run:
      ```
      > make
      ```
    - Execute the following command:
      ```
      > ./compiler <testcase_file.txt> <generated_code.asm>
      ```
    - Where:
        - <testcase_file.txt> could be replaced with any .txt file. For performing lexical, syntactic, semantic and execution checks, files *t[1-6].txt, ts[1-10].txt, or c[1-10].txt* can be run (in case the user is curious :D). Note these contain lexical, syntactic and semantic errors for testing the robustness of the compiler.
        - <generated_code.asm> is the x86 generated executable code. It could be replaced with any .asm file name. Note that this file will only be generated if the input .txt file is correct lexically, syntactically, and semantically.
    -  To run the generated .asm file, execute the following command:
        ```
        > nasm -felf64 <generated_code.asm> && ld code.o && ./a.out
        ```
_Note: This project has been developed using **gcc version 11.3.0 ~ ubuntu 22.04** and **nasm version 2.14.02**. Please ensure compatibility with these versions on your system prior to testing._
- Finally, cheers and shoutout to my teammates **_Harsh, Hrishikesh, Antriksh, and Kaustab_** for their contributions to the project. It is all those little steps that make the journey complete. The journey is the reward, and my journey with them has been in truly invaluable.
