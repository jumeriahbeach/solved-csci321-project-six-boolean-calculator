Download Link: https://assignmentchef.com/product/solved-csci321-project-six-boolean-calculator
<br>
<strong>Objectives:</strong>

<ol>

 <li>Implement a menu</li>

 <li>Apply Table-Driven Selection technique (Read Section 6.5.4)</li>

 <li>Implement user defined procedures</li>

 <li>Call user defined procedures</li>

 <li>Apply Irvine32.inc library</li>

</ol>

<strong>Problem Description:</strong>

Create a program that functions as a simple Boolean calculator for 32-bit integers. It should display a menu that asks the user to make a selection from the following list:

<ol>

 <li>X AND Y</li>

 <li>X OR Y</li>

 <li>NOT X</li>

 <li>X XOR Y</li>

 <li>Exit Program</li>

</ol>

When the user makes a choice, call the corresponding procedure, which is one of the following four:

<ol>

 <li>AND_op: Prompt the user for two hexadecimal integers. AND them together and display the result in hexadecimal</li>

 <li>OR_op: Prompt the user for two hexadecimal integers. OR them together and display the result in hexadecimal.</li>

 <li>NOT_op: Prompt the user for a hexadecimal integer. NOT the integer and display the result in hexadecimal.</li>

 <li>XOR_op: Prompt the user for two hexadecimal integers. Exclusive-OR them together and display the result in hexadecimal.</li>

</ol>

You may refer to Programming Exercises #5 and #6 on page 239

<strong>Sample Run:</strong>

After menu displayed, I chose 1. I use “Call ReadChar” to get user input. However, ReadChar will not echo the char typed in terminal window. So I use:

call ReadChar

call WriteChar




<strong>Explain Result:</strong>

12345678h in binary is 0001 0010 0011 0100 0101 0110 0111 1000

11112222h in binary is 0001 0001 0001 0001 0010 0010 0010 0010

So their bit-wise and is 0001 0000 0001 0000 0000 0010 0010 0000 which is 101000220h

After hit any key, loop repeated. First it cleared the screen, then displayed menu for user to choose again. This time I chose 2 and entered 12345678 and 11112222 and the result was 1335767A.

<strong>Explain Result:</strong>

12345678h in binary is 0001 0010 0011 0100 0101 0110 0111 1000

11112222h in binary is 0001 0001 0001 0001 0010 0010 0010 0010

So their bit-wise OR is: 0001 0011 0011 0101 0111 0110 0111 1010 which is 1335767Ah

After hit any key, loop repeated. First it cleared the screen, then displayed menu for user to choose again. This time I chose 3 and entered 12345678. The result was: EDCBA987

<strong>Explain Result:</strong>

12345678h in binary is 0001 0010 0011 0100 0101 0110 0111 1000

So its bit-wise NOT is      1110 1101 1100 1011 1010 1001 1000 0111 which is EDCBA987h

After hit any key, loop repeated. First it cleared the screen, then displayed menu for user to choose again. This time I chose 4 and entered 12345678 and 11112222 and the result was 0325745Ah

<strong>Explain Result:</strong>

12345678h in binary is 0001 0010 0011 0100 0101 0110 0111 1000

11112222h in binary is 0001 0001 0001 0001 0010 0010 0010 0010

So their bit-wise xor is  0000 0011 0010 0101 0111 0100 0101 1010 which is 0325745A

After hit any key, the menu in new screen show up. This time I chose option 5

Then I hit any key to exit to program.

<strong>Due Date:</strong>

Turn in YourNameProj6.asm via Blackboard. Due date will be announced on Blackboard.