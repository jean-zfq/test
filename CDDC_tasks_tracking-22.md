## 2024年6月24日 第26周例会  任务看板

### 一【W3K集成测试环境开发】
####  1.	ATE测试软件需求梳理√
####  2. 架构设计（Xuan）

####  3. 详细设计 （Zehao）

#####  3.1.    基础框架搭建

- [x] console组件移植与修改   

 - [x] lua解释器   

 - [x] 版本控制机制   

#####  3.2. 模块实现
- [x] spi模块   
- [x] common模块
- [x] mem模块    
  - [x] compare改进(可打印2片空间的不同)  
- [x] emmc/sd模块   
- [ ] ddr模块 
  
  > （ddr pll配置函数/ddr初始化流程/training通过 Ok）   
  
- [ ] log模块     

  - [x] 分级控制实现   

##### 3.3. 初审分享会  √

##### 3.4. 模块测试  
- [ ] DDR 测试   

  > （ 1.单次测试的内存大小不能超过32K, 否则测试会失败 ）

####    4. 文档输出

- [ ]  《ATE设计文档.md》

- [x] 《W3K SOC 验证系统.md》 

- [x] 《ATE固件软件实现架构.md》  

- [x] 《ATE固件开发指南.md》   

- [x] 《ATE固件用户手册.md》   



### 二 【PPE模块调研】（Team）

> （PPE/Qos/HNAT/NSS） 

####  1. 竞品处理流程分析

##### 1.1. MTK (Richard)

- [x] MT7981 （HNAT/IPV4）开源代码分析   
- [ ] BPI平台测试  （根据DPDK进行测试） 

##### 1.2. Qualcomm (Deon)

- [ ] NSS-PPE代码分析 
##### 1.3. NSS分析 √（Xuan）《ppe.pdf》
> （架构，数据流，功能模块）

- [ ]  描述符整理    （Tx/Rx/VLAN/Tso/QinQ/Timestamp?）

##### 1.4. 应用场景分析

- [ ] 基于CMCC 测试文件提取关于PPE的的要求（ACL/Qos）

#### 2. NetFPGA（PPE）原型分析 （Sai）

##### 2.1. NetFPGA测试环境搭建

> （因Full-Source- Package 无法从GitHub下载，切换到FPGA-Plus平台） 

- [x]  自建仿真环境   
    
    > （netfpga工程代码，删除路由功能外的其他模块）  
    > （当前状态：device id读取以及寄存器读写，配置接口功能正常；数据流已通过GMII接口到达路由模块）  
- [ ]  路由模块配置  
- [ ]  功能仿真

##### 2.2. NetFPGA- [x]Plus测试环境搭建
- [x] bit文件生成完成 √ 


### 三【竞品封装委外分析 】
(MT7981/MT7986/W3KMPW, MA-Tek, )   
#### 1.    非破坏性测试（X-ray/OM）√
#### 2.    破坏性测试
#### 3.    封装技术调研（Kai）  


### 四【W3KMPW验证】
> (CPU Core/DDR/Flash/EMMC/SD/PCIe/Jesd204B/GMAC/ADC/DAC/测试工具/操作系统)

#### 1. GMAC速率测试（VU13P FPGA）

（SNPS MAC + Xilinx PHY）<br>

#####  1.1.   FPGA代码准备 (Sai)√

#####  1.2.   测试用例(Xuan)

- [x] 读写功能、DMA 、PTP、AXI

#####  1.3.   测试工作(Xuan)

#### 2. GMAC速率测试（W3KMPW）

#### 3. I2C  接口测试 
- [x] I2C接口测试（W3KMPW，GDB test script） (Dan) √ 
- [ ] I2C接口测试（FPGA，IIC duty cycle issue fix） (Dan)  
 
 > （查找无法读出寄存器的数据的原因，提供bit文件再继续测试）

#### 4. PCIE验证（Team）  √
- [x] bar地址读写  
- [x] DMA功能  

#### 5. NAND flash 驱动开发（Lingsong）  
##### 5.1 spi   
 - [x] 驱动设计 
 - [ ] 功能验证 
   - [x] reset功能
   - [x] 读取id
   - [x] 读写状态寄存器
##### 5.2 qspi


### 五【W3KMPW问题总结】

#### 1.  Cache coherency (Richard/Xuan)

#### 2.  eMMC读写问题 （Zehao） √

#### 3.  I2C duty cycle (Dan)

 - [ ] I2C接口调试,问题定位中 (Sai)  

   > 问题定位：APB2IIC信号抓取分析（IIC0的scl正常运行；IIC1没有时钟） (Judy)  

#### 4.  JESD204B 多lane 读写问题 (Sai)   


### 六【W3KMPW动态路由板测试】
####  1.   测试问题调试
- [x] 打流测试时0.85V Core电压掉电问题已解决(Yawen)      

  > （更换RL电阻为4.4k,补偿电容为470PF，160M下上行发包正常）

#### 2.   双频合一测试分析（Deon）

#### 3.   吞吐率测试分析（Kai）



### 七【路由器吞吐率测试环境搭建】

####  1. STA陪测设备调试（Dan）√

####  2. 吞吐测试√（Yawen） （5G &2.4G ）


### 八【OpenWrt功能完善】
#### 1.   GMAC 驱动移植（Richard）√

- [x] 动态板串口乱码问题已解决√   

  > （原因：波特率不对；措施：设置波特率为105700）  

- [x] DVT GMAC调试  

  > （当前状态：gmac和phy连接OK； 网速测试百兆OK； 千兆接收情况下出现panic的问题已解决OK（千兆：接收为200Mbps，发送为312Mbps））



### 九【W3K FPGA development】

#### 1.   APB到MDIO的通讯接口设计 （Judy）



### 十【电路板维护】

#### 1. FPGA

#####  1.1.   

#### 2. DVT

#####  2.1.

#### 3. 动态路由板   

#####  3.1.   动态板Rework导致以太网无法使用问题暂未解决       √

> （原因：变压器的问题；措施：重焊变压器未解决）   

