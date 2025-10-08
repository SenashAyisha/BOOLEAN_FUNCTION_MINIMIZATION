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
module funct1(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
endmodule
```


```
module funct2(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=((~y & z)|( w & y )|(x & y));
endmodule
```

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: RegisterNumber:*/


**RTL realization**
<img width="1621" height="951" alt="image" src="https://github.com/user-attachments/assets/feec7d65-36d4-465c-95a3-d41b54cf7223" />
<img width="1534" height="874" alt="image" src="https://github.com/user-attachments/assets/c1f52e82-967f-49ee-8756-08ef336700b0" />

**Output:**

**RTL**
<img width="1902" height="543" alt="image" src="https://github.com/user-attachments/assets/57f9a209-37af-4e89-ba08-a7621af89439" />
<img width="1913" height="657" alt="image" src="https://github.com/user-attachments/assets/ba73e481-c43d-4d7f-bb67-f1375b7fd80f" />

**Timing Diagram**

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

