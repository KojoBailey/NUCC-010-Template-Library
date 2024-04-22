# [NUCC 010 Editor Template Library](https://github.com/KojoBailey/NUCC-010-Template-Library/)
**Run 1 template for all XFBINs.** That is the ultimate goal of this library.

![image](https://github.com/KojoBailey/NUCC-010-Template-Library/assets/50509420/82a9df28-c956-4d1b-a501-f527cac03917)

This repository contains a library of **[010 Editor](https://jojomodding.miraheze.org/wiki/010_Editor) templates** for parsing **[CyberConnect2](https://jojomodding.miraheze.org/wiki/CyberConnect2) [NUCC](https://jojomodding.miraheze.org/wiki/NUCC) file data**, whether that be [XFBIN](https://jojomodding.miraheze.org/wiki/XFBIN) container files in their entirety, or the individual files they contain. This of course includes certain formats and versions of formats from Bandai Namco's **NU Library**, which games by other Japanese studios may be familiar with (e.g. NUT, NUS3Bank, NUD, etc.), aiming to provide information on as much data as XFBIN files contain as possible.

However, despite the *very* wide range of templates included in this library, when it comes to the big daddy XFBIN files themselves, you should only ever need to run a **single template**: `xfbin.bt`. The other templates exist to:
1. split the library into different files for **easier** management and contribution.
2. provide **flexibility**, allowing the singling out of certain sections of data and run individual templates on them.

## Installation
Start by downloading **all** of the templates from the [Templates](https://github.com/KojoBailey/NUCC-010-Template-Library/tree/main/Templates) folder. Eventually, I'll have releases in ZIPs for these, but downloading the repo manually will do for now.

It is important that you do download **all** of them, even if you don't "need" all of them, since the nature of 010 Editor's include system requires that every mentioned file exists (I'll see if this can be combatted in the future). Once you've done that, just open and run `xfbin.bt`. You can also set this to run on XFBIN files automatically.

If you've never ran templates with 010 Editor before, you may want to check out this quick guide: [Installing and running 010 Editor templates](https://jojomodding.miraheze.org/wiki/Guide:Installing_and_running_010_Editor_templates).

## Structure
Like most file formats, XFBINs start with the magic `NUCC` (`4E 55 43 43`), and this is asserted with the library. Although XFBIN files can technically load into games fine without this "magic", the library requires it anyway to verify an XFBIN.
