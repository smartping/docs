#配置说明
SmartPing从0.3.0版本开始，配置可以使用WEB界面修改。

## 配置修改节点
![](/assets/changeconfig.png)

进行修改后，左上角输入密码即可生效（默认密码为smartping）

##　备注
- 首次运行SmartPing时，SmartPing默认优先读取conf/config.json文件，若无此文件，则读取conf/config-base.json文件
- 若需要修改密码，需要手工修改conf/config.json或conf/config-base.json文件中的password字段，并重启SmartPing