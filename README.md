# Instruction List

Timing (3):
- NOP: "No OPeration" does nothing except going to the next instruction (made with a relative jump of 1)
- SLP [Value]: "SLeeP" like a NOP except it jumps to the next instruction after value clock cycles
- HALT: alias for a relative jump of 0

Data Logistics (7):
- CPY [Register 1] [Register 2]: "CoPY" write the value of register 1 to register 2
- SWP [Register 1] [Register 2]: "SWaP" write the value of register 1 into register 2 and write the value of register 2 into register 1 at the same time
- STLS [Value] [Register]: "SeT Least Significant bits" write the value to the lower half of the register
- STMS [Value] [Register]: "SeT Most Significant bits" write the value to the upper half of the register
- LOAD [Address] [Register]: write the value contained at the address into the register
- SAVE [Register] [Address]: write the value of the register at the address
- DRFL [Register 1] [Register 2]: "DeReFerence Load" load the value contained at the address equal to the value of register 1 into register 2
- DRFS [Register 1] [Register 2]: "DeReFerence Save" save the value of register 1 into the memory at the address contained in register 2

Memory Address Manipulations (40):
- JMP [Value]: "JuMP" set the next program address to value
- JEQZ [Register] [Value]: "Jump if register is EQual to Zero" set the next program address to value if the register is equal to zero
- JNEZ [Register] [Value]: "Jump if register is Not Equal to Zero" set the next program address to value if the register is not equal to zero
- JGTZ [Register] [Value]: "Jump if register is Greater Than Zero" set the next program address to value if the register is greater than zero
- JLTZ [Register] [Value]: "Jump if register is Less Than Zero" set the next program address to value if the register is less than zero
- JGEZ [Register] [Value]: "Jump if register is Greater than or Equal to Zero" set the next program address to value if the register is greater than or equal to zero
- JLEZ [Register] [Value]: "Jump if register is Less than or Equal to Zero" set the next program address to value if the register is less than or equal to zero
- JREQ [Register 1] [Register 2] [Register 3]: "Jump if Registers are EQual" set the next program address to the value of register 3 if register 1 and register 2 are equal
- JRNE [Register 1] [Register 2] [Register 3]: "Jump if Registers are Not Equal" set the next program address to the value of register 3 if register 1 and register 2 are not equal
- JRGT [Register 1] [Register 2] [Register 3]: "Jump if Register is Greater Than the other" set the next program address to the value of register 3 if register 1 is greater than register 2
- JRLT [Register 1] [Register 2] [Register 3]: "Jump if Register is Less Than the other" set the next program address to the value of register 3 if register 1 is less than register 2
- JRGE [Register 1] [Register 2] [Register 3]: "Jump if Register is Greater than or Equal to the other" set the next program address to the value of register 3 if register 1 is greater than or equal to register 2
- JRLE [Register 1] [Register 2] [Register 3]: "Jump if Register is Less than or Equal to the other" set the next program address to the value of register 3 if register 1 is less than or equal to register 2

