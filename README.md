<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/7d1610b8-36ca-4add-94de-15ef257b9d06" />### study-of-basic-gates

**AIM:** 

To study and verify the truth table of logic gates in Quartus II using Verilog programming.

**Equipments Required:**

Software – Quartus prime 

**Theory**

Introduction Logic gates are the basic building blocks of any digital system. Logic gates are electronic circuits having one or more than one input and only one output. The relationship between the input and the output is based on a certain logic. Based on this, logic gates are named as

AND gate OR gate NOT gate NAND gate NOR gate Ex-OR gate Ex-NOR gate

**AND gate**

The AND gate is an electronic circuit that gives a high output (1) only if all its inputs are high. A dot (.) is used to show the AND operation i.e. A.B or can be written as AB
Y= A.B

**OR gate** 

The OR gate is an electronic circuit that gives a high output (1) if one or more of its inputs are high. A plus (+) is used to show the OR operation.
Y= A+B

**NOT gate**

The NOT gate is an electronic circuit that produces an inverted version of the input at its output. It is also known as an inverter. If the input variable is A, the inverted output is known as NOT A. This is also shown as A' or A with a bar over the top, as shown at the outputs.
Y= A'

**NAND gate**

This is a NOT-AND gate which is equal to an AND gate followed by a NOT gate. The outputs of all NAND gates are high if any of the inputs are low. The symbol is an AND gate with a small circle on the output. The small circle represents inversion.
Y= (AB)’

**NOR gate**

This is a NOT-OR gate which is equal to an OR gate followed by a NOT gate. The outputs of all NOR gates are low if any of the inputs are high. The symbol is an OR gate with a small circle on the output. The small circle represents inversion.
Y= (A+B)’

**Ex-OR gate**

The 'Exclusive-OR' gate is a circuit which will give a high output if either, but not both of its two inputs are high. An encircled plus sign (⊕) is used to show the Ex-OR operation.
Y= A⊕B

**Ex-NOR gate**

The 'Exclusive-NOR' gate circuit does the opposite to the EX-OR gate. It will give a low output if either, but not both of its two inputs are high. The symbol is an EX-OR gate with a small circle on the output. The small circle represents inversion.
Y= A⊕B

**Procedure** 

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**PROGRAM**

Program for logic gates and verify its truth table in quartus using Verilog programming

 Developed by: RegisterNumber: 25011975
 ```
module logic_gates(
    input A,
    input B,
    output AND_out,
    output OR_out,
    output NOT_out,
    output NAND_out,
    output NOR_out,
    output XOR_out,
    output XNOR_out
);

assign AND_out = A & B;
assign OR_out = A | B;
assign NOT_out = ~A;
assign NAND_out = ~(A & B);
assign NOR_out = ~(A | B);
assign XOR_out = A ^ B;
assign XNOR_out = ~(A ^ B);

endmodule
```

 
**Logic symbol & Truthtable**

<img width="1203" height="277" alt="Screenshot 2025-11-26 204223" src="https://github.com/user-attachments/assets/3aa726dd-31b9-4e01-8a10-4c9a7a85e18d" />
<img width="596" height="148" alt="Screenshot 2025-11-26 204153" src="https://github.com/user-attachments/assets/9c48ed94-6c89-483d-b2b5-4431b1385f1c" />


**RTL realization Output:** 
<img width="511" height="388" alt="Screenshot 2025-11-26 203635" src="https://github.com/user-attachments/assets/d538c9f4-2e15-44f4-a947-bf7257b3251b" />
**RTL**

**Result:**
<img width="1919" height="1079" alt="Screenshot 2025-11-26 203923" src="https://github.com/user-attachments/assets/0980dbb7-2e6c-4a4b-ad62-9a01e96fec46" />


