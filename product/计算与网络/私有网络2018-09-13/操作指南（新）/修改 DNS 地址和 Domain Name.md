动态主机设置协议（Dynamic Host Configuration Protocol，DHCP）是一种局域网的网络协议， 提供了将配置信息传递到 TCP / IP 网络服务器的标准。
腾讯云私有网络内的云服务器支持 DHCP 协议，支持配置的 DHCP Options 字段包括：DNS 地址、Domain Name。您可在私有网络配置 DNS 地址和 Domain Name，该配置将对该私有网络下的所有云服务器生效。

>?
- 2018年4月1日前创建的私有网络暂不支持 DHCP 特性，若您在控制台无法修改 DNS 地址和 Domain Name，即说明您的私有网络不支持该特性。
- 为了保证配置修改后及时生效，已有的云服务器需重启机器或 dhclient。

## 操作步骤
1. 登录 [腾讯云控制台](https://console.cloud.tencent.com/) ，选择【云产品】>【网络】>【私有网络】，进入私有网络控制台。
2. 单击需要修改的私有网络 ID，进入详情页，即可在基本信息内配置 DNS 地址和 Domain Name。
 - DNS 地址
	 - DNS 最多支持4个 IP，IP 之间请用逗号隔开。
	 - DNS 可以指定4个 IP，但某些操作系统可能无法支持4个 DNS 地址。
	 - 腾讯云默认 DNS 为：`183.60.83.19`，`183.60.82.98`。如不使用腾讯云默认 DNS，将无法使用内部服务，如 Windows 激活、NTP、YUM 等。
 - Domain Name
	 - 云服务器 hostname 后缀，如`example.com`。

![](https://main.qcloudimg.com/raw/b6c45b1894296513876be194d7ba086d.png)

