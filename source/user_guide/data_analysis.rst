数据分析
================

软件能够对采集到的数据进行实时的计算和统计分析，数据计算采用模块化方式构建计算模型实现，使用者能够搭建各种计算模型。另外，还可以通过python语言构建自定义的计算模块实现各种自定义算法。

统计分析
----------------

软件内置了多种统计算法，可以通过选择的方式快速配置统计分析结果。

统计算法
^^^^^^^^^^^

软件内置以下统计算法：
 
- Min，最小值
- Max，最大值
- Min_X，最小值对应X值
- Max_X，最大值对应x值
- Mean，平均值
- Median，中值
- Range，范围
- Peak，峰值
- Sum，算术和
- Std Dev，标准差
- COV，循环变动
- RMS，有效值
- Peak Factor，峰值系数，peak/RMS
  
统计配置
^^^^^^^^^^^^

1. 点击功能栏上的 **统计计算设置** 按钮，打开统计设置视图
   
.. figure:: /images/statistic_wnd.png
    :width: 600px
    :alt: statistic window
    :align: center
    :name: img_statistic_wnd

    统计设置窗口

2. 勾选或取消勾选复选框，可以添加或删除统计结果
3. 单击选择数据，数据名称变为 **粗体** 表示选中。可以用 **Shift** 或 **Ctrl** 进行批量多选。
4. 如果需要批量添加统计结果，单击需要添加统计的 **列标题** ，对应的复选框会变为选中状态，表示选择完成。如 :numref:`img_statistic_wnd_add` 所示，选择CH2、CH3后，单击 **Mean列标题** ，则增加了CH2和CH3的 **Mean** 计算结果。如果需要取消的话则再次单击Mean列标题。

.. figure:: /images/statistic_wnd_add.png
    :width: 600px
    :alt: statistic window add
    :align: center
    :name: img_statistic_wnd_add

    添加统计算法
    
5. 点击 **保存** 按钮保存配置
6. 打开数据选择窗口，可以看到数据列表中已经有了添加的计算结果
   
.. figure:: /images/data_select_after_add_statistic_config.png
    :width: 600px
    :alt: data select after add statistic
    :align: center
    :name: img_data_select_after_add_statistic_config

    数据选择窗口增加了统计结果


计算模型
----------------

为了能够灵活构建数据分析算法及流程，软件采用了图形化构建计算模型的方式来进行数据分析。

打开模型视图
^^^^^^^^^^^^^^^^

- 点击功能栏上的 **计算模型视图** 按钮，打开计算模型视图

.. figure:: /images/model_wnd.png
    :width: 600px
    :alt: model window
    :align: center
    :name: img_model_wnd 

    计算模型视图

- 计算模型视图包括三部分

    + 工具条，修改模型的快捷工具
    + 模块库，软件内置的计算模块（c++）或自定义计算模块（python）
    + 模型区域，显示和编辑模型


新建模型
^^^^^^^^^^^^^^^^

1. 点击工具栏的 **新模型** 按钮来创建新模型
2. 从模块库的 **Port** 组中将 **source** 和 **result** 拖放到模型区域

.. figure:: /images/model_add_source.png
    :width: 300px
    :alt: model window add source
    :align: center
    :name: img_add_source

    计算模型添加模块

3. 从模块库的 **General** 组中将 **signal_stat** 拖放到模型区域
4. 连接各个模块，如 :numref:`img_model_demo` 所示

.. figure:: /images/model_demo.png
    :width: 300px
    :alt: model demo
    :align: center
    :name: img_model_demo

    计算模型示例
    
5. 点击模块左下角的三角符号，打开参数列表，修改source和result的名称如 :numref:`img_model_demo_rename` 所示。
   
.. figure:: /images/model_demo_rename.png
    :width: 300px
    :alt: model demo rename
    :align: center
    :name: img_model_demo_rename

    修改模块参数

6. 点击工具栏的 **保存模型** 按钮来创建保存模型，在保存对话框中输入模型名称，点击 **确定** 按钮保存模型文件，同时模型文件也会自动添加到试验中。模型文件的扩展名是 **.bpm**。
   
.. figure:: /images/save_model.png
    :width: 200px
    :alt: save model
    :align: center
    :name: img_save_model

    保存模型后自动添加到试验

7. 在 **试验视图** 中的模型名称上点击右键，选择 **启用** 菜单项，当模型名称变为 **粗体** 后表示模型已经启用了。

.. figure:: /images/model_active.png
    :width: 200px
    :alt: model active
    :align: center
    :name: img_model_active

    启用模型

8. 打开数据选择窗口，可以看到数据列表中已经有了添加的模型计算结果 **rms1** 和 **mean1**
   
.. figure:: /images/data_select_after_add_model.png
    :width: 600px
    :alt: data select after add model 
    :align: center
    :name: img_data_select_after_add_model

    数据选择窗口增加了模型计算结果
    

模块库
----------------

模块库中的计算模块分为两类：

- 内置计算模块，由C++实现，计算速度块
- 自定义计算模块，由python实现，计算速度比C++慢，优点是使用方便、扩展性好，能够使用各种python的库