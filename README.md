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
~~~
module exp_2(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
endmodule
~~~
~~~
module exp_2(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=((~y & z)|( w & y )|(x & y));
endmodule
**RTL realization**
~~~

**Output:**
![WhatsApp Image 2025-10-17 at 10 34 22 AM](https://github.com/user-attachments/assets/cc47bf78-52db-49fc-addc-e79d5f611719)

![WhatsApp Image 2025-10-17 at 10 34 23 AM](https://github.com/user-attachments/assets/256d9b32-2c0f-45ae-a01d-e0e43d8e60ec)

**RTL**
![WhatsApp Image 2025-10-17 at 10 34 23 AM (1)](https://github.com/user-attachments/assets/163828bf-a181-496c-86c3-317f2e89f466)
![WhatsApp Image 2025-10-17 at 10 34 24 AM](https://github.com/user-attachments/assets/104277a6-d339-4aa6-a8f1-f24e83ec1222)

**Timing Diagram**

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

