# OffensiveGo - Golang Weaponization for your malwares.

![image](https://user-images.githubusercontent.com/75935486/220174996-d0a44ce7-6c90-4ec1-b140-c410cfc0fc07.png)


This repo that contains some examples of offensives tools & utilities that can be used in a red team engagement rewrote in Golang. This project is also a way to train me to golang.

## Table of Content

- [Previous work](#previous-work)
- [About Golang](#about-golang)  
  - [Installation](#installation)
  - [Compilation](#compilation)
- [Examples](#examples)
- [Interesting Tools in Golang](#interesting-tools-in-golang)
- [Credits](#credits)

## Previous work

These repo inspires me to make [OffensiveGo](https://github.com/RistBS/OffensiveGo)

- https://github.com/trickster0/OffensiveRust : Made by [trickster012](https://twitter.com/trickster012), this projects contains a bunch of example made in Rust
- https://github.com/byt3bl33d3r/OffensiveNim : 


## About Golang

- **Simpler syntax**: Go's syntax is simpler and easier to learn compared to Rust, which has a steeper learning curve.
- **Garbage collection**: Go uses garbage collection, which makes memory management easier for developers. Rust, on the other hand, uses a borrow checker to enforce memory safety, which can be more difficult to work with.
- **Cross-platform support**: Go has excellent cross-platform support and can be compiled to run on a wide range of platforms, including Windows, Linux, and macOS. Rust also has good cross-platform support, but its compilation process can be more complex.


Why using Golang

- Excellent cross platform compilation capabilities
- Performant, type safe, garbage collected
- Robust development stack
- Native code with few, if any, deployment dependencies
- Easy Syntax


### Installation


### Compilation

`go build` for compilation 

Go binaries generally have no installation dependencies, compiler statically links Go runtime and needed packages. Static linking results in larger binaries


## Examples 

| File                                                                                                   | Description                                                                                                                                                                              |
|--------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [Allocate_With_Syscalls](../master/Allocate_With_Syscalls/src/main.rs)                                 | It uses NTDLL functions directly with the ntapi Library                                                                                                                                  |
| [Create_DLL](../master/Create_DLL/src/lib.rs)                                                          | Creates DLL and pops up a msgbox, Rust does not fully support this so things might get weird since Rust DLL do not have a main function                                            |
| [DeviceIoControl](../master/DeviceIoControl/src/main.rs)                                               | Opens driver handle and executing DeviceIoControl                                                                                                                                        |
| [EnableDebugPrivileges](../master/EnableDebugPrivileges/src/main.rs)                                   | Enable SeDebugPrivilege in the current process                                                                                                                                            |
| [Shellcode_Local_inject](../master/Shellcode_Local_inject/src/main.rs)                                 | Executes shellcode directly in local process by casting pointer                                                                                                                      |
| [Sleep Obfuscation](../main/Sleep_Obfuscation/main.go)                                                 | Perform Sleep Obfuscation with Queue Timers                                                                                                                                              |
 


## Interesting Tools in Golang

- [BananaPhone](https://github.com/C-Sto/BananaPhone) : An easy to use GO variant of [Hells gate](https://github.com/am0nsec/HellsGate) with automatic SSN parsing.
- [SourcePoint](https://github.com/Tylous/SourcePoint) : C2 profile generator for Cobalt Strike command and control servers designed to ensure evasion by reducing the Indicators of Compromise IoCs.
- [ScareCrow](https://github.com/optiv/ScareCrow) : Payload creation framework designed around EDR bypass such as AMSI & ETW Bypass, Encryption, Stealth Process Injections ect...
- [Freeze](https://github.com/optiv/Freeze) : Payload toolkit for bypassing EDRs using suspended processes, direct syscalls, and alternative execution methods.
- [Mangle](https://github.com/optiv/Mangle) : A tool that manipulates aspects of compiled executables (.exe or DLL) to avoid detection from EDRs.
- [Dent](https://github.com/optiv/Dent) : A framework for creating COM-based bypasses utilizing vulnerabilities in Microsoft's WDAPT sensors.
- [Ivy](https://github.com/optiv/Ivy) : Payload creation framework for the execution of arbitrary VBA (macro) source code directly in memory. Ivy’s loader does this by utilizing programmatical access in the VBA object environment to load, decrypt and execute shellcode.




## Credits

- [@BlueSentinelSec](https://twitter.com/BlueSentinelSec) - https://github.com/bluesentinelsec/OffensiveGoLang/blob/master/Offensive%20GoLang%202.0%20-%20SANS%20Pen%20Test%20HackFest%202021.pdf
