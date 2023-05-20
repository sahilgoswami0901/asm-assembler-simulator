# Instruction Set Architecture(ISA) used while designing of Assembler and Simulator:
Program an assembler for the aforementioned ISA and assembly. 
The input to the assembler is
a text file containing the assembly instructions. Each line of the text file may be of one of 3
types:
● Empty line: Ignore these lines
● A label
● An instruction
● A variable definition
Each of these entities have the following grammar:
● The syntax of all the supported instructions is given above. The fields of an instruction are
whitespace separated. The instruction itself might also have whitespace before it. An
instruction can be one of the following:
● The opcode must be one of the supported mnemonic.
● A register can be one of R0, R1, ... R6, and FLAGS.
● A mem_addr in jump instructions must be a label.
● A Imm must be a whole number <= 255 and >= 0.
● A mem_addr in load and store must be a variable.
● A label marks a location in the code and must be followed by a colon (:). No spaces are
allowed between label name and colon(:)
● A variable definition is of the following format:
var xyz
which declares a 16 bit variable called xyz. This variable name can be used in place of
mem_addr fields in load and store instructions. All variables must be defined at the
very beginning of the assembly program.
