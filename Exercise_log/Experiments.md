![[Pasted image 20251130160144.png]]

Step1:锁存器（PD2）置高电平

Step2:将相应的GPIO口置低电平

Step3:锁存器（PD2）置低电平

![[Pasted image 20251130161418.png]]

将PCX和PD2置高电平,上电一瞬间，锁存器就是可写入状态，PCX以高电平形式接入LED负端（熄灭状态）

![[Pasted image 20251130162721.png]]

创建一个自己写代码的文件，熟悉几个常用的头文件

![[0ed783d2835af7449fd88715fde12fe9.jpg]]

![[Pasted image 20251130165102.png]]

将PC8口置低电平，成功点亮LED1

