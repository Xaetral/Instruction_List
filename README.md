# Instruction List

Data Logistics:
- CPY [Register 1] [Register 2]: "CoPY" write the value of register 1 into register 2
- SWP [Register 1] [Register 2]: "SWaP" write the value of register 1 into register 2 and write the value of register 2 into register 1 at the same time
- STLS: "SeT Least Significant bits"
- STMS: "SeT Most Significant bits"

Memory Address Manipulations:
- BRCH [Value]: "BRanCH" set the next program address to value
- BEQZ [Register] [Value]: "Branch if register is EQual to Zero" set the next program address to value if the register is equal to zero
- BNEZ [Register] [Value]: "Branch if register is Not Equal to Zero" set the next program address to value if the register is not equal to zero
- BGTZ [Register] [Value]: "Branch if register is Greater Than Zero" set the next program address to value if the register is greater than zero
- BLTZ [Register] [Value]: "Branch if register is Less Than Zero" set the next program address to value if the register is less than zero
- BGEZ [Register] [Value]: "Branch if register is Greater than or Equal to Zero" set the next program address to value if the register is greater than or equal to zero
- BLEZ [Register] [Value]: "Branch if register is Less than or Equal to Zero" set the next program address to value if the register is less than or equal to zero

- JMP [Value]: "JuMP" set the next program address to the sum of the current program address and value
- JEQZ [Register] [Value]: "Jump if register is EQual to Zero" set the next program address to the sum of the current program address and value if the register is equal to zero
- JNEZ [Register] [Value]: "Jump if register is Not Equal to Zero" set the next program address to the sum of the current program address and value if the register is not equal to zero
- JGTZ [Register] [Value]: "Jump if register is Greater Than Zero" set the next program address to the sum of the current program address and value if the register is greater than zero
- JLTZ [Register] [Value]: "Jump if register is Less Than Zero" set the next program address to the sum of the current program address and value if the register is less than zero
- JGEZ [Register] [Value]: "Jump if register is Greater than or Equal to Zero" set the next program address to the sum of the current program address and value if the register is greater than or equal to zero
- JLEZ [Register] [Value]: "Jump if register is Less than or Equal to Zero" set the next program address to the sum of the current program address and value if the register is less than or equal to zero

- CALL [Value]: "CALL"
- CEQZ [Register] [Value]: "Call if register is EQual to Zero" set the next program address to value if the register is equal to zero
- CNEZ [Register] [Value]: "Call if register is Not Equal to Zero" set the next program address to value if the register is not equal to zero
- CGTZ [Register] [Value]: "Call if register is Greater Than Zero" set the next program address to value if the register is greater than zero
- CLTZ [Register] [Value]: "Call if register is Less Than Zero" set the next program address to value if the register is less than zero
- CGEZ [Register] [Value]: "Call if register is Greater than or Equal to Zero" set the next program address to value if the register is greater than or equal to zero
- CLEZ [Register] [Value]: "Call if register is Less than or Equal to Zero" set the next program address to value if the register is less than or equal to zero
- RET: "RETurn"
