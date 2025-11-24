

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**

**Logic Diagram**
<img width="545" height="823" alt="Screenshot 2025-11-22 221507" src="https://github.com/user-attachments/assets/eb702b85-dbfb-4e8e-8f6f-70e3ae13dd9c" />
<img width="621" height="864" alt="Screenshot 2025-11-22 221559" src="https://github.com/user-attachments/assets/ab209d8e-42e1-4e66-a35f-74126ee43f06" />
![logic](https://github.com/user-attachments/assets/add9dadb-2890-4314-8ee9-c5eecaeab86a)

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by:Sujith Mano M 
RegisterNumber:25018328 */
```
i) 
module suji02(a,b,c,d,f1); 
input a,b,c,d; 
output f1; 
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c)); 
endmodule 
ii) 
module suji03(w,x,y,z,f2); 
input w,x,y,z; 
output f2; 
assign f2=((~y & z)|( w & y )|(x & y)); 
endmodule
```

**RTL realization**
<img width="1920" height="1080" alt="Screenshot 2025-11-22 223938" src="https://github.com/user-attachments/assets/f3332dfb-fcb3-4d63-9643-c1c47489616f" />
<img width="1920" height="1080" alt="Screenshot 2025-11-22 224722" src="https://github.com/user-attachments/assets/555c40f7-c2b3-4abb-8148-79849e774a43" />

**Output:**
<img width="1920" height="1080" alt="Screenshot 2025-11-24 110129" src="https://github.com/user-attachments/assets/19582ec4-d0ac-404b-9775-0bfcccf63f33" />
<img width="1920" height="1080" alt="Screenshot 2025-11-24 110610" src="https://github.com/user-attachments/assets/62ee1ecb-b5ab-4359-bbf8-41ad86e6d020" />

**RTL**
<img width="1920" height="1080" alt="Screenshot 2025-11-22 223303" src="https://github.com/user-attachments/assets/c50febee-9443-4c37-a4bb-d5de50e76c13" />
<img width="1920" height="1080" alt="Screenshot 2025-11-22 224630" src="https://github.com/user-attachments/assets/86e8109e-86ef-4cd8-865f-b9cb82dcad3b" />

**Timing Diagram**

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

