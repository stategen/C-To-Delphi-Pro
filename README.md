# C-To-Delphi-Pro
![Screenshot](https://github.com/stategen/C-To-Delphi-Pro/blob/master/CToDelphiProSnap3.png)
## Description
After spending a month manually modifying the Pascal code translated by C-To-Delphi, I'm exhausted, and the progress I made feels close to zero. After searching again on the internet, I had to start over and rewrite C-To-Delphi. Initially, I thought C-To-Delphi had completed 90% of the work, and I would just need to fix a few bugs. However, once I started the task, I realized that C-To-Delphi had only done 10%, leaving the remaining 90% of the conversion details unhandled. It took me a whole six months to complete that 90%. Hence, the software is named C-To-Delphi Pro. I want to express my gratitude to the author of C-To-Delphi for providing the initial framework and idea. C-To-Delphi Pro is a niche software designed for those who need to accurately and efficiently translate C or C++ code into Delphi(pascal), saving time. Don't underestimate the complexity of the C++ language and avoid attempting manual translation.
Account settings

[Download](https://www.stategen.org/download/ "Download") executable here.
<!-- [![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/s/fc3fdce454) -->
It contains a split view, with C on the left and Delphi(pascal)on the right.
The Delphi code gets updated in realtime when you edit the C code.
The editors are kept in sync, so you can easily find how a specific piece of code was converted.

* The **Syntax checks** of the generated code is verified. (uses DelphiAST)
* You can even **run** the generated code by pressing F9 (uses DWS)

* You can drag/drop multiple C files to the application. It'll find the .h files that belong to it, and convert all to .pas files in the same folder.

## Features:

* If function main exists, a program will be generated. Otherwise a pascal unit with interface/implementation sections.
* Merge header  and implementation file to one dephi file
* Aggregate scattered implementation code across different c/c++ files.
* Converts routines and arguments
* Converts for loops(check use for or for-to-while, "count" as "to count -1" )
* Converts case statements(remove breaks,auto surround with begin...end)
* Smart Convers if-statement
* Smart Surround 'and' and 'or' with parentheses on both sides.
* Converts structs
* Converts enums
* Converts 1 and 2 dimensional arrays
* Converts many other common routines to Delphi equivalents (strcpy,strcat,strlen,printf,argv,argc,etc)
* Converts classes
* Nested class ,structs,enums
* Inline class ,structs,enums
* Inline method,
* Method as variable.
* C interface to Delphi interface
* C stack object to Delphi heap object with smart call constructor
* C pointer to Delphi var parameter
* Smart keep @ ^
* Smart C (Type) to Delphi Type() 
* C String to Delphi String with delphi chars #10,#13,#0...
* Auto C Const to delphi  Const or  ar
* Nested Const  Var initialization
* Custom regular conversion or fix
* Custom file name prefix and suffix

