# 8085-Microprocessor-Simulator

## Objective: Design and Develop a desktop Application to emulate the fuctionality of 8085 Microprocessor.

This microprocessor constains following instructions:<br/>
**A. Load and Store:**<br /> 1. MOV-This instruction copies the contents of the source register into the destination register without any alteration.<br/> 2. MVI-The 8-bit data is stored in the destination register or memory.<br/> 3. LXI-The instruction loads 16-bit data in the register pair designated in the register or the memory.<br/> 4. LDA-The contents of a memory location, specified by a 16-bit address in the operand, are copied to the accumulator.<br/> 5. STA-The contents of the accumulator are copied into the memory location specified by the operand.<br/> 6. LHLD-The instruction copies the contents of the memory location pointed out by the address into register L and copies the contents of the next memory location into register H.<br/> 7. SHLD-The contents of register L are stored in the memory location specified by the 16-bit address in the operand and the contents of H register are stored into the next memory location by incrementing the operand.<br/> 8. STAX-The contents of the accumulator are copied into the memory location specified by the contents of the operand.<br/> 9. XCHG-The contents of register H are exchanged with the contents of register D, and the contents of register L are exchanged with the contents of register E.<br/>
**B. Arithmetic:**<br/> 1. ADD-The contents of the register or memory are added to the contents of the accumulator and the result is stored in the accumulator.<br/> 2. ADI-The 8-bit data is added to the contents of the accumulator and the result is stored in the accumulator.<br/> 3. SUB-The contents of the register or the memory are subtracted from the contents of the accumulator, and the result is stored in the accumulator.<br/> 4. INR-The contents of the designated register or the memory are incremented by 1 and their result is stored at the same place.<br/> 5. DCR-The contents of the designated register or memory are decremented by 1 and their result is stored at the same place.<br/> 6. INX-The contents of the designated register pair are incremented by 1 and their result is stored at the same place.<br/> 7. DCX-The contents of the designated register pair are decremented by 1 and their result is stored at the same place.<br/> 8. DAD-The 16-bit data of the specified register pair are added to the contents of the HL register.<br/> 9. SUI-The 8-bit data is subtracted from the contents of the accumulator & the result is stored in the accumulator.<br/>
**C. Logical:**<br/> 1. CMA-The contents of the accumulator are complemented. No flags are affected.<br/> 2. CMP-The contents of the operand (register or memory) are M compared with the contents of the accumulator.<br/>
**D. Branching:**<br/> 1. JMP-The program sequence is transferred to the memory address given in the operand.<br/> 2. JC-The program sequence is transferred to the memory address given in the operand when carry flag is 1.<br/> 3. JNC-The program sequence is transferred to the memory address given in the operand when carry flag is 0.<br/> 4. JZ-The program sequence is transferred to the memory address given in the operand when zero flag is 1.<br/> 5. JNZ-The program sequence is transferred to the memory address given in the operand when zero flag is 0.<br />
**E. Extra**:<br/>
An additional command SET is used to set data into memory location.<br/>
SYNTAX: `SET <Memory Address>, <2 Byte Hexadecimal Data>`<br/>
eg: `SET 2500, FF`

You can also use inbuilt debugger to debug your 8085 program. The debugger has following 6 functionality/ commands:<br/> 1. break or b <line number>: It will set breakpoint on given line number.<br/>
Eg: `break 10 or b 10`<br/> 2. run or r : It will run the program until end of code or breakpoint is encountered.
Eg: `run or r`<br/> 3. step or s : It will run the program one instruction at a time.
Eg: `step or s`<br/> 4. print or p : It will print value of register, flags, current line number or memory location.<br/>
To print value of register use print or p <Register>. Eg: `print A` or `p A`.<br/>
To print value flag use print or p flag. Eg: `print flag` or `p flag`.<br/>
To print current line number use print or p loc. Eg: `print loc` or `p loc`.<br/>
To print value of memory location use print or p x<memory address>. Eg: `print x2000` or `p x2000.`<br/> 5. Quit or q : Quits the debugger.<br/>
Eg: `quit` or `q`<br/> 6. help : It will show all the commands of the debugger.<br/>
Eg: `help`<br/>
