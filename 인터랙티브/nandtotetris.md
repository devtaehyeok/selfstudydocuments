# nandtotetris

![](/images/nandtotetris/nandtotetris_235556.png)

nand로 컴퓨터 만들기

how : implementation
what : abstration

In a nutshell: We will start with a brief introduction of Boolean algebra, and learn how Boolean functions can be physically implemented using logic gates. We will then learn how to specify gates and chips using a Hardware Description Language (HDL), and how to simulate the behaviour of the resulting chip specifications using a hardware simulator. 

기초 15개의 로직 게이트를 nand로 만들기

-> ALU, MEMORY SYSTEM
Arithmetic Logic Unit 

지능이란 도구를 위한 도구를 만드는 능력.

objects
whose interfaces consist of input and output pins that carry binary signals, and whose
implementations are connected arrangements of other, lower-level, chips.

![](/images/nandtotetris/nandtotetris_054443.png)

![](/images/nandtotetris/nandtotetris_054509.png)

The contract is as follows: you are allowed to do
whatever you want under the PARTS statement; you are not allowed to change anything above
the PARTS statement.

0,1 on and off

formula

truth table

communicative laws 

![](/images/nandtotetris/nandtotetris_055844.png)

![](/images/nandtotetris/nandtotetris_055959.png)

![](/images/nandtotetris/nandtotetris_060329.png)

idempotence

![](/images/nandtotetris/nandtotetris_064627.png)

OR 은 드모르간으로 표현 가능하므로

모든 연산은 AND NOT 만으로 표현 가능.
모든 불리언 연산은 NAND로 표현 가능

https://slideplayer.com/user/14945439/

one obstruction

many imlementation

very typical in sc

circuit implementation

and circuit

arch of this circuit will be on 
omplemntation
architecture of th

willbe oniy if two 
both relays are ratched
takes on one ratch

we dont deal with physical implementation

 "HDL file", "HDL program", and "HDL implementation" 

 "build a chip", "construct a chip", and "implement a chip" 

 "build a chip", "construct a chip", and "implement a chip" i

 That is, a stub file contains the chip name and the names of all the chip's input and output pins, without the chip's implementation,
also known as the "PARTS" section of the HDL program. 

Multiplexor select 
Demultiplexor 