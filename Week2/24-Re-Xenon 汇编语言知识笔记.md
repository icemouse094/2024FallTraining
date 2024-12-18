:::info
💡汇编语言是直接建立在硬件之上工作的编程语言

:::

章节小结

| **1.** | 汇编指令是机器指令的助记符，同机器指令一一对应 |
| --- | --- |
| **2.** | 每一种CPU都有自己的汇编指令集 |
| **3.** | CPU可以直接使用的信息在存储器中存放 |
| **4.** | 在存储器中指令和数据没有任何区别，都是二进制信息 |
| **5.** | 存储单元从0开始编号。 |
| **6.** | 一个存储单元可以存储8个bit，即8位二进制数 |
| **7.** | 1Byte=8bit 1KB=1024B  1MB=1024KB 1GB=1024MB |
| **8.** | 每一个CPU芯片都有许多管脚，这些管脚和总线相连。也可以说，这些管脚引出总线。一个CPU可以引出3种总线的宽度标志了这个CPU的不同方面的性能：<br/>(1)地址总线的宽度决定了CPU的寻址能力<br/>(2)数据总线的宽度决定了CPU与其他器件进行数据传送时的一次数据传送量<br/>(3)控制总线的宽度决定了CPU对系统中其他器件的控制能力 |


<h2 id="RqZ57">思维导图</h2>
> 用思维导图，结构化记录本章的核心观点。
>

![画板](https://cdn.nlark.com/yuque/0/2024/jpeg/49936975/1731677458452-f21fcabb-7810-4dfa-b79c-5d7f8e841378.jpeg)

<h2 id="HP1DO">在CPU中</h2>
+ 运算器进行信息处理
+ 寄存器进行信息存储
+ 控制器控制各种器件进行工作
+ 内部总线连接各种器件，在它们之间进行数据传递

<h3 id="FMxIe">通用寄存器</h3>
> 8086CPU的所有寄存器都是16位的，可以存放2个字节例如AX,BX,CX,DX等
>

同时这4个寄存器又可以分成两个独立的8位寄存器使用

如AX可以分成AH和AL；

<h3 id="HQOk8">汇编指令</h3>
> mov ax,18--将18送入寄存器AX--AX=18
>
> mov ah,78--将78送入寄存器AH--AH=78
>
> add ax,8--将寄存器AX的数值加上8--AX=AX+8
>
> mov ax,bx--将寄存器BX的数值送入寄存器AX--AX=BX
>
> add ax,bx--将AX和BX中的数值相加，结果存在AX中--AX=AX+BX
>

一般这里的数据更多使用十六进制数，可以直观表达



:::info
*一旦计算结果超出寄存器存储范围，那么最高一位可能会丢失

:::

知识小结

| 1. | 段地址在8086CPU的段寄存器中存放。当8086CPU要访问内存时，有段寄存器提供内存单元的段地址。8086CPU有4个段寄存器，其中CS用来存放指令的段地址 |
| --- | --- |
| 2. | CS存放指令的段地址，IP存放指令的偏移地址。<br/>8086机中，任意时刻，CPU将CS:IP指向的内容当成指令执行 |
| 3. | 8086机的工作过程：<br/>(1)从CS:IP指向的内存单元读取指令，读取的指令进入指令缓冲器；<br/>(2)IP指向下一条指令；<br/>(3)执行指令（再转回步骤1，重复该过程） |
| 4. | 8086CPU提供转移指令修改CS，IP的内容 |


<h3 id="ybjeV"></h3>
> 
>

<h2 id="UKgZ0"></h2>
+ <font style="color:#8C8C8C;"></font>
+ <font style="color:#8C8C8C;"></font>
+ <font style="color:#8C8C8C;"></font>

<h2 id="NRfzd">相关资料</h2>
> <font style="color:#8C8C8C;">可通过“⌘+K”插入引用链接，或使用“本地文件”引入源文件。</font>
>





