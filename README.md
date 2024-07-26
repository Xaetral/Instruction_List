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

- BVAB [Value] (alias JMP): "Branch from Value, ABsolute" jump to the address equal to value
- BVRO [Value] (alias JRO): "Branch from Value, Relative to Origin" jump to the address equal to the current address plus value
- BVEQ (alias JEQ): "Branch if the Value is EQual"
- BVNE (alias JNE):
- BVGT (alias JGT):
- BVLT (alias JLT):
- BVGE (alias JGE):
- BVLE (alias JLE):
- BRAB:
- BRRO:
- BREQ:
- BRNE:
- BRGT:
- BRLT:
- BRGE:
- BRLE:
