# Instruction Set Architecture

- ISA is abstract computer model, an interface between software and hardware.
- ISA defines all operations a CPU can perform.
- ISA by complexity: RISC and CISC; also VLIW, LIW, EPIC.


ISA defines:
* states:
  - registers
  - cache
  - main memory
* data types:
  - 6-bit, 16-bit, 32-bit
  - word
  - quadword
* instructions
  - mnemonics
  - translations
  - assembly
* memory consistency
* memory addressing modes
  - immediate
  - relative
  - absolute
* IO model

---

Instruction Set Architecture (ISA) is abstract computer model, interfacing between software and hardware; also regarded as a programmer's view of the machine. A realization of a particular ISA is called an implementation.

An ISA defines everything a machine language programmer needs to know in order to author programs for a computer that implements that ISA. In theory, such programs can then run on different computers provided they all implement that same ISA. This has provided *binary compatibility* across different generations of CPUs and the concept of computer families. For example, you can run a program intended for Intel's 8086 CPU on a modern one since they both implement the x86 instruction set (with the latter implementing the extended, but backwards compatible, x86_64 ISA).

ISA defines:
- Instruction set: machine instructions comprising computer's machine language
- Supported data types, in terms of bit-size: 8-bit, 16-bit, 32-bit, etc.
- Available states: registers, caches, main memory
- State semantics: memory consistency, addressing modes
- IO model


ISA defines *instructions* and their encoding (binary, in most cases) and related entities such as *data types*, *registers*, *addressing modes* and *memory access*. Instructions refer to these entities using register indices and memory addressing modes. ISA also defines short mnemonic names, *mnemonics*, for each available instruction; e.g. MULQ might refer to the multiplication of quad-sized, i.e. 64 bits, integers.



Mnemonics are recognized by an **assembler**, which is a program that translates a user-friendly form of an ISA, called **assembly**, into machine code. **Disassemblers** perform the reverse process, taking machine code (executable) and turning it into an assembly.


Classification by Architectural complexity: RISC and CISC.

**Complex Instruction Set Computer** (CISC) is driven by enhancement. It packs the lot including many specialized (possibly infrequently used) instructions; if an operation can be made more optimal by providing a dedicated instruction, it will usually make its way into the ISA.

**Reduced Instruction Set Computer** (RISC) is driven by ease of implementation. It simplifies the CPU by implementing only the basic instructions.

Other architectures include:
- **VLIW** Very long instruction word
- **LIW**  Long instruction word
- **EPIC** Explicitly parallel instruction computing
- **MISC** Minimal instruction set computer
- **OISC** One instruction set computer

The former 3 architectures aim to exploit instruction-level parallelism, thus reducing hardware, by having the compiler issue instructions and perform scheduling. The latter two aim to decrease complexity even further then RISC.



---

https://www.wikiwand.com/en/Instruction_set_architecture
https://www.wikiwand.com/en/Reduced_instruction_set_computer
https://www.wikiwand.com/en/Minimal_instruction_set_computer
https://www.wikiwand.com/en/One_instruction_set_computer

https://www.wikiwand.com/en/Von_Neumann_architecture
