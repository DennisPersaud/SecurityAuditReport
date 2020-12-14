# SecurityAuditReport
This is an audit report for an application that I analyzed for security flaws.

## Summary of Methods

When visually inspecting the code, I first checked where the developer accepted user input in each unit of code. I found that the developer had accepted user input in multiple units through out different class files. I then checked to verify if the developer created any functionality to validate the user input in each unit where the user input was accepted. I found that the developer did not validate the user input anywhere in the code, this indicates to me that this code may potentially contain vulnerabilities and bugs.

When trying to compile the code I received 37 warnings but the code compiled successfully with 0 errors. This confirmed my suspicion from my visual inspection that the code contained potentially contained vulnerabilities and bugs. The warnings that were thrown by the compiler indicated that there had been bugs present in several files contained within this project. Those files are Gas.cpp, Login.cpp, Record.cpp, and Service.cpp. The compiler warnings and their description can be found in the attached image below.

![CppChecker](https://i.imgur.com/AWgqisa.jpg)

After reviewing the warnings thrown by the compiler, I then used cppchecker to perform a static analysis of the code. After running the static code analysis, I found several errors, warnings, and style warnings contained within different class files of this program. The static code analysis indicated that there are more severe errors contained within the code in comparison to the warnings thrown by the compiler. The resources that were found to contain these errors within the project are Gas.cpp, Login.cpp, Record.cpp, Service.cpp, and Service.h. A summary of each of the errors and warnings found by the static code analysis tool is shown in the image below.

![CompilerWarnings](https://i.imgur.com/9EnwZBQ.jpg)
