Assembly language is a low level programming language which is specific to each processor architecture. e.g. x86 ASM is used on x86 (32 bit) processors

Our exam board Oxford AQA has its own Assembly Language which is specified in the syllabus, it has a limited number of commands. It can be found in [Appendix 6 of the syllabus](https://www.oxfordaqa.com/wp-content/uploads/2024/04/oxfordaqa-a-level-computer-science-specification.pdf). but I've also summarised it here in [[oaqa_assembly_syntax]]

Use the [Peter Higgson AQA Assembly Simulator](https://www.peterhigginson.co.uk/AQA/) and the [Documentation](https://www.peterhigginson.co.uk/AQA/info.html) to write, run and test assembly language programs

Please note that there are some additions to the standard OAQA syntax with:

| Mnemonic | Meaning                                                                                  |
| -------- | ---------------------------------------------------------------------------------------- |
| OUT Rd   | Output to the output box from the given register                                         |
| INP Rd   | Input to the given register from the input box                                           |
| DAT Data | Store the data into the next available memory reference (use at the end of your program) |
|          |                                                                                          |

``` ASM
	  // An example of adding two numbers from input
      INP R0,2
      INP R1,2
      ADD R2,R1,R0
      OUT R2,4
      HALT
```

``` ASM
      // Input two numbers and output the higher
      INP R0,2
      INP R1,2
      CMP R1,R0
      BGT HIGHER
      OUT R0,4
      B DONE
HIGHER:
      OUT R1,4
DONE:
      HALT
```
