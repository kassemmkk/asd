# RV32I ALU IP REQUIREMENTS QUESTIONNAIRE

**Instructions:** Please fill out all sections below by replacing the blank lines with your specific requirements. Open this file in VS Code to complete it, then notify me when finished.

## 1. Functional Requirements
**Primary Function:** RV32I Arithmetic Logic Unit (ALU)
**Detailed Description:** _______________
**Key Features Required:**
- [ ] Integer arithmetic operations (ADD, SUB)
- [ ] Logical operations (AND, OR, XOR)
- [ ] Shift operations (SLL, SRL, SRA)
- [ ] Comparison operations (SLT, SLTU)
- [ ] Additional operations: _______________

## 2. Technical Specifications
**Target Technology:** [ ] FPGA [ ] ASIC [X] Generic
**Clock Frequency:** _____ MHz
**Interface Type:** [ ] AXI [ ] APB [ ] AHB [X] Custom: Simple combinational/registered
**Data Width:** 32 bits (RV32I standard)
**Operation Width:** _____ bits (ALU operation encoding)

## 3. RV32I Specific Requirements
**Supported Instructions:**
- [ ] ADD/ADDI (Addition)
- [ ] SUB (Subtraction) 
- [ ] AND/ANDI (Bitwise AND)
- [ ] OR/ORI (Bitwise OR)
- [ ] XOR/XORI (Bitwise XOR)
- [ ] SLL/SLLI (Shift Left Logical)
- [ ] SRL/SRLI (Shift Right Logical)
- [ ] SRA/SRAI (Shift Right Arithmetic)
- [ ] SLT/SLTI (Set Less Than)
- [ ] SLTU/SLTIU (Set Less Than Unsigned)
- [ ] LUI (Load Upper Immediate) - if handled in ALU
- [ ] AUIPC (Add Upper Immediate to PC) - if handled in ALU

**ALU Control Encoding:**
**Control Signal Width:** _____ bits
**Preferred Encoding Style:** [ ] Binary [ ] One-hot [ ] Custom: _____

## 4. Performance Requirements
**Critical Path Target:** _____ ns
**Pipeline Stages:** [ ] Combinational only [ ] 1-stage [ ] 2-stage [ ] Custom: _____
**Throughput:** [ ] 1 operation/cycle [ ] Custom: _____

## 5. Interface Requirements
**Input Ports:**
- operand_a [31:0] - First operand
- operand_b [31:0] - Second operand  
- alu_op [X:0] - ALU operation select
- Additional inputs: _______________

**Output Ports:**
- result [31:0] - ALU result
- zero_flag - Result is zero
- Additional flags: _______________
- Additional outputs: _______________

## 6. Verification Requirements
**Coverage Target:** _____%
**Number of Sprints:** _____ (recommended: 3-4)
**Priority:** [ ] Performance [ ] Area [ ] Power [X] Features
**Test Strategy:**
- [ ] Directed tests for each operation
- [ ] Random instruction testing
- [ ] Corner case testing (overflow, underflow)
- [ ] Compliance with RISC-V specification
- [ ] Custom: _____

## 7. Integration Requirements
**CPU Integration:**
- [ ] Standalone ALU module
- [ ] Part of execution unit
- [ ] Custom integration: _____

**Timing Requirements:**
- [ ] Combinational (no clock)
- [ ] Single-cycle (registered outputs)
- [ ] Multi-cycle: _____ cycles
- [ ] Pipeline: _____ stages

## 8. Additional Features
**Error Handling:**
- [ ] Overflow detection
- [ ] Underflow detection
- [ ] Division by zero (if division supported)
- [ ] Custom: _____

**Debug Features:**
- [ ] Operation tracing
- [ ] Internal state visibility
- [ ] Custom: _____

## 9. Constraints
**Area Constraints:** _______________
**Power Constraints:** _______________
**Timing Constraints:** _______________
**Technology Constraints:** _______________

## 10. Sprint Planning Preferences
**Sprint 1 Focus:** [ ] Basic arithmetic (ADD/SUB) [ ] Core logical ops [ ] Custom: _____
**Sprint 2 Focus:** [ ] Shift operations [ ] Comparison ops [ ] Custom: _____
**Sprint 3 Focus:** [ ] Advanced features [ ] Optimization [ ] Custom: _____
**Sprint 4 Focus:** [ ] Integration features [ ] Performance tuning [ ] Custom: _____

---
**Please fill out all sections above and notify me when complete. I will then proceed with the agile IP development process.**