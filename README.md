# Microcontroller-Project
这是一个在51单片机上运行的万年历项目，用于xcn的硬件综合实践的结课设计，可以通过它的测试样例

## 基本要求：    

电子万年历  

电路图：
不使用DS1302计时器模块，用软件逻辑实现计时功能。  

注意：
（1）	闰年闰月；   

（2）	时间和日期可以手工设置，星期随日期自动更新，无需手工设置  

（3）	计时准确性问题（定时器模式选择）  


    
按键：
K1-->P31
K2-->P30
K3-->P32
K4-->P33（该按键未做功能，大家可扩展）

  
**要求**：
LCD1602显示时钟，按K3键进入时钟设置，此时秒钟停止走动；
按K1键选择设置的秒、分、时、日、月、星期、年；
按K2键进行加1，设置完成后，再次按下K3键继续走时

  
## **给分标准**
  万年历（基准分85）  
  1.自主演示无错误 60分  
  2.测试61秒32天等非法数值 **（测试用例2021-13-32-25-61）** 70分  
  3.演示闰年（3个测试用例每个5分，全对85）  
  普通闰年：公历年份是4的倍数，且不是100的倍数的，为闰年（如2004年、2020年等就是闰年）。 **（测试用例2024 -2-29、1900-2-29 ）**  
  世纪闰年：公历年份是整百数的，必须是400的倍数才是闰年（如1900年不是闰年，2000年是闰年）。**（测试用例2000-2-29 ）**  
  4.k4键有额外设计的酌情加分（5-10分）  
  
## 项目运行方式  

  项目只有一个main.c文件，在keil5中进行编译，生成的.hex文件烧入单片机即可运行  
  具体的使用和其他教程可见下面这个B站课程：[51单片机入门教程](https://www.bilibili.com/video/BV1Mb411e7re?spm_id_from=333.788.videopod.episodes&vd_source=74f1f63aa5fd4c634b4f10ecaed1ff0e)   
  推荐看到6-2矩阵键盘密码锁这一节课，中间的4-1和4-2数码管的内容可以跳过（大约2天即可），学完便可以调试和修改本代码并通过结课答辩的提问  
  
