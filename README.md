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

要求：
LCD1602显示时钟，按K3键进入时钟设置，此时秒钟停止走动；
按K1键选择设置的秒、分、时、日、月、星期、年；
按K2键进行加1，设置完成后，再次按下K3键继续走时

