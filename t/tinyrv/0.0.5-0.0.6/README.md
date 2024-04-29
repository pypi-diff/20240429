# Comparing `tmp/tinyrv-0.0.5.tar.gz` & `tmp/tinyrv-0.0.6.tar.gz`

## Comparing `tinyrv-0.0.5.tar` & `tinyrv-0.0.6.tar`

### file list

```diff
@@ -1,11 +1,24 @@
--rw-r--r--   0        0        0    18900 2020-02-02 00:00:00.000000 tinyrv-0.0.5/tinyrv.py
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 tinyrv-0.0.5/tinyrv_opcodes/arg_lut.csv
--rw-r--r--   0        0        0     7855 2020-02-02 00:00:00.000000 tinyrv-0.0.5/tinyrv_opcodes/constants.py
--rw-r--r--   0        0        0     5994 2020-02-02 00:00:00.000000 tinyrv-0.0.5/tinyrv_opcodes/csrs.csv
--rw-r--r--   0        0        0     2690 2020-02-02 00:00:00.000000 tinyrv-0.0.5/tinyrv_opcodes/csrs32.csv
--rw-r--r--   0        0        0   236488 2020-02-02 00:00:00.000000 tinyrv-0.0.5/tinyrv_opcodes/instr_dict.yaml
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 tinyrv-0.0.5/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 tinyrv-0.0.5/LICENSE
--rw-r--r--   0        0        0     8153 2020-02-02 00:00:00.000000 tinyrv-0.0.5/README.md
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 tinyrv-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     8648 2020-02-02 00:00:00.000000 tinyrv-0.0.5/PKG-INFO
+-rwxr-xr-x   0        0        0     3546 2020-02-02 00:00:00.000000 tinyrv-0.0.6/tinyrv_opcodes_gen.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 tinyrv-0.0.6/tests/config.ini
+-rwxr-xr-x   0        0        0      125 2020-02-02 00:00:00.000000 tinyrv-0.0.6/tests/run_riscof.sh
+-rwxr-xr-x   0        0        0      865 2020-02-02 00:00:00.000000 tinyrv-0.0.6/tests/run_riscv_tests.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 tinyrv-0.0.6/tests/sail_cSim/__init__.py
+-rw-r--r--   0        0        0     5238 2020-02-02 00:00:00.000000 tinyrv-0.0.6/tests/sail_cSim/riscof_sail_cSim.py
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 tinyrv-0.0.6/tests/sail_cSim/env/link.ld
+-rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 tinyrv-0.0.6/tests/sail_cSim/env/model_test.h
+-rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 tinyrv-0.0.6/tests/tinyrv/riscof_tinyrv.py
+-rwxr-xr-x   0        0        0      880 2020-02-02 00:00:00.000000 tinyrv-0.0.6/tests/tinyrv/runner.py
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 tinyrv-0.0.6/tests/tinyrv/tinyrv_isa.yaml
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 tinyrv-0.0.6/tests/tinyrv/tinyrv_platform.yaml
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 tinyrv-0.0.6/tests/tinyrv/env/link.ld
+-rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 tinyrv-0.0.6/tests/tinyrv/env/model_test.h
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 tinyrv-0.0.6/tinyrv/__init__.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 tinyrv-0.0.6/tinyrv/dump.py
+-rw-r--r--   0        0        0   391925 2020-02-02 00:00:00.000000 tinyrv-0.0.6/tinyrv/opcodes.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 tinyrv-0.0.6/tinyrv/sim.py
+-rw-r--r--   0        0        0    23962 2020-02-02 00:00:00.000000 tinyrv-0.0.6/tinyrv/tinyrv.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 tinyrv-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 tinyrv-0.0.6/LICENSE
+-rw-r--r--   0        0        0     8583 2020-02-02 00:00:00.000000 tinyrv-0.0.6/README.md
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 tinyrv-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     9078 2020-02-02 00:00:00.000000 tinyrv-0.0.6/PKG-INFO
```

