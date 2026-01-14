## List of awesome OLLVM

- [obfuscator](#obfuscator)
- [Hikari](#Hikari)
- [Pluto](#Pluto)
- [goron](#goron)
- [Arkari](#Arkari)
- [O-MVLL](#O-MVLL)
- [VMP](#VMP)

### Obfuscator

[https://github.com/obfuscator-llvm/obfuscator](https://github.com/obfuscator-llvm/obfuscator)

The earliest public Obfuscator-LLVM implementation, supports LLVM 3.3~4.0. Features:
* Instructions Substitution 
* Bogus Control Flow
* Control Flow Flattening 

### Hikari

[https://github.com/HikariObfuscator/Hikari](https://github.com/HikariObfuscator/Hikari)

Hikari, supports LLVM 6~8. Features(in addtion to Obfuscator):
* Anti Class Dump
* Function Call Obfuscate
* Function Wrapper
* Indirect Branching
* Split Basic Block
* String Encryption

~~[https://github.com/61bcdefg/Hikari-LLVM15](https://github.com/61bcdefg/Hikari-LLVM15)~~

Hikari-LLVM15, based on Hikari, supports LLVM 15~19, currently closed-source. Features(in addtion to Hikari):
* Anti Debugging
* Anti Hook
* Constant Encryption

### goron

[https://github.com/amimo/goron](https://github.com/amimo/goron)

goron, supports LLVM 7~10. Features(in addtion to Obfuscator):
* Indirect Branch
* Indirect Call
* Indirect GlobalVariable

[https://github.com/KomiMoe/Arkari](https://github.com/KomiMoe/Arkari)

Arkari, based on goron, supports LLVM 14~newest.

⚠️ **Note: Goron-style (Goron/Arkari) indirect-related obfuscation can be easily deobfuscated by setting the data segment as read-only.**

### Pluto

~~[https://github.com/bluesadi/Pluto](https://github.com/bluesadi/Pluto)~~

Pluto, supports LLVM 14, currently closed-source. Features(in addtion to Obfuscator):
* MBA Obfuscation
* Random ControlFlow
* Split Basic Block
* Trap Angr

[https://github.com/za233/Polaris-Obfuscator](https://github.com/za233/Polaris-Obfuscator)

Polaris (formerly Pluto), supports LLVM16. Features(in addtion to Obfuscator):
* Alias Access
* Indirect Branch
* Indirect Call
* String Encryption
* Merge Function
* Linear MBA
* Dirty Bytes Insertion (MIR level)
* Function Splitting (MIR level)
* Junk Instruction Insertion (MIR level)
* Instruction Substitution (MIR level)

### O-MVLL

* [https://github.com/open-obfuscator/o-mvll](https://github.com/open-obfuscator/o-mvll)

O-MVLL is a LLVM-based obfuscator driven by Python and the LLVM pass manager. Features(in addtion to Obfuscator):
* Anti Hooking
* Arithmetic Obfuscation (MBA Obfuscation)
* Basic Block Duplicate
* Control Flow Breaking
* Function Outline (Function Wrapper)
* Indirect Branch
* Indirect Call
* Opaque Constants (Constant Encryption)

### VMP

* [https://github.com/NiTianErXing666/SmallVmp](https://github.com/NiTianErXing666/SmallVmp)
* [https://github.com/25077667/VMPilot](https://github.com/25077667/VMPilot)
* [https://github.com/GANGE666/xVMP](https://github.com/GANGE666/xVMP)

## List of awesome IDA deobfuscation plugins

- [AI](#AI)
- [Ctree](#Ctree)
- [Decryption](#Decryption)
- [Lifting](#Lifting)
- [MBA](#MBA)
- [Microcode](#Microcode)
- [OLLVM](#OLLVM)
- [VMP](#VMP)

### AI

* [aiDAPal](https://github.com/atredispartners/aidapal). Use a locally running LLM that has been fine-tuned for Hex-Rays pseudocode to assist with code analysis.
* [Gepetto](https://github.com/JusticeRage/Gepetto). Query language models to speed up reverse-engineering.
* [ida-pro-mcp](https://github.com/mrexodia/ida-pro-mcp). AI-powered reverse engineering assistant that bridges IDA Pro with language models through MCP. 
* [WPeChatGPT](https://github.com/WPeace-HcH/WPeChatGPT). Analyze binary file, based on commonly used AI big models such as OpenAI and DeepSeek.

### Ctree

* [herast](https://github.com/Mizari/herast). Framework to automate working with AST in IDA Pro.
* [HexRaysCodeXplorer](https://github.com/REhints/HexRaysCodeXplorer). Hex-Rays Decompiler plugin for better code navigation.
* [HexraysToolbox](https://github.com/patois/HexraysToolbox). Find code patterns within the Hexrays ctree.
* [HrDevHelper](https://github.com/patois/HRDevHelper). HexRays ctree visualization plugin.
* [strikeout](https://github.com/allthingsida/strikeout). A Hex-Rays decompiler plugin to patch the Ctree.

Other useful repositories:
* [GhidraMCP](https://github.com/LaurieWired/GhidraMCP). MCP Server for Ghidra.
* [LLM4Decompile](https://github.com/albertan017/LLM4Decompile). Reverse Engineering: Decompiling Binary Code with Large Language Models.

### Decryption

* [AntiXorstr](https://github.com/lstaroth/AntiXorstr). This plugin is used to recover Xorstr.
* [xorstr-decrypt](https://github.com/yubie-re/ida-jm-xorstr-decrypt-plugin). Attempts to decrypt JM Xorstr in some x64 binaries.

### Lifting

* [HyRES](https://github.com/Sandspeare/HyRES). HyRES is an innovative hybrid reasoning technique that combines static analysis, large language model (LLM), and heuristic methods to recover data structures from stripped binaries.
* [IDA2LLVM](https://github.com/Sandspeare/ida2llvm). Lifting microcode (IDA IR) into LLVM IR.
* [IDA2LLVM](https://github.com/loyaltypollution/ida2llvm). Dynamic Binary Lifting IDA code to LLVM IR.

Other useful repositories:
* [Anvill](https://github.com/lifting-bits/anvill). anvill forges beautiful LLVM bitcode out of raw machine code.
* [Llvm-mctoll](https://github.com/Microsoft/llvm-mctoll). This tool statically (AOT) translates (or raises) binaries to LLVM IR.
* [McSema](https://github.com/lifting-bits/mcsema). Framework for lifting x86, amd64, aarch64, sparc32, and sparc64 program binaries to LLVM bitcode.
* [Miasm](https://github.com/cea-sec/miasm). Reverse engineering framework in Python.
* [Rellume](https://github.com/aengelke/rellume). Lift machine code to performant LLVM IR.
* [RetDec](https://github.com/avast/retdec). RetDec is a retargetable machine-code decompiler based on LLVM. 
* [rev.ng](https://github.com/revng/revng). The rev.ng binary analysis framework and decompiler.

### MBA

* [D-810](https://gitlab.com/eshard/d810). Deobfuscate code at decompilation time by modifying IDA Pro microcode.
* [gooMBA](https://github.com/HexRaysSA/goomba). Simplify Mixed Boolean-Arithmetic (MBA) expressions.

Other useful repositories:
* [GAMBA](https://github.com/DenuvoSoftwareSolutions/GAMBA). Simplification of General Mixed Boolean-Arithmetic Expressions.
* [POCKET](https://github.com/seekbytes/pocket). Mixed Boolean Arithmetic Expression Obfuscator.
* [SiMBA](https://github.com/DenuvoSoftwareSolutions/SiMBA). Efficient Deobfuscation of Linear Mixed Boolean-Arithmetic Expressions.
* [sspam](https://github.com/quarkslab/sspam). Symbolic Simplification with PAttern Matching.

### Microcode

* [genmc](https://github.com/patois/genmc). Display Hex-Rays Microcode.
* [Lucid](https://github.com/gaasedelen/lucid). An Interactive Hex-Rays Microcode Explorer.

### OLLVM

* [AntiOllvm](https://github.com/IIIImmmyyy/AntiOllvm). AntiOllvm Fla with Fake Runtime.
* [D-810](https://gitlab.com/eshard/d810). Deobfuscate code at decompilation time by modifying IDA Pro microcode.
* [HexRaysDeob](https://github.com/RolfRolles/HexRaysDeob). A plugin for breaking an obfuscating compiler.
* [hrtng](https://github.com/KasperskyLab/hrtng). IDA Pro plugin with a rich set of features: decryption, deobfuscation, patching, lib code recognition and various pseudocode transformations.
* [ObfDetect](https://github.com/mcdulltii/obfDetect). IDA plugin to pinpoint obfuscated code.
* [Stadeo](https://github.com/eset/stadeo). Control-flow-flattening and string deobfuscator.
* [obpo-plugin](https://github.com/obpo-project/obpo-plugin). An OLLVM-CFF Deobfuscation Plugin.

### VMP

* [NoVmpy](https://github.com/wallds/NoVmpy). Proof of Concept, IDA integration of a static devirtualizer for VMProtect x64 3.x. powered by VTIL.
* [VMAttack](https://github.com/anatolikalysch/VMAttack). Use additional analysis features designed to counter virtualization-based obfuscation.