- BRCH [Value]: "BRanCH" set the next program address to the sum of the current program address and value
- BEQZ [Register] [Value]: "Branch if register is EQual to Zero" set the next program address to the sum of the current program address and value if the register is equal to zero
- BNEZ [Register] [Value]: "Branch if register is Not Equal to Zero" set the next program address to the sum of the current program address and value if the register is not equal to zero
- BGTZ [Register] [Value]: "Branch if register is Greater Than Zero" set the next program address to the sum of the current program address and value if the register is greater than zero
- BLTZ [Register] [Value]: "Branch if register is Less Than Zero" set the next program address to the sum of the current program address and value if the register is less than zero
- BGEZ [Register] [Value]: "Branch if register is Greater than or Equal to Zero" set the next program address to the sum of the current program address and value if the register is greater than or equal to zero
- BLEZ [Register] [Value]: "Branch if register is Less than or Equal to Zero" set the next program address to the sum of the current program address and value if the register is less than or equal to zero
- BREQ [Register 1] [Register 2] [Register 3]: "Branch if Registers are EQual" set the next program address to the sum of the current program address and the value of register 3 if register 1 and register 2 are equal
- BRNE [Register 1] [Register 2] [Register 3]: "Branch if Registers are Not Equal" set the next program address to the sum of the current program address and the value of register 3 if register 1 and register 2 are not equal
- BRGT [Register 1] [Register 2] [Register 3]: "Branch if Register is Greater Than the other" set the next program address to the sum of the current program address and the value of register 3 if register 1 is greater than register 2
- BRLT [Register 1] [Register 2] [Register 3]: "Branch if Register is Less Than the other" set the next program address to the sum of the current program address and the value of register 3 if register 1 is less than register 2
- BRGE [Register 1] [Register 2] [Register 3]: "Branch if Register is Greater than or Equal to the other" set the next program address to the sum of the current program address and the value of register 3 if register 1 is greater than or equal to register 2
- BRLE [Register 1] [Register 2] [Register 3]: "Branch if Register is Less than or Equal to the other" set the next program address to the sum of the current program address and the value of register 3 if register 1 is less than or equal to register 2

- CALL [Value]: set the next program address to value and store the current address
- CEQZ [Register] [Value]: "Call if register is EQual to Zero" set the next program address to value and store the current address if the register is equal to zero
- CNEZ [Register] [Value]: "Call if register is Not Equal to Zero" set the next program address to value and store the current address if the register is not equal to zero
- CGTZ [Register] [Value]: "Call if register is Greater Than Zero" set the next program address to value and store the current address if the register is greater than zero
- CLTZ [Register] [Value]: "Call if register is Less Than Zero" set the next program address to value and store the current address if the register is less than zero
- CGEZ [Register] [Value]: "Call if register is Greater than or Equal to Zero" set the next program address to value and store the current address if the register is greater than or equal to zero
- CLEZ [Register] [Value]: "Call if register is Less than or Equal to Zero" set the next program address to value and store the current address if the register is less than or equal to zero
- CREQ [Register 1] [Register 2] [Register 3]: "Call if Registers are EQual" set the next program address to the value of register 3 and store the current address if register 1 and register 2 are equal
- CRNE [Register 1] [Register 2] [Register 3]: "Call if Registers are Not Equal" set the next program address to the value of register 3 and store the current address if register 1 and register 2 are not equal
- CRGT [Register 1] [Register 2] [Register 3]: "Call if Register is Greater Than the other" set the next program address to the value of register 3 and store the current address if register 1 is greater than register 2
- CRLT [Register 1] [Register 2] [Register 3]: "Call if Register is Less Than the other" set the next program address to the value of register 3 and store the current address if register 1 is less than register 2
- CRGE [Register 1] [Register 2] [Register 3]: "Call if Register is Greater than or Equal to the other" set the next program address to the value of register 3 and store the current address if register 1 is greater than or equal to register 2
- CRLE [Register 1] [Register 2] [Register 3]: "Call if Register is Less than or Equal to the other" set the next program address to the value of register 3 and store the current address if register 1 is less than or equal to register 2
- RET: "RETurn" set the next program address to the last stored address

Arithmetics and Logic Operations (18):
- NEG: "NEGation" (made from other operation)
- ADD: "ADDition"
- SUB: "SUBtraction"
- MUL: "MULtiplication"
- DIV: "DIVision"
- MOD: "MODulo"

- NOT: "bitwise NOT" (made from other operation)
- OR: "bitwise OR"
- NOR: "bitwise NOR"
- AND: "bitwise AND"
- NAND: "bitwise NAND"
- XOR: "bitwise XOR"
- XNOR: "bitwise XNOR"

- RAS: "Right Arithmetic Shift"
- LAS: "Left Arithmetic Shift"
- RCS: "Right Circular Shift"
- LCS: "Left Circular Shift"
- RLS: "Right Logical Shift"

Total: 68
