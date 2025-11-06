DRV8825-RS485 LabVIEW VISA Controller
--------------

&emsp;&emsp;
本项目基于LabVIEW VISA串口通信，基于DRV8825-RS485一体化步进电机驱动控制器的Modbus-RTU通讯协议，实现了部分功能的封装，以满足对步进电机的常规控制。

&emsp;&emsp;
常用功能vi以库文件形式封装进“DRV8825 Series.llb”中，目前封装的功能包括：

- DRV8825 VISA Init.vi&emsp;根据VISA资源初始化串口
- DRV8825 VISA Read.vi&emsp;向VISA串口写入数据(uint8格式)
- DRV8825 VISA Write.vi&emsp;从VISA串口读出数据(uint8格式)
- DRV8825 VISA Close.vi&emsp;关闭VISA串口
- DRV8825 Setting.vi&emsp;向保持寄存器写入设置的驱动参数
- DRV8825 Single Run.vi&emsp;驱动一次“单次运行”
- DRV8825 Single Run Status Check.vi&emsp;检查“单次运行”是否到位
- DRV8825 Continue Run.vi&emsp;驱动连续正转/反转
- DRV8825 Continue Stop.vi&emsp;停止连续正转/反转
- DRV8825 Immediately Stop.vi&emsp;电机急停
- CRC-16 MODBUS Check.vi&emsp;生成CRC-16/MODBUS校验位(2x uint8)

<br>&emsp;&emsp;
“demo_1 Single Run.vi”和“demo_2 Continuous Run.vi”文件是基于“DRV8825 Series.llb”实现的两个案例。“demo_1 Single Run.vi”实现特定运行长度的单次驱动；“demo_2 Continuous Run.vi”实现了持续正转/反转的驱动。

&emsp;&emsp;
关于DRV8825-RS485的具体使用说明，请参照“DRV8825-RS485使用说明V1.0.pdf”。

&emsp;&emsp;
本项目为个人所作，当前封装功能不全，仅满足手头使用需求。欢迎迭代升级、扩充及批评指正。