### Comparing `tinyrv-0.0.5/LICENSE` & `tinyrv-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tinyrv-0.0.5/README.md` & `tinyrv-0.0.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 # tinyRV
 
 A RISC-V instruction decoder and instruction set simulator in less than 200 lines of python.
 
+**Mission**: Make the most useful RISC-V disassembler/simulator for understanding the ISA and reverse-engineering binaries with the least amount of easily extendable code. Simulation performance is secondary.
+
 - Uses official RISC-V specs to decode *every* specified RISC-V instruction.
 - Simulates the base ISAs and is easily extendable.
-- RV32IMZicsr_Zifencei and RV64IMZicsr_Zifencei compliance validated using RISCOF (see Testing below).
+- RV32IMAZicsr_Zifencei and RV64IMAZicsr_Zifencei compliance validated using RISCOF (see Testing below).
 
 ## Getting Started
 
 ```sh
 pip install tinyrv
 ```
 
 Print all RISC-V instructions in a binary:
-```py
-from tinyrv import rvprint
-rvprint('firmware.bin', xlen=32)  # xlen just for output formatting
+```
+tinyrv-dump firmware.bin
 ```
 Outputs for `firmware.bin` from [picorv32](https://github.com/YosysHQ/picorv32/tree/main):
 ```
 00000000: custom0                                  # INVALID data=0x800400b
 00000004: custom0                                  # INVALID data=0x600600b
 00000008: jal        zero, 0x3e0                   # rv_i
 0000000c: addi       zero, zero, 0                 # rv_i
@@ -36,60 +37,63 @@
 00000038: sw         gp, 12(ra)                    # rv_i
 0000003c: sw         tp, 16(ra)                    # rv_i
 ...
 ```
 picorv32 uses some custom instructions for IRQ handling.
 
 Decode instructions from data:
+```
+tinyrv-dump 0xf2410113 0xde0ec086 0x2013b7
+```
+or in python:
 ```py
-from tinyrv import rvdecoder
-for op in rvdecoder(0xf2410113, 0xde0ec086, 0x2013b7):
+import tinyrv
+for op in tinyrv.rvdecoder(0xf2410113, 0xde0ec086, 0x2013b7):
     print(op)
 ```
 Outputs four instructions (the second word contains actually two 16-bit compressed instructions):
 ```
 addi       sp, sp, -220
 c.swsp     ra, uimm8sp_s=64
 c.swsp     gp, uimm8sp_s=60
 lui        t2, 0x201000
 ```
 Each decoded instruction comes with a lot of metadata and parsed arguments:
 ```py
-op = next(rvdecoder(0xf2410113))
-print(hex(op.data), op.name, op.extension, op.encoding, op.variable_fields, op.valid())
+op = tinyrv.rvdecode(0xf2410113)
+print(hex(op.data), op.name, op.extension, op.variable_fields, bin(op.mask), bin(op.match), op.valid())
 print(op.args, op.rd, op.rs1, op.imm12)
 print(op.arg_str())
 ```
 ```
-0xf2410113 addi ['rv_i'] -----------------000-----0010011 ['rd', 'rs1', 'imm12'] True
+0xf2410113 addi ['rv_i'] ['rd', 'rs1', 'imm12'] 0b111000001111111 0b10011 True
 {'rd': 2, 'rs1': 2, 'imm12': -220} 2 2 -220
 sp, sp, -220
 ```
 Simulate a binary:
 ```py
-from tinyrv import rvmem, rvsim
-mem = rvmem(xlen=32)  # xlen just for output formatting
-mem.load('firmware.bin', base=0)
-rv = rvsim(mem, xlen=32)  # xlen affects overflows, sign extensions
+rv = tinyrv.rvsim(xlen=32)  # xlen affects overflows, sign extensions
+rv.read_bin('firmware.bin', base=0)
 print(rv)  # print registers
 print()
