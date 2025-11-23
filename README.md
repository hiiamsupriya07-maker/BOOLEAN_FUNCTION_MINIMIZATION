# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**
**Logic Diagram**
<img width="1024" height="883" alt="image" src="https://github.com/user-attachments/assets/af764848-b37b-4c75-a832-11fb01688050" />

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 
```
module exp2(f1,a,b,c,d,f2,w,x,y,z);
input (a,b,c,d,w,x,y,z);
output (f1,f2);
assign f1=~(a&b&c&d)|(a~&c~d)|(~b&c~&d)|(a&b&c&d)|(b&~&c&d);
assign f2=(x~&y&z)|(x~&y~&z)|(w~&x&y)|(w~&x&y)|(w&x&y);
endmodule
```
Developed by: RegisterNumber:25017133

**RTL realization**

**Output:**
**Table**

<img width="513" height="1280" alt="image" src="https://github.com/user-attachments/assets/f978b74e-9a03-48b4-a4d7-57429baed0e2" />

**RTL**
<img width="1024" height="883" alt="image" src="https://github.com/user-attachments/assets/2aafbf55-f957-4dd5-86f9-abeaf4d0b7e9" />
**Timing Diagram**
<img width="1280" height="419" alt="image" src="https://github.com/user-attachments/assets/239980c1-0eca-4bd2-9e50-3c68729e1097" />
**Result:**
Thus the given logic functions are implemented and their operations are verified using Verilog programming.

