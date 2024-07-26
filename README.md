# Instruction List

Data Logistics:
- CPY [Register 1] [Register 2] [Register 3]: "CoPY" write the value of register 1 into register 2 and register 3
- SWP [Register 1] [Register 2]: "SWaP" write the value of register 1 into register 2 and write the value of register 2 into register 1 at the same time
- STLS [Value] [Register]: "SeT Least Significant bits" write the value to the lower half of the register
- STMS [Value] [Register]: "SeT Most Significant bits" write the value to the upper half of the register

Memory Address Manipulations:
- BRCH [Value]: "BRanCH" set the next program address to value
- BEQZ [Register] [Value]: "Branch if register is EQual to Zero" set the next program address to value if the register is equal to zero
- BNEZ [Register] [Value]: "Branch if register is Not Equal to Zero" set the next program address to value if the register is not equal to zero
- BGTZ [Register] [Value]: "Branch if register is Greater Than Zero" set the next program address to value if the register is greater than zero
- BLTZ [Register] [Value]: "Branch if register is Less Than Zero" set the next program address to value if the register is less than zero
- BGEZ [Register] [Value]: "Branch if register is Greater than or Equal to Zero" set the next program address to value if the register is greater than or equal to zero
- BLEZ [Register] [Value]: "Branch if register is Less than or Equal to Zero" set the next program address to value if the register is less than or equal to zero
- BREQ [Register 1] [Register 2] [Register 3]: "Branch if Register are EQual" set the next program address to the value of register 3 if register 1 and register 2 are equal
- BRNE [Register 1] [Register 2] [Register 3]: "Branch if Register are Not Equal" set the next program address to the value of register 3 if register 1 and register 2 are not equal
- BRGT [Register 1] [Register 2] [Register 3]: "Branch if Register are Greater Than" set the next program address to the value of register 3 if register 1 is greater than register 2
- BRLT [Register 1] [Register 2] [Register 3]: "Branch if Register are Less Than" set the next program address to the value of register 3 if register 1 is less than register 2
- BRGE [Register 1] [Register 2] [Register 3]: "Branch if Register are Greater than or Equal" set the next program address to the value of register 3 if register 1 is greater than or equal to register 2
- BRLE [Register 1] [Register 2] [Register 3]: "Branch if Register are Less than or Equal" set the next program address to the value of register 3 if register 1 is less than or equal to register 2

- JMP [Value]: "JuMP" set the next program address to the sum of the current program address and value
- JEQZ [Register] [Value]: "Jump if register is EQual to Zero" set the next program address to the sum of the current program address and value if the register is equal to zero
- JNEZ [Register] [Value]: "Jump if register is Not Equal to Zero" set the next program address to the sum of the current program address and value if the register is not equal to zero
- JGTZ [Register] [Value]: "Jump if register is Greater Than Zero" set the next program address to the sum of the current program address and value if the register is greater than zero
- JLTZ [Register] [Value]: "Jump if register is Less Than Zero" set the next program address to the sum of the current program address and value if the register is less than zero
- JGEZ [Register] [Value]: "Jump if register is Greater than or Equal to Zero" set the next program address to the sum of the current program address and value if the register is greater than or equal to zero
- JLEZ [Register] [Value]: "Jump if register is Less than or Equal to Zero" set the next program address to the sum of the current program address and value if the register is less than or equal to zero

- CALL [Value]: "CALL" set the next program address to value and store the current address
- CEQZ [Register] [Value]: "Call if register is EQual to Zero" set the next program address to value and store the current address if the register is equal to zero
- CNEZ [Register] [Value]: "Call if register is Not Equal to Zero" set the next program address to value and store the current address if the register is not equal to zero
- CGTZ [Register] [Value]: "Call if register is Greater Than Zero" set the next program address to value and store the current address if the register is greater than zero
- CLTZ [Register] [Value]: "Call if register is Less Than Zero" set the next program address to value and store the current address if the register is less than zero
- CGEZ [Register] [Value]: "Call if register is Greater than or Equal to Zero" set the next program address to value and store the current address if the register is greater than or equal to zero
- CLEZ [Register] [Value]: "Call if register is Less than or Equal to Zero" set the next program address to value and store the current address if the register is less than or equal to zero
- RET: "RETurn" set the next program address to the last stored address

Arithmetics and Logic Operations:
- NEG: "NEGation"
- ADD: "ADDition"
- SUB: "SUBtraction"
- MUL: "MULtiplication"
- DIV: "DIVision"
- MOD: "MODulo"

- NOT: "bitwise NOT"
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
