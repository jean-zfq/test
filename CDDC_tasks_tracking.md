## 2024年6月24日 第26周例会  任务看板

### 一【W3K集成测试环境开发】

#### &emsp; 1.	ATE测试软件需求梳理√

#### &emsp; 2. 架构设计（Xuan）

​           *-《ATE设计文档.md》*

`程序 层v出v出vCBB`

`https://github.com/jean-zfq/test/blob/main/CDDC_tasks_tracking.md`

[git](https://github.com/jean-zfq/test/blob/main/CDDC_tasks_tracking.md)

[baidu](https://www.baidu.com/)

> 卡迪仓库
>
> 陈小姐才能



[百度](https://www.baidu.com/)

1. 您的
2. 机电局
3. 打开
4. 多少

5. 层
小程序 
小程序



- 效率惊喜你参加先看下
- 形成
- 小程序
- 总线



- [x] 你的
- [x] 技术
- [x] jshcjb

![](D:\Profiles\Pictures\Screenshots\屏幕截图 2024-06-19 174843.png)

#### &emsp; 3. 详细设计 （Zehao）

##### &emsp;&emsp; 3.1.    基础框架搭建

&emsp;&emsp;&emsp; - console组件移植与修改√ 
&emsp;&emsp; &emsp;- lua解释器√  

##### &emsp;&emsp; 3.2. 模块实现

&emsp;&emsp;&emsp;-	spi模块√ 
&emsp;&emsp;&emsp;-    common模块√  
&emsp;&emsp;&emsp;-	mem模块√  
&emsp;&emsp;&emsp;-	emmc/sd模块√  
&emsp;&emsp;&emsp;-	ddr模块  
&emsp;&emsp;&emsp;**（ddr pll配置函数/ddr初始化流程/training通过 Ok）**  

##### &emsp;&emsp;3.3. 初审分享会 √



### 二 【PPE模块调研】（Team）

&emsp;（PPE/Qos/HNAT/NSS） 
#### &emsp; 1. 竞品处理流程分析
##### &emsp;&emsp;1.1. MTK (Richard)
&emsp;&emsp;&emsp;- MT7981 开源代码分析 √  
&emsp;&emsp;&emsp;- BPI平台测试  （根据DPDK进行测试） 

##### &emsp;&emsp;1.2. Qualcomm (Deon)
&emsp;&emsp;&emsp;- NSS-PPE代码分析 

#### &emsp;&emsp;1.3. NSS分析 √（Xuan）

​             -《ppe.pdf》  

&emsp;&emsp;&emsp;（架构，数据流，功能模块）
#### &emsp;&emsp;1.4. 应用场景分析 
#### &emsp;2. NetFPGA（PPE）原型分析 （Sai）

##### &emsp;&emsp;2.1. NetFPGA测试环境搭建

&emsp;（因Full-Source-Package 无法从GitHub下载，切换到FPGA-Plus平台）

##### &emsp;&emsp;2.2. NetFPGA-Plus测试环境搭建

&emsp;&emsp;&emsp;- bit文件生成完成 √ 


### 三【竞品封装委外分析 】

&emsp;(MT7981/MT7986/W3KMPW, MA-Tek, )   
#### &emsp;1.    非破坏性测试（X-ray/OM）√
#### &emsp;2.    破坏性测试

#### &emsp;3.    封装技术调研（Kai）  


### 四【W3KMPW验证】
&emsp;(CPU Core/DDR/Flash/EMMC/SD/PCIe/Jesd204B/GMAC/ADC/DAC/测试工具/操作系统)

#### &emsp;1. GMAC速率测试（VU13P FPGA）

&emsp;（SNPS MAC + Xilinx PHY）

##### &emsp;&emsp; 1.1.   FPGA代码准备 (Sai)√

##### &emsp;&emsp; 1.2.   测试用例(Xuan)

&emsp;&emsp;&emsp;- 读写功能、DMA 、PTP、AXI
##### &emsp;&emsp; 1.3.   测试工作(Xuan)  
#### &emsp;2. GMAC速率测试（W3KMPW）
#### &emsp;3. I2C  接口测试 
&emsp;&emsp;&emsp;- I2C接口测试（W3KMPW，GDB test script） (Dan) √  
&emsp;&emsp;&emsp;- I2C接口测试（FPGA，IIC duty cycle issue fix） (Dan)    
&emsp;&emsp;&emsp; （查找无法读出寄存器的数据的原因，提供bit文件再继续测试）
#### &emsp;4. PCIE验证（Team）  √
&emsp;&emsp;&emsp;- bar地址读写√   
&emsp;&emsp;&emsp;- DMA功能√  
#### &emsp;5. NAND flash 驱动开发（Lingsong）  
&emsp;&emsp;&emsp;- spi   
&emsp;&emsp;&emsp;- qspi   

### 五【W3KMPW问题总结】
#### &emsp;1.  Cache coherency (Richard/Xuan)
#### &emsp;2.  eMMC读写问题 （Zehao）√

#### &emsp;3.  I2C duty cycle (Dan)
&emsp; &emsp;- I2C接口调试,问题定位中 (Sai)  
#### &emsp;4.  JESD204B 多lane 读写问题 (Sai)   


### 六【W3KMPW动态路由板测试】
#### &emsp; 1.   测试问题调试
&emsp;&emsp;- 打流测试时0.85V Core电压掉电问题已解决(Yawen)  √     

（更换RL电阻为4.4k,补偿电容为470PF，160M下上行发包正常）

#### &emsp;2.   双频合一测试分析（Deon）  
#### &emsp;3.   吞吐率测试分析（Kai）



### 七【路由器吞吐率测试环境搭建】
#### &emsp; 1. STA陪测设备调试（Dan）√    
&emsp;&emsp;2. 吞吐测试√（Yawen） （5G &2.4G ）  


### 八【OpenWrt功能完善】
#### &emsp;1.   GMAC 驱动移植（Richard）  
&emsp;&emsp;&emsp;- 动态板串口乱码问题已解决√   
&emsp;&emsp;&emsp;&emsp;（原因：波特率不对；措施：设置波特率为105700）  
    

&emsp;&emsp;&emsp;- 动态板软件无法使用问题未解决       
&emsp;&emsp;&emsp;&emsp;（原因：变压器的问题；措施：重焊变压器未解决）  


&emsp;&emsp;&emsp;- DVT GMAC调试  
&emsp;&emsp;&emsp;&emsp;（当前状态：gmac能和phy正常连接<br>
&emsp;&emsp;&emsp;&emsp;  问题：cache一致性的问题/出现tx timeout的问题/gmac的中断未上来/pcs和phy的连接状态无法link，打印，tx/rx状态是错误的）  



### 九【W3K FPGA development】
#### &emsp;1.   APB到MDIO的通讯接口设计 （Judy）

### 十【测试】●

#### &emsp;1. 测试01（XXX）

#### &emsp;2. 测试02（XXX）





