# Gtouch
G touch就是一个把普通显示屏改造为触控屏的项目，该装置可为电脑、投影等设备增加触屏的功能。他需要的仅仅是一个对应系统的驱动以及一个轻松固定可随时拆卸的小型外部装置。通过红外激光发射器扫描屏幕表面，手指放上去之后加了滤光片的摄像头即能捕捉到手指的反射的红外光，将其转化为二值图后通过算法把亮斑转化为单点的坐标，配合驱动通过校准程序得到的屏幕坐标转化参数矩阵将其映射到电脑屏幕上对应的坐标值，与前几帧的数据进行对比判断是否为单击，双击，长按或是上滑下拉，最后通过相应的Windows API触发对应事件。 这种触屏加装技术是目前市面上所没有的，G touch的出现填补了当前技术与市场的空白，相信其小巧的身躯与强大的多设备适应性再配上亲民的价格，一定会让这个世界触手可及!