-rv.run(10)  # simulate up to 10 instructions
+rv.step()  # simulate a single instruction at rv.pc
 ```
 Outputs:
 ```
 x00(ro)=00000000  x08(fp)=00000000  x16(a6)=00000000  x24(s8)=00000000
 x01(ra)=00000000  x09(s1)=00000000  x17(a7)=00000000  x25(s9)=00000000
 x02(sp)=00000000  x10(a0)=00000000  x18(s2)=00000000  x26(10)=00000000
 x03(gp)=00000000  x11(a1)=00000000  x19(s3)=00000000  x27(11)=00000000
 x04(tp)=00000000  x12(a2)=00000000  x20(s4)=00000000  x28(t3)=00000000
 x05(t0)=00000000  x13(a3)=00000000  x21(s5)=00000000  x29(t4)=00000000
 x06(t1)=00000000  x14(a4)=00000000  x22(s6)=00000000  x30(t5)=00000000
 x07(t2)=00000000  x15(a5)=00000000  x23(s7)=00000000  x31(t6)=00000000
 
-vvvvvvvv: unknown opcode: 0800400b
+
+00000000: unimplemented: 0800400b custom0    
 00000000: custom0                                  #
 ```
 Simulation halts at the first instruction that is not implemented. Just set the pc and carry on:
 ```py
 rv.pc = 8
 rv.run(50)
 ```
@@ -122,54 +126,67 @@
 00000b18: addi       a0, a0, 1                     # a0=0000c79e
 00000b1c: sw         a5, 0(a4)                     # 00000065->mem[10000000]
 00000b20: jal        zero, 0xb0c                   # 
 
 00000b0c: lbu        a5, 0(a0)                     # mem[0000c79e]->6c a5=0000006c
 00000b10: bne        a5, zero, 0xb18               # 
 ```
-Each jump, taken branch produces a newline, right-hand side has register changes and memory transactions. `rvmem` is paged. Memory is allocated on demand and persists. Now let's get past this loop by setting a breakpoint:
+Each jump, taken branch produces a newline, right-hand side has register changes and memory transactions. Memory is paged, allocated on demand and persists. Now let's get past this loop by setting a breakpoint:
 ```py
 rv.run(1000, bpts={0xb14})
 rv.run(10)
 ```
 ```
 ...
+00000b1c: sw         a5, 0(a4)                     # 00000064->mem[10000000]
+00000b20: jal        zero, 0xb0c                   # 
+
 00000b0c: lbu        a5, 0(a0)                     # mem[0000c7a7]->0a a5=0000000a
 00000b10: bne        a5, zero, 0xb18               # 
 
 00000b18: addi       a0, a0, 1                     # a0=0000c7a8
 00000b1c: sw         a5, 0(a4)                     # 0000000a->mem[10000000]
 00000b20: jal        zero, 0xb0c                   # 
 
 00000b0c: lbu        a5, 0(a0)                     # mem[0000c7a8]->00 a5=00000000
 00000b10: bne        a5, zero, 0xb18               # 
 00000b14: jalr       zero, 0(ra)                   # 
 
 00000464: addi       ra, zero, 0x3e8               # ra=000003e8
 
-vvvvvvvv: unknown opcode: 0a00e00b
-00000468: custom0                                  #
+00000468: unimplemented: 0a00e00b custom0    
+00000468: custom0                                  # 
+```
+Simulate from command line:
+```
+# usage: tinyrv-sim file.bin [(32|64) [run limit in decimal [start PC in hex]]]
+
+tinyrv-sim firmware.bin 32 100 8
 ```
 
+
 ## Dev Setup
 
