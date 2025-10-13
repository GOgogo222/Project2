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

