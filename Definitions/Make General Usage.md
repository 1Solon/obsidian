**General Notes:**
* The user runs the command **make blah** to build the target blah 
* If the user just types **make**, make will build the first rule that doesn’t start with a dot (.) 
* Common practice to also include a target called clean to remove build files, and a target called install to install the program to somewhere on the system path.