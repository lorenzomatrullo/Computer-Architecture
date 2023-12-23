# Logic Gates

**0** -> OFF -> False -> 0 Volts
<br>
**1** -> ON -> True -> 5 volts (something over than 0)

<br>

**Transistor**: *device that is used to control or regulate the flow of electronic signals.*<br>

<img align="right" width="400" height="193" src="../imgs/transistor.png">

<font size = "1">Parts of the transistor
<br>
&emsp;&emsp; **Emitter** -> *the transistor's negative lead.*
<br>
&emsp;&emsp; **Base** -> the terminal that activates the transistor.
<br>
&emsp;&emsp; **Collector** -> *the transistor's positive lead.*<br></font>

&emsp;&emsp; **NPN** -> *Negative-Positive-Negative*<br>
&emsp;&emsp; **PNP** -> *Positive-Negative-Positive*

<br>
<br>
<br>

### **BUFFER Gates**:

*Strengthens a signal without changing its logic value.<br> 
<font size = "1">(E.G. if it receives a logic 1, it outputs a logic 1, and if receives a logic 0, it outputs a logic 0)*</font>


![BUFFER-GATES](../imgs/BUFFER-gates.png)

<br>

### **NOT Gates**:

**Ā** = *Complementary of A*

*Not gate is also called a negator, because it "negates" the input.
<br>
<font size = "1">If it receives a logic 1, it outputs a logic 0, and if it receives a logic 0, it outputs a logic 1*</font>

![NOT-GATES](../imgs/NOT-gates.png)


### **AND Gate**:

*We can get an AND gate using two NPN transistors connected in series in a common collector configuration.*


![AND-GATES](../imgs/AND-gates.png)


### **NAND Gate**:

*NAND is the complementary of AND.*
<br>
<font size = "1">*The combination of an AND gate and a NOT gate --> NAND gate*</font>

![NAND-GATES](../imgs/NAND-gates.png)


### **OR Gate**:

*The OR gate outputs "true" if any of its inputs are "true", otherwise it outputs "false".*

![OR-GATES](../imgs/OR-gates.png)


### **NOR Gate**:

*NOR is the complementary of OR.*
<br>
<font size = "1">*The combination of an OR gate and a NOT gate --> NOR gate*</font>

![NOR-GATES](../imgs/NOR-gates.png)

<br>
<b>- <ins>FUNCTION EXAMPLES</b></ins>
<br>
<br>

**AND GATE** = *multiplication*
<br>
**OR GATE** = *addition*

![write-funtion-from-diagrams](../imgs/write_function.png)


![draw_diagram_from_function_SOP](../imgs/draw_function_SOP.png)
<font size = "1">*SOP -> sum of products expression*</font>


![draw_diagram_from_function_POS](../imgs/draw_function_POS.png)
<font size = "1">*POS -> product of sums expression*</font>
