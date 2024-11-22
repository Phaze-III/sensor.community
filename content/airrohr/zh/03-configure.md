---
title: Configure
---
### Get the unique station ID
1. 将管理平台连接到USB电缆上，为传感器供电。

2. 管理站将尝试连接到配置的 WiFi 网络。对于新的设置，连接将失败，管理站将创建一个名称为 "颗粒物ID"、"Feinstaubsensor-ID "或 "airRohr-ID "的WiFi网络。这个ID就是**芯片ID**（例如13597771）。**请记下这个数字，因为您将需要它来进行登记**。

3. 在电脑或智能手机上连接到台建立的WiFi网络。默认密码是“airrohrcfg”。<br>*安卓*.等待，直到建立连接。如果立即断开连接，您可能需要停用 "连接->WiFi->高级 "下的 "智能网络开关 "选项。

4. 打开浏览器，输入[http://192.168.4.1/](http://192.168.4.1/)。

> ⚠️ **请注意**NodeMCU可能需要几次尝试才能连接到家庭WiFi网络。請耐心地嘗試幾次，直到成功為止。如果传感器的配置成功，站内WiFi网络将不可用，配置页面将不再以该IP 192.168.4.1访问。

### Configure the station
1. 在 "配置 "页面中输入你的SSID（家庭WiFi网络名称）、网络安全密钥（Windows下）或WiFi密码。

2. 如果您使用的是推荐的微尘传感器(SDS011)，则无需进一步更改配置。

3. 点击 "保存配置并重新启动 "按钮。管理站将重新启动，当它连接到您的家庭WiFi网络时，将不再以这种方式访问。

<br>

<img src=".../docs/airrohr_config_initial.jpg" loading="lazy"/>

<br>

###验证台站的配置是否正确。
如果您在上一步中除了WiFi网络配置外没有做其他更改，传感器现在将开始记录和上传数据。您可以通过导航到以下页面来验证每项工作是否正常，大约10分钟后。在这些页面上搜索芯片ID（在上面的例子中是13597771）。

* [传感器数据](https://www.madavi.de/sensor/graph.php)
* [WiFi信号数据](https://www.madavi.de/sensor/signal.php)
