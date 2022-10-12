
参考
============

设备配置文件格式
--------------------------
设备配置文件定义了设备的参数、通道数等信息。

.. figure:: /images/device_config_param.png
    :width: 300px
    :align: center
    :name: tool_file 

    设备配置文件格式

- ID：设备ID，用于标识参数
- Editable：是否可编辑，1表示能够编辑
- Name：参数名称
- CommonPropertyName：通用属性名称，例如所有通道都有输入信号类型，则可以设置Name为Input Type CH1，此参数设置为Input Type，在软件显示时会将多个通道的参数合并显示
- Unit：单位
- Type：INDEX表示是字典数据，INT表示为整数数值，FLOAT表示为浮点数值
- Description：描述
- ScaleUp：转换为发送数据时放大倍数
- ScaleDown：转换为发送数据时缩小倍数
- OutputBytes：发送/接收数据字节数
- SingleResponse：No Used
- Max：最大值
- Min：最小值
- AccessLevel：访问级别，0表示用户不可见，1表示用户可见
- Category：类别，在设备参数配置界面用来分类显示
- ValueContain：数值

  + ValuePhy：参数数值

    * V：表示数值的值
  + ValueEnum：字典数据值

    * VE：表示数值对应的字典值

