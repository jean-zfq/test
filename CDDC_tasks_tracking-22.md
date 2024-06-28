## 2024年6月24日 第26周例会  任务看板

### 一【W3K集成测试环境开发】

####  1.	ATE测试软件需求梳理√
####  2. 架构设计（Xuan）

####  3. 详细设计 （Zehao）



数学公式
$$
(a+b)/2=a/2+b/2
$$


 表格

| 姓名 | 年龄 | 班级 |
| :--- | :--: | ---: |
|      |      |      |

脚注：

一件三联[^三联]

---



三个横线加横线  ---

---



----搜索引擎

[修真苑](https://ic.coachip.cn/article/list/6"一个搜索引擎")

---引用链接

[百度][id]

[id]：https://www.baidu.com/“一个搜索引擎”

请参考[标题一](#一【W3K集成测试环境开发】)

【8分钟让你快速掌握Markdown】 https://www.bilibili.com/video/BV1JA411h7Gw/?share_source=copy_web&vd_source=8d53cc5bcce210b9519b851b05bdb786

ULR:

https://www.bilibili.com/



图片

![鲜花](https://www.baidu.com/"百度")




##### 5.2 qspi

1. bcnv 
   1. cxh  -[ ] 
      1. - [x] lkslc
      2. 
2. 
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

---

#### 5. NAND flash 驱动开发（Lingsong）  
##### 5.1 spi

 - [x] 驱动设计 

 - [ ] 功能验证 
   - [x] reset功能
   
   - [x] 读取id
   
   - [x] 读写状态寄存器
   
       

```c



### 五【W3KMPW问题总结】

#### 1.  Cache coherency (Richard/Xuan)

#### 2.  eMMC读写问题 （Zehao） √

#### 3.  I2C duty cycle (Dan)

 - [ ] I2C接口调试,问题定位中 (Sai)  

   - [ ] >  问题定位：APB2IIC信号抓取分析（IIC0的scl正常运行；IIC1没有时钟） (Judy)  


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


[^三联]:点赞，收藏，投币






