# verilog-lab-2-binary-to-bcd-solved
**TO GET THIS SOLUTION VISIT:** [Verilog Lab 2-Binary-to-BCD Solved](https://www.ankitcodinghub.com/product/verilog-lab-2-binary-to-bcd-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;91439&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;0&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;0&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;0\/5 - (0 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;Verilog Lab 2-Binary-to-BCD Solved&quot;,&quot;width&quot;:&quot;0&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 0px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            <span class="kksr-muted">Rate this product</span>
    </div>
    </div>
<div class="page" title="Page 1">
<div class="layoutArea">
<div class="column">
Lab 2 Binary-to-BCD

The purpose of this lab is to build a Binary-to-BCD converter using the double dabble algorithm (aka the shift-add-3 algorithm). You will only utilize combinational circuit components, verify the functionality of the converter using a testbench, and test the converter on the FPGA board by using it to display the output of a simple calculator.

Part 1 (Building a Binary-to-BCD Converter)

Binary Coded Decimal (BCD) is a numbering system used to represent decimal numbers using binary representations. Each BCD digit is composed of 4 bits and can represent a number from 0 to 9. Table 1 shows how to represent all decimal digits using BCD, the table also indicate the other six binary numbers (i.e. 1010, 1011, etc.) are not used.

Table 1: BCD Representation

</div>
</div>
<div class="layoutArea">
<div class="column">
Decimal Digit

0 1 2 3 4 5 6 7 8 9

</div>
<div class="column">
BCD Representation

<pre>     0000
     0001
     0010
     0011
     0100
     0101
     0110
     0111
     1000
     1001
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
Decimal numbers with multiple digits require 4-bit BCD numbers for each of the digits. Table 2 shows an example of using BCD to represent a 3 digits decimal number. The same concept can be applied to decimal numbers with more digits.

Table 2: Multidigit Decimal Number in BCD

Hundreds Tens Ones Decimal 3 9 7

BCD 0011 1001 0111

Many arithmetic operations are done in binary, then converted to BCD for display purposes (i.e. displaying the result on a seven-segment or LCD display). In this lab you will build a circuit that takes an 8-bit binary number and converts it to its 3 digits BCD representation.

</div>
</div>
<div class="layoutArea">
<div class="column">
1

</div>
</div>
</div>
<div class="page" title="Page 2">
<div class="layoutArea">
<div class="column">
When converting a binary number to its BCD reperesentation, more than one BCD digit locations might be required. For example, the binary number 1100 represent the decimal number 12, to convert this 4-bit binary number to its BCD representation, we first note that it is greater than 1001 (9 decimal), so we have to add 0110 (6 decimal), the result is 10010 which is equivalent to 0001 0010 the BCD representation of 12.

A similar computation could be done using shifts. Recall that a left shift moves all bit values one position to the left (toward the MSB). A left shift has the same function as multiplying the binary number by two. If we have the number 0101 (5 decimal), and we shift it left, we know the result will be 1010 (10 decimal), assuming we shift in a zero. If we then want to convert this number to a BCD, we will have to add six to it. Knowing that we will convert the number to BCD, we can check the original number before shifting it. If it is greather than or equal to five, then we can add three to that number (instead of adding 6 to the shifted number). Then when we shift it, it will automatically be in BCD form. Table 3 illustrates this concept using the number 0110.

Table 3: Preemptive add, then shift example

</div>
</div>
<div class="layoutArea">
<div class="column">
Operation

Original number Add 3

Shift Left Decimal

</div>
<div class="column">
Binary

1001 0001 0010 12

</div>
</div>
<div class="layoutArea">
<div class="column">
0110

</div>
</div>
<div class="layoutArea">
<div class="column">
This concept can be used on a binary number with any number of bits. For each bit in the binary number, the shift-add-3 algorithm must be implemented. For a four bit number, four shifts must be performed. Before each shift is performed, if the number is greater than or equal to five, then it must be added to three. Once all four bits have been shifted, the final BCD number will be in the upper-most bits of the new number. See the example in Table 4.

Table 4: Example of converting 1111 to BCD

</div>
</div>
<div class="layoutArea">
<div class="column">
Operation

Start Shift Shift Shift Add-3 Shift Decimal

</div>
<div class="column">
Tens Ones Binary

1111 1 111

11 11 111 1 1010 1

1 0101 1 5

</div>
</div>
<div class="layoutArea">
<div class="column">
To perform a 4-bit binary conversion, 12 bits must be used. The upper four bits will be the tens decimal digit and the middle four will be the ones decimal digit. The lower four bits will be ignored. In the previous example, only the relevant bits were shown. In reality, the missing bit

</div>
</div>
<div class="layoutArea">
<div class="column">
2

</div>
</div>
</div>
<div class="page" title="Page 3">
<div class="layoutArea">
<div class="column">
locations would contain zeros. This process can be extended for any size of binary number. Check Table 5 for another example using an 8- bit binary number.

</div>
</div>
<div class="layoutArea">
<div class="column">
Table 5: Example of converting 1111 1111 to BCD

</div>
</div>
<div class="layoutArea">
<div class="column">
Operation

</div>
<div class="column">
Hundreds

</div>
<div class="column">
Tens Ones

</div>
<div class="column">
Binary

</div>
</div>
<div class="layoutArea">
<div class="column">
Start

Shift

Shift

Shift

Add-3

Shift

Add-3

Shift

Shift

Add-3

Shift

Add-3

Shift

Decimal 255

Implementation Steps

The double dabble algorithm can be used to convert binary numbers of arbiterary length. In fact, the double dabble’s wikipedia article contains a parameterized verilog implementation that can be used with binary numbers of any length. You should not use that code. Instead you should develop a version that converts an 8-bit binary numbers into their equivalent BCD. Of course an 8-bit binary numbers should result in BCDs ranging from 000 to 255.

The double dabble can be completely implemented using combinational circuit elements, without using storage elements nor registers. Table 6 and figure one contain the details of the implementation.

The following steps should guide you through the implementation.

</div>
</div>
<div class="layoutArea">
<div class="column">
<pre>               1111
               1111
               1111
               1111
               1111
</pre>
1 0101 1111

</div>
<div class="column">
1111 111 11

1

1

</div>
</div>
<div class="layoutArea">
<div class="column">
1 11 111 1010

</div>
</div>
<div class="layoutArea">
<div class="column">
1 1000 1111 11 0001 111

</div>
</div>
<div class="layoutArea">
<div class="column">
1

1 10

</div>
<div class="column">
110 0011 11 1001 0011 11 0010 0111 1 0010 1010 1 0101 0101

</div>
</div>
<div class="layoutArea">
<div class="column">
Table 6: Add-3 module

A[3:0] S[3:0]

0000 0000 0001 0001 0010 0010 0011 0011 0100 0100 0101 1000 0110 1001 0111 1010 1000 1011 1001 1100 1010 XXXX 1011 XXXX 1100 XXXX 1101 XXXX 1110 XXXX 1111 XXXX

</div>
</div>
<div class="layoutArea">
<div class="column">
1. Create a module (call it add_3) to implement the add-3 part of the

algorithm. Follow the truth table shown in Table 6. The module

should have 4-bit input (A) and 4-bit output (S). The truth table

shows that when the number in the input is less than 4, it is passed as is, when the number exceeds 4, the output will be the result of adding 3 to the input. The algorithm

</div>
</div>
<div class="layoutArea">
<div class="column">
3

</div>
</div>
</div>
<div class="page" title="Page 4">
<div class="layoutArea">
<div class="column">
will not allow any number above 9, so the implementation treats those inputs as don’t

care.

<ol start="2">
<li>Shifting numbers in combinational circuits is done by connecting the inputs to the
outputs while shifting by one position. For example, a left shift can be achieved by connecting the least significant bit to the second least significant bit, and the same for the rest of the wires. You should also connect 0 to the least signficiant bit of the output.
</li>
<li>Create a module (call it bin2bcd) that implements an 8-bit binary to BCD converter. Figure 1 shows the diagram for this module. The module should have 8-bit input (bin) and 12-bit output (bcd). You should instantiate as many instances of add_3 as necessary.</li>
<li>Verify the functionality of bin2bcd by writing a testbench (bin2bcd_tb) to test its functionality .</li>
<li>Include a screenshot of the simulation output with your submission, you should embed the screenshot in your README.md file.
Figure 1: 8-bit implementation of the double dabble binary to BCD converter
</li>
</ol>
Part 2 (Building a simple calculator with BCD outputs)

In this part, you will modify the simple_calc module you developed in a previous lab so that it displays its output as BCD instead of binary. Recall, the calculator should perform 4-bit addition, subtraction, and multiplication.

1. Import simple_calc along with all necessary dependencies (i.e. the adder/subtractor, csa multiplier,etc.)

</div>
</div>
<div class="layoutArea">
<div class="column">
4

</div>
</div>
</div>
<div class="page" title="Page 5">
<div class="layoutArea">
<div class="column">
<ol start="2">
<li>Modify the module so it displays its result on 12 LEDs as BCD. You should utilize the bin2bcd module you developed in part 1.

As a reminder

a. The module should accept two 4-bit inputs X, Y

b. The module should accept a 2-bit operator select input (op_sel).

i. op_sel = 00 (add)

ii. op_sel = 01 (subtract) iii. op_sel = 1x (multiply)

c. The module should output a 12-bit signal (result) represented in BCD
</li>
<li>The bin2bcd module you developed in part 1 assumes positive numbers only. You
should figure out what needs to be done if the answer of the simple_calc is being interpreted as a signed number. For example, you might need to take its 2’s complement before passing it to the converter and use one of the LEDs to indicate the answer is negative.
</li>
<li>Verify the functionality of your simple calculator by implementing in on the FPGA board using the following IO specifications:
i. SW3ßSW0 for the inputX ii. SW7 ß SW4 for the input Y

iii. SW15 ß SW14 for the op_sel

iv. LED11 ß LED0 for the output result (displayed as BCD)

v. LED13 to indicate the result displayed is negative

vi. LED14 to display the carry_out of the adder/subtractor

vii. LED15 to display the overflow of the adder/subtractor
</li>
</ol>
</div>
</div>
</div>