-All code is in `tinyrv.py`.
-No dependencies, except [pyyaml](https://pypi.org/project/PyYAML/).
-However, tinyRV needs to load opcode specs from [riscv-opcodes](https://github.com/riscv/riscv-opcodes).
-Do this:
+All code is in `tinyrv/tinyrv.py` and has no external dependencies.
+tinyRV loads opcode specs from `tinyrv/opcodes.py`, which is auto-generated by `tinyrv_opcodes_gen.py` from [riscv-opcodes](https://github.com/riscv/riscv-opcodes).
+
+Do this to re-generate:
 ```sh
-git clone https://github.com/riscv/riscv-opcodes.git tinyrv_opcodes
-cd tinyrv_opcodes; make
+git clone https://github.com/riscv/riscv-opcodes.git
+make -C riscv-opcodes
+python3 tinyrv_opcodes_gen.py
 ```
-The necessary opcode specs are also bundled in the PyPI package. If there is a `tinyrv_opcodes` in the current directory, tinyRV will try to use those instead of the packaged ones.
+
 
 ## Testing
 
 Install [riscv-gnu-toolchain](https://github.com/riscv/riscv-gnu-toolchain) or [homebrew-riscv](https://github.com/riscv-software-src/homebrew-riscv) (for MacOS).
 
+### RISCOF
+
 Install [the RISC-V compatibility framework RISCOF](https://github.com/riscv-software-src/riscof):
 ```sh
 pip3 install setuptools wheel
 git clone https://github.com/riscv/riscof.git
 cd riscof
 pip3 install -e .
 ```
@@ -203,14 +220,28 @@
 make install
 spike  # test
 ```
 Then, run the tests:
 ```sh
 cd tests
 riscof --verbose info arch-test --clone
-riscof run --config=config.ini --suite=riscv-arch-test/riscv-test-suite/ --env=riscv-arch-test/riscv-test-suite/env
+./run_riscof.sh
+```
+
+### riscv-software-src/riscv-tests
+
+```sh
+cd tests
+git clone https://github.com/riscv/riscv-tests
+cd riscv-tests
+git submodule update --init --recursive
+autoconf
+./configure
+make
+cd ..
+./run_riscv_tests.py
 ```
 
 ## Related
 
 - [TinyFive](https://github.com/OpenMachine-ai/tinyfive)
 - [mini-rv32ima](https://github.com/cnlohr/mini-rv32ima)
```

### Comparing `tinyrv-0.0.5/PKG-INFO` & `tinyrv-0.0.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: tinyrv
-Version: 0.0.5
+Version: 0.0.6
 Summary: A tiny RISC-V instruction set simulator
 Project-URL: Homepage, https://github.com/s-holst/tinyrv
 Project-URL: Issues, https://github.com/s-holst/tinyrv/issues
 Author-email: Stefan Holst <mail@s-holst.de>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,28 +12,29 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # tinyRV
 
 A RISC-V instruction decoder and instruction set simulator in less than 200 lines of python.
 
+**Mission**: Make the most useful RISC-V disassembler/simulator for understanding the ISA and reverse-engineering binaries with the least amount of easily extendable code. Simulation performance is secondary.
+
 - Uses official RISC-V specs to decode *every* specified RISC-V instruction.
 - Simulates the base ISAs and is easily extendable.
-- RV32IMZicsr_Zifencei and RV64IMZicsr_Zifencei compliance validated using RISCOF (see Testing below).
+- RV32IMAZicsr_Zifencei and RV64IMAZicsr_Zifencei compliance validated using RISCOF (see Testing below).
 
 ## Getting Started
 
 ```sh
 pip install tinyrv
 ```
 
 Print all RISC-V instructions in a binary:
-```py
-from tinyrv import rvprint
-rvprint('firmware.bin', xlen=32)  # xlen just for output formatting
+```
+tinyrv-dump firmware.bin
 ```
 Outputs for `firmware.bin` from [picorv32](https://github.com/YosysHQ/picorv32/tree/main):
 ```
 00000000: custom0                                  # INVALID data=0x800400b
 00000004: custom0                                  # INVALID data=0x600600b
 00000008: jal        zero, 0x3e0                   # rv_i
 0000000c: addi       zero, zero, 0                 # rv_i
@@ -50,60 +51,63 @@
 00000038: sw         gp, 12(ra)                    # rv_i
 0000003c: sw         tp, 16(ra)                    # rv_i
 ...
 ```
 picorv32 uses some custom instructions for IRQ handling.
 
 Decode instructions from data:
+```
+tinyrv-dump 0xf2410113 0xde0ec086 0x2013b7
+```
+or in python:
 ```py
-from tinyrv import rvdecoder
-for op in rvdecoder(0xf2410113, 0xde0ec086, 0x2013b7):
+import tinyrv
+for op in tinyrv.rvdecoder(0xf2410113, 0xde0ec086, 0x2013b7):
     print(op)
 ```
 Outputs four instructions (the second word contains actually two 16-bit compressed instructions):
 ```
 addi       sp, sp, -220
 c.swsp     ra, uimm8sp_s=64
 c.swsp     gp, uimm8sp_s=60
 lui        t2, 0x201000
 ```
 Each decoded instruction comes with a lot of metadata and parsed arguments:
 ```py
-op = next(rvdecoder(0xf2410113))
-print(hex(op.data), op.name, op.extension, op.encoding, op.variable_fields, op.valid())
+op = tinyrv.rvdecode(0xf2410113)
+print(hex(op.data), op.name, op.extension, op.variable_fields, bin(op.mask), bin(op.match), op.valid())
 print(op.args, op.rd, op.rs1, op.imm12)
 print(op.arg_str())
 ```
 ```
-0xf2410113 addi ['rv_i'] -----------------000-----0010011 ['rd', 'rs1', 'imm12'] True
+0xf2410113 addi ['rv_i'] ['rd', 'rs1', 'imm12'] 0b111000001111111 0b10011 True
 {'rd': 2, 'rs1': 2, 'imm12': -220} 2 2 -220
 sp, sp, -220
 ```
 Simulate a binary:
 ```py
-from tinyrv import rvmem, rvsim
-mem = rvmem(xlen=32)  # xlen just for output formatting
-mem.load('firmware.bin', base=0)
-rv = rvsim(mem, xlen=32)  # xlen affects overflows, sign extensions
+rv = tinyrv.rvsim(xlen=32)  # xlen affects overflows, sign extensions
+rv.read_bin('firmware.bin', base=0)
 print(rv)  # print registers
 print()
-rv.run(10)  # simulate up to 10 instructions
+rv.step()  # simulate a single instruction at rv.pc
 ```
 Outputs:
 ```
 x00(ro)=00000000  x08(fp)=00000000  x16(a6)=00000000  x24(s8)=00000000
 x01(ra)=00000000  x09(s1)=00000000  x17(a7)=00000000  x25(s9)=00000000
 x02(sp)=00000000  x10(a0)=00000000  x18(s2)=00000000  x26(10)=00000000
 x03(gp)=00000000  x11(a1)=00000000  x19(s3)=00000000  x27(11)=00000000
 x04(tp)=00000000  x12(a2)=00000000  x20(s4)=00000000  x28(t3)=00000000
 x05(t0)=00000000  x13(a3)=00000000  x21(s5)=00000000  x29(t4)=00000000
 x06(t1)=00000000  x14(a4)=00000000  x22(s6)=00000000  x30(t5)=00000000
 x07(t2)=00000000  x15(a5)=00000000  x23(s7)=00000000  x31(t6)=00000000
 
-vvvvvvvv: unknown opcode: 0800400b
+
+00000000: unimplemented: 0800400b custom0    
 00000000: custom0                                  #
 ```
 Simulation halts at the first instruction that is not implemented. Just set the pc and carry on:
 ```py
 rv.pc = 8
 rv.run(50)
 ```
@@ -136,54 +140,67 @@
 00000b18: addi       a0, a0, 1                     # a0=0000c79e
 00000b1c: sw         a5, 0(a4)                     # 00000065->mem[10000000]
 00000b20: jal        zero, 0xb0c                   # 
 
 00000b0c: lbu        a5, 0(a0)                     # mem[0000c79e]->6c a5=0000006c
 00000b10: bne        a5, zero, 0xb18               # 
 ```
-Each jump, taken branch produces a newline, right-hand side has register changes and memory transactions. `rvmem` is paged. Memory is allocated on demand and persists. Now let's get past this loop by setting a breakpoint:
+Each jump, taken branch produces a newline, right-hand side has register changes and memory transactions. Memory is paged, allocated on demand and persists. Now let's get past this loop by setting a breakpoint:
 ```py
 rv.run(1000, bpts={0xb14})
 rv.run(10)
 ```
 ```
 ...
+00000b1c: sw         a5, 0(a4)                     # 00000064->mem[10000000]
+00000b20: jal        zero, 0xb0c                   # 
+
 00000b0c: lbu        a5, 0(a0)                     # mem[0000c7a7]->0a a5=0000000a
 00000b10: bne        a5, zero, 0xb18               # 
 
 00000b18: addi       a0, a0, 1                     # a0=0000c7a8
 00000b1c: sw         a5, 0(a4)                     # 0000000a->mem[10000000]
 00000b20: jal        zero, 0xb0c                   # 
 
 00000b0c: lbu        a5, 0(a0)                     # mem[0000c7a8]->00 a5=00000000
 00000b10: bne        a5, zero, 0xb18               # 
 00000b14: jalr       zero, 0(ra)                   # 
 
 00000464: addi       ra, zero, 0x3e8               # ra=000003e8
 
-vvvvvvvv: unknown opcode: 0a00e00b
-00000468: custom0                                  #
+00000468: unimplemented: 0a00e00b custom0    
+00000468: custom0                                  # 
+```
+Simulate from command line:
+```
+# usage: tinyrv-sim file.bin [(32|64) [run limit in decimal [start PC in hex]]]
+
+tinyrv-sim firmware.bin 32 100 8
 ```
 
+
 ## Dev Setup
 
-All code is in `tinyrv.py`.
-No dependencies, except [pyyaml](https://pypi.org/project/PyYAML/).
-However, tinyRV needs to load opcode specs from [riscv-opcodes](https://github.com/riscv/riscv-opcodes).
-Do this:
+All code is in `tinyrv/tinyrv.py` and has no external dependencies.
+tinyRV loads opcode specs from `tinyrv/opcodes.py`, which is auto-generated by `tinyrv_opcodes_gen.py` from [riscv-opcodes](https://github.com/riscv/riscv-opcodes).
+
+Do this to re-generate:
 ```sh
-git clone https://github.com/riscv/riscv-opcodes.git tinyrv_opcodes
-cd tinyrv_opcodes; make
+git clone https://github.com/riscv/riscv-opcodes.git
+make -C riscv-opcodes
+python3 tinyrv_opcodes_gen.py
 ```
-The necessary opcode specs are also bundled in the PyPI package. If there is a `tinyrv_opcodes` in the current directory, tinyRV will try to use those instead of the packaged ones.
+
 
 ## Testing
 
 Install [riscv-gnu-toolchain](https://github.com/riscv/riscv-gnu-toolchain) or [homebrew-riscv](https://github.com/riscv-software-src/homebrew-riscv) (for MacOS).
 
+### RISCOF
+
 Install [the RISC-V compatibility framework RISCOF](https://github.com/riscv-software-src/riscof):
 ```sh
 pip3 install setuptools wheel
 git clone https://github.com/riscv/riscof.git
 cd riscof
 pip3 install -e .
 ```
@@ -217,14 +234,28 @@
 make install
 spike  # test
 ```
 Then, run the tests:
 ```sh
 cd tests
 riscof --verbose info arch-test --clone
-riscof run --config=config.ini --suite=riscv-arch-test/riscv-test-suite/ --env=riscv-arch-test/riscv-test-suite/env
+./run_riscof.sh
+```
+
+### riscv-software-src/riscv-tests
+
+```sh
+cd tests
+git clone https://github.com/riscv/riscv-tests
+cd riscv-tests
+git submodule update --init --recursive
+autoconf
+./configure
+make
+cd ..
+./run_riscv_tests.py
 ```
 
 ## Related
 
 - [TinyFive](https://github.com/OpenMachine-ai/tinyfive)
 - [mini-rv32ima](https://github.com/cnlohr/mini-rv32ima)
```

