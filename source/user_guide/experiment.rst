试验配置
--------------
本软件中的所有设置和数据都使用试验文件来组织和保存，在进行测试之前首先要新建或打开试验文件，试验文件的扩展名为 **exp**。

新建或打开试验
~~~~~~~~~~~~~~~~

新建试验
^^^^^^^^^^^^

点击 **文件** 按钮，如 :numref:`img-new_experiment-no_select` 所示：

.. figure:: /images/new_experiment-no_select.png
    :width: 600px
    :align: center
    :name: img-new_experiment-no_select

    新建试验

在 **新建** 页面有多个按钮能够新建不同类型的试验项目，包括 **新建试验** 、 **新建脚本** 、 **新建xxx试验** 等按钮及模板

    -  **新建试验** 按钮能够建立空试验，后续再添加试验使用的设备
    -  **新建脚本** 按钮能够建立空的python脚本，结合软件提供的API接口实现数据计算、自动控制等多种功能
    - 其他的按钮为针对各种设备的模板，能够再创建试验后自动添加设备、计算脚本、显示模板到试验中，然后可以直接开始测试

新建试验模板由python代码构成，可以自己构建所需的模板。

点击 **新建** -> **新建试验** 按钮，选择试验数据文件的保存目录，建议选择空目录，避免出现文件覆盖的问题。完成后在目录中会出现扩展名为 **exp** 的文件，这个文件包括了试验中所需的配置信息，再次试验时只需要重新打开试验文件就可以继续进行试验。

创建试验后可以在左侧功能栏点击 **试验视图** 按钮打开试验视图查看试验包括的内容, 如 :numref:`img_experiment_wnd` 所示。

.. figure:: /images/experiment_wnd.png
    :width: 400px
    :align: center
    :name: img_experiment_wnd

    试验视图内容

打开试验
^^^^^^^^^^^^^^

点击工具栏 **文件->打开** 按钮，如 :numref:`file_open` 所示：

.. figure:: /images/open_experiment.png
    :width: 600px
    :align: center
    :name: file_open 

    打开试验文件

打开试验包括两部分： **最近的文件** 和 **计算机文件** 。通过 **最近的文件** 能够快速打开最近打开过的试验；通过 **计算机文件** 能够浏览计算机中的试验文件并打开。


设备配置
~~~~~~~~~~~~~~~~

点击工具栏上 **更改设备** 按钮，打开设备管理窗口。如 :numref:`img_device_list_wnd` 所示。 

.. figure:: /images/device_list_wnd.png
    :width: 600px
    :align: center
    :name: img_device_list_wnd

    设备管理窗口


添加设备
^^^^^^^^^^^^^^

1. 添加设备

 - 在左侧 **设备列表** 中双击设备名称
 - 在左侧 **设备列表** 中单选或多选设备，点击上方 **添加** 按钮

2. 修改设备SN和IP地址

.. figure:: /images/set_sn_ip.png
    :width: 600px
    :align: center
    :name: set_sn_ip 

    添加设备并修改SN和IP


删除设备
^^^^^^^^^^^^^^

- 在 **已添加设备** 列表中选择待删除的设备，点击 **删除** 按钮

删除所有设备
^^^^^^^^^^^^^^

- 点击 **删除所有** 按钮

自动搜索设备
^^^^^^^^^^^^^^

1. 点击 **搜索** 按钮
2. 搜索到的设备会自动添加到 **已添加设备** 列表中



通道配置
~~~~~~~~~~~~~~~~

添加信号
^^^^^^^^^^^^^^

1. 在左侧工具栏点击 **通道设置** 按钮, 显示如 :numref:`img_channel_setting_wnd` 所示。

.. figure:: /images/channel_setting_wnd.png
    :width: 600px
    :align: center
    :name: img_channel_setting_wnd 

    通道设置视图
    
2. 根据 **Device_SN** 和 **Channel** 列单选或多选使用的通道, 然后点击工具栏 **添加** 按钮，软件会自动选择通道并创建对应的信号，根据连接的传感器信息修改 **Signal Name**、 **Unit** 、 **Factor** 和 **Offset** 等列的信息。然后点击工具栏 **保存** 按钮。
   

删除信号
^^^^^^^^^^^^^^

- 单选或多选需要删除的信号名称, 点击工具栏 **删除** 按钮删除所选的信号
  

复制粘贴信息
^^^^^^^^^^^^^^

1. 点击工具栏 **复制** 按钮能够复制通道信息到剪贴板，能够粘贴到excel中便于统一编辑信号信息
2. 在excel中编辑信号参数后，选择信号参数区域复制
3. 在通道视图中，在复制信息左上角对应单元格点击右键，选择 **Paste** ，将excel中编辑的信息粘贴到通道配置中
4. 点击工具栏 **保存** 按钮
   

.. figure:: /images/channel_setting_copy_paste.png
    :width: 600px
    :align: center
    :name: img_channel_setting_copy_paste

    通道设置视图