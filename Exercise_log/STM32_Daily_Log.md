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

“总结一下就是TX引脚输出定时翻转的高低电平，RX引脚定时读取引脚的高低电平。每个字节的数据加上起始位，停止位，可选的校验位，打包成数据帧，依次输出在TX引脚，另一端RX引脚依次jie'shou”

