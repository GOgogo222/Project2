### October 4th  
**LCD和LED引脚冲突**：非常得难受，不知道哪里出错了，整整卡了我两天, ps:其实主要是因为两天没碰单片机:)
### October 5th  
今天准备弄点单片机，弄点LeetCode，弄点数学  

**LCD与LED引脚冲突**：  

![image](https://github.com/GOgogo222/Project-2/blob/main/Exercise_log/Attachments/Pasted%20image%2020251005105126.png)
  
所以一开始就没碰过PD2？那我刚开始的功能是怎么做到的？无敌了，卡我三四个小时，记录一下。。。

![image](https://github.com/GOgogo222/Project-2/blob/main/Exercise_log/Attachments/da428a4a864740dfb451bff2ef502ebc.jpg)

爽了！

## October 7th
**救命，把CubeMX更新了一下，旧工程全消失了，一定要引以为戒**

## October 8th

![定时器内部结构](https://github.com/GOgogo222/Project-2/blob/main/Exercise_log/Attachments/%E5%AE%9A%E6%97%B6%E5%99%A8%E5%86%85%E9%83%A8%E7%BB%93%E6%9E%84.png)
**定时器内部结构**

![定时器比喻](https://github.com/GOgogo222/Project-2/blob/main/Exercise_log/Attachments/%E5%AE%9A%E6%97%B6%E5%99%A8%E6%AF%94%E5%96%BB.png)
**定时器比喻**

![定时器频率_周期公式](https://github.com/GOgogo222/Project-2/blob/main/Exercise_log/Attachments/%E5%AE%9A%E6%97%B6%E5%99%A8%E9%A2%91%E7%8E%87_%E5%91%A8%E6%9C%9F%E5%85%AC%E5%BC%8F.png)
**定时器公式**

![系统时钟内部结构](https://github.com/GOgogo222/Project-2/blob/main/Exercise_log/Attachments/%E7%B3%BB%E7%BB%9F%E6%97%B6%E9%92%9F%E5%86%85%E9%83%A8%E7%BB%93%E6%9E%84.png)
**系统时钟内部结构**


## October 13th

![PWM&PWM模块&信号发生器](https://github.com/GOgogo222/Project-2/blob/main/Exercise_log/Attachments/PWM%26PWM%E6%A8%A1%E5%9D%97%26%E4%BF%A1%E5%8F%B7%E5%8F%91%E7%94%9F%E5%99%A8.png)

**PWM&PWM模块&信号发生器**

| 项目       | 说明                 |
| -------- | ------------------ |
| CNT      | 定时器计数器，控制 PWM 周期   |
| ARR      | 决定周期长度，影响 PWM 频率   |
| CCR      | 控制高电平宽度，占空比核心      |
| OC 模块    | 自动控制 GPIO 输出高低电平   |
| PSC      | 时钟分频器，调节计数速度       |
| PWM 模式   | PWM1/PWM2，决定高低电平逻辑 |
| 输出到 GPIO | 最终信号输出到引脚          |
| DMA/中断   | 可选，自动更新占空比或响应事件    |

**PWM模块**

|函数|参数|作用|说明|
|---|---|---|---|
|`HAL_TIM_Base_Start()`|&htim|启动计数器 CNT|计数器模式，普通定时器，无 PWM 输出|
|`HAL_TIM_PWM_Start()`|&htim, TIM_CHANNEL_x|启动 CNT + 指定通道 OC 输出 PWM|通道参数告诉定时器哪个 OC 模块连接 GPIO 输出|


**两个参数:CNT+指定通道OC**


![STM32系统架构图](https://github.com/GOgogo222/Project-2/blob/main/Exercise_log/Attachments/STM32%E7%B3%BB%E7%BB%9F%E6%9E%B6%E6%9E%84%E5%9B%BE.jpg)

### STM32系统架构图



## October 16th

**今天学习了串口通信和adc转换器，很轻松的感觉**



## October 17th

**今天开始学习 *江协科技***  

![工程架构](https://github.com/GOgogo222/Project-2/blob/main/Exercise_log/Attachments/%E5%B7%A5%E7%A8%8B%E6%9E%B6%E6%9E%84.png)

![工程架构（2）](https://github.com/GOgogo222/Project-2/blob/main/Exercise_log/Attachments/%E5%B7%A5%E7%A8%8B%E6%9E%B6%E6%9E%84%EF%BC%882%EF%BC%89.png)

### STM32的工程架构


![句柄是什么](https://github.com/GOgogo222/Project-2/blob/main/Exercise_log/Attachments/%E5%8F%A5%E6%9F%84%E6%98%AF%E4%BB%80%E4%B9%88.png)

### 句柄

![什么是中断函数](https://github.com/GOgogo222/Project-2/blob/main/Exercise_log/Attachments/%E4%BB%80%E4%B9%88%E6%98%AF%E4%B8%AD%E6%96%AD%E5%87%BD%E6%95%B0.png)

### 中断函数

## October 18th

**宏定义 #define和typedef->专门针对数据类型的改名**

![指针的定义](https://github.com/GOgogo222/Project-2/blob/main/Exercise_log/Attachments/%E6%8C%87%E9%92%88%E7%9A%84%E5%AE%9A%E4%B9%89.png)

**指针的定义**

![强制类型转换的_星号](https://github.com/GOgogo222/Project-2/blob/main/Exercise_log/Attachments/%E5%BC%BA%E5%88%B6%E7%B1%BB%E5%9E%8B%E8%BD%AC%E6%8D%A2%E7%9A%84_%E6%98%9F%E5%8F%B7.png)

**强制类型转换的_星号**

## October 19th

https://chat.deepseek.com/share/u0kl5gkivour06bfvs

**关于优先级的分组问题**

## October 21th

![关于频率](https://github.com/GOgogo222/Project-2/blob/main/Exercise_log/Attachments/%E5%85%B3%E4%BA%8E%E9%A2%91%E7%8E%87.png)

**总线的频率问题**


## October 24th

- 学会了如何使用OLED显示屏
- 学会了用光敏传感器加蜂鸣器
- 连接了旋钮编码器等基本电路

## October 25th

- 了解了EXIT外设和中断系统的基本结构
- 实现了RCC,GPIO,AFIO,EXTI和NVIC的初始化配置
- （注：中断函数要在Start文件中找,判断标志位+清除标志位，类似于**new**的用法）

## October 26th

- 实现了旋转编码器计次 
- BUG: Num = Encoder();   // 所以显示器一直为0000 

![PWM基本结构](https://github.com/GOgogo222/Project-2/blob/main/Exercise_log/Attachments/PWM%E5%9F%BA%E6%9C%AC%E7%BB%93%E6%9E%84.png)

**PWM基本结构**

## October 28th

### 今天主要学习内容为ADC

- 什么是 *A* - *D* - *C* (模拟信号 Analog，数字信号 Digital，转换器 Converter)
- 什么是模拟信号（连续的，无穷的），数字信号（离散的）
- 采样深度的概念/分辨率的概念（例如12位的ADC,就是将0~3.3V的电压分成 *2^12-1（4035）* 份 ）
- 了解逐次逼近型的ADC的运行原理(流程：采样->保持 *（采样保持电路)* -> 量化 -> 编码)，学习到其中二分法的思想，可以与放砝码的过程作类比
- 复习了ADC外围电路的相关知识，电位器可调电压电路，传感器输出电压电路和简易电压转换电路

![ADC外围电路](https://github.com/GOgogo222/Project-2/blob/main/Exercise_log/Attachments/ADC%E5%A4%96%E5%9B%B4%E7%94%B5%E8%B7%AF.png)

**ADC外围电路**

## October 29th

- 初识USART和DMA

## November 1th


| 层级        | 示例               | 估计数量       | 概率（约）      | 概率换算      |
| --------- | ---------------- | ---------- | ---------- | --------- |
| 留名于任何史料   | 地方志人物、墓志铭、家谱     | 10,000,000 | 0.0085%    | 1/1,200 万 |
| 有百科或可检索档案 | 维基百科、国家档案、学术数据库  | 1,700,000  | 0.00015%   | 1/70 万    |
| 全球公认的知名人物 | 改变历史的政治家、科学家、艺术家 | 50,000     | 0.0000043% | 1/2,000 万 |
### "青史留名"



- 学到了I2C通信，但有敷衍了事之嫌，接下来要反复巩固

### DMA

- **DMA就是个数据搬运工**，你告诉它数据在哪儿，数据有多少，数据搬往哪儿等信息，就会开始按照你说的进行数据搬运工作。
- 落实到具体的参数就是：
- **数据宽度**：一个字节，半个字，一个字
- **地址是否自增**：Peripheral/Memory
- **优先级**：Low/Medium/High/Very High
- **循环模式**：适用于与ADC的连续转换模式协同操作,由**自动重装寄存器**控制
- **数据数量**：“并且搬运数量为ADC通道数”
- ——参考keysking【STM32】关于DMA那些事

**DMA的搬运区域就只有**外设**和**存储器**俩地方，且方向也被限定了**
- 外设-->存储器
- 存储器-->外设
- 存储器-->存储器

**【STM32F1】内部的存储器**
- **ROM-只读寄存器**：非易失性，掉电不丢失的寄存器
- **RAM-随机寄存器**：易失性，掉电丢失的寄存器

![RAM和ROM](https://github.com/GOgogo222/Project-2/blob/main/Exercise_log/Attachments/RAM%E5%92%8CROM.png)

**RAM和ROM**

- 通常情况下Flash存储器不可写入，作为DMA的目标寄存器会出错！

**“所以外设和存储器两个站点，就都有三个参数”**
- 起始地址
- 数据宽度（Byte/Halfword/Word）
- 地址是否自增

**“软件触发和循环模式不可同时使用，因其速度快的特性，软件触发比较适合从存储器到存储器的转运”**



## November 2th

了解了各个通信接口的特性，USART,I2C,SPI,CAN和USB
- **引脚
- **双工（全双工/半双工）
- **时钟（异步/同步）
- **电平（单端/差分）
- **设备（点对点/多设备）

“总结一下就是TX引脚输出定时翻转的高低电平，RX引脚定时读取引脚的高低电平。每个字节的数据加上起始位，停止位，可选的校验位，打包成数据帧，依次输出在TX引脚，另一端RX引脚依次接收，这样就完成了一个字节数据的通信”

“串口就是靠这样约定好的波形来进行通信的”

串口参数，我们最常用的就是：
- 波特率，9600/115200
- 数据位8位
- 停止位1位
- 无校验

数据寄存器DR(Data Register)

**一个物理引脚可以有多种功能，GPIO只是它可能承担的其中一种功能。**

“这里可以看到，在每个数据位的中间，都有一个时钟上升沿，时钟的频率和数据速率也是一样的，**接收端可以在时钟上升沿进行采样**”

- **单工**：一根线，只能一个发一个接
- **全双工**：两根线，两个都能发都能接 
- **半双工**：一根线，两个都能发

## November 4th

**完整过了各章的概念部分，仍需加强，实践

## November 8th

- 复习了GPIO架构图
- 复习了TIM定时器架构图
- 熟悉了CubeMX的基本操作

## November 9th

- 单片机核心板PCB：学会了元器件的放置

## November 10th

- 回看**TIM定时器**的输入捕获/输出比较部分
- 回看ADC工作原理
- 实现LED呼吸灯

## November 12th

- 编码器接口相当于是为实际单元提供了一个时钟

## November 13th

- 实现编码器测速
- 实现输入捕获测频率&占空比

## November 17th

- 重新理解时钟：时钟比较好理解，时钟是单片机的脉搏，时钟频率决定了单片机运行一个指令周期的时。。就好像我们做广播体操的时候 广播上喊的节拍1234 2234 3234。。。。然后我们全部的同学就按照这个节奏进行一个个动作，节拍越快我们动作越快，节拍越慢我们动作的越慢。
- 迟滞比较：设置两个阈值，一个下阈值，一个上阈值，用于输出抖动的问题，常见的有施密特触发器等
- **DMA转运三条件：**①计数器大于0；②触发源有触发信号（若为软件触发可忽略此条件）；③DMA使能

## November 19th

- **STM32硬件自动化：** "各个外设相互连接，互相交织，不再是传统的一个CPU，单独控制多个独立的外设"
- **USART框图部分：** 在程序上数据寄存器只表现为一个：数据寄存器DR；在硬件上表现为两个：用于"T"的发送数据寄存器，用于接受"R"的接受数据寄存器
- “**波特率发生器**其实就是**分频器**”

- 起始位侦测，不理解。。。

- **关于USART GPIO口模式的选择：** “TX引脚是USART外设控制的输出脚，所以选复用推挽输出；RX引脚是USART外设控制的输入脚，所以选择输入”

**“输入模式并不分普通输入，复用输入”**

**“一个引脚只能有一个输出，但可以有多个输入，所以输入脚，外设和GPIO都可以使用！！！”**


## November 20th

- **串口使用printf和sprinrf:** 
- 	printf("Num=%d\r\n",666);(需要重新定义底层的fputc函数)
- 	sprintf(String,"Num=%d\r\n",666); （更强大，指定打印位置【String数组】，不涉及重定向的东西）

**************************************
### 解决串口信息乱码问题

“所以总结一下就是，要么Keil和串口助手都选择UTF8，且Keil加上 **--no--multibyte-chars** ”
"要么都使用GB开头的中文编码格式"

******************************

- 数据包：把数据打包成一个整体，一次性发送

*********************************

### I2C总线

- **开漏输出：** "开漏输出呢，就是去掉这个强上拉的开关管，输出低电平时，下管导通，是强下拉；而输出高电平时，由于上拉开关管被去除，此时引脚处于浮空状态"
- “串口时序是**低位先行**，I2C是**高位先行**”
- **I2C通信原理：** “接受一个字节：SCL低电平期间，从机将数据位依次放到SDA线上（高位先行），然后释放SCL，主机将在SCL高电平期间读取数据位，所以SCL高电平期间SDA不允许有数据变化，依次循环上述过程8次，即可接受一个字节（主机在接受前，需要释放SDA）”
- **六块拼图：** 起始/终止条件， 发送/接受一个字节，发送/接受应答（0表示应答，1表示非应答）
- **从机地址7位+读写位1位（0表示写入，1表示读取）= 一个字节8位**
- **“套话”：** 
- ①“对于指定设备（Slave Address）,在当前地址指针指示的地址下，读取/写入从机数据（Data）” 
- ②“对于指定设备（Slave Address）,在指定地址（Reg Address）下，读取/写入从机数据（Data）” 

**总结：** 想象主机或从机在控制SDA/SCL的过程就是不停在“拉杆子”，这个杆子由一个轻质弹簧连接，你不拉他他就往上弹，但是一旦被拉就肯定被拉“下来”了，只不过是谁来拉，怎么拉，拉多久的问题

## November 21th

**************************

**实践部分：**
1. TXD和RED引脚接反程序不会有任何反应
2. Serial_SendByte()函数写错，导致一连串的函数SendString(),SendArray()...等函数也不中用了。毕竟像这种更高级的函数不过是SendByte()的叠加罢了

*********************************

### MPU6050:6轴姿态传感器
### 6/9/10轴姿态传感器

- 6轴：3轴加速度和3轴角速度
- 9轴：3轴加速度，3轴角速度和3轴磁场强度
- 10轴：3轴加速度，3轴角速度，3轴磁场强度和1个气压强度

 "MPU6050由三轴加速度计和三轴陀螺仪组成，它可以测量物体在x、y、z三个方向上的加速度和角速度。加速度计可以检测物体的线性加速度，而陀螺仪可以检测物体的角速度。通过将加速度计和陀螺仪的测量结果进行组合，可以计算出物体的方向和角度。"
——知乎博主

“加速度传感器的静态稳定性更好，但在运动时其数据相对不可靠，而陀螺仪的动态稳定性更好，但在静止时数据相对不可靠。所以，可以通过加速度传感器的输出来修正陀螺仪的漂移误差。

机体坐标系与地面惯性坐标系之间的夹角就是飞行器的姿态角，又称为欧拉角。
”
——CSDN

MPU6050所测得的数据**角速度**和**加速度**都可测欧拉角

加速度计/陀螺仪**满量程选择，** 值越大，分辨率越高

从机地址的三种表现方式：0x68  0xD0和1101 000

“XCL和XDA,通常是用于外接**磁力计**或**气压计**使得MPU6050的主机接口可以直接访问这些拓展芯片的数据”

**MPU6050内部的DMP单元**：用于数据融合和姿态解算

r(roll)滚转角
p(pitch)俯仰角
y(yaw)偏航角



*****************************

