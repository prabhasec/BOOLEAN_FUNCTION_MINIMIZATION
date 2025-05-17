# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**

**Logic Diagram**

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**
```
module func(a,b,c,d,f1); 
input a,b,c,d; 
output f1; 
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c)); 
endmodule

module func1(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=((~y&z)|(w&y)|(x&y));
endmodule
```
/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: prabha B G RegisterNumber:212224050029*/


**RTL realization**

**Output:**

**RTL**
![Screenshot 2025-04-16 083107](https://github.com/user-attachments/assets/59c669b2-a3a3-4215-a6ea-36891bef1d58)
![Screenshot 2025-04-16 092843](https://github.com/user-attachments/assets/70b702e6-1831-4ba4-8258-ba952332d6ed)


**Timing Diagram**
![Screenshot 2025-04-16 090419](https://github.com/user-attachments/assets/9292fc19-f074-4620-810b-d12188862b64)
![Screenshot 2025-04-16 093236](https://github.com/user-attachments/assets/8d23cc7b-7f5d-4073-b818-cd564610f55e)



**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.



