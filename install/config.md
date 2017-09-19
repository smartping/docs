#配置说明
SmartPing从0.3.0版本开始，配置可以使用WEB界面修改。

## 配置修改节点
![](/assets/changeconfig.png)

- 目标类型只支持 C 或 CS ， C即为Client模式，目标节点只接收PING数据包，CS模式即Client&Server模式，目标节点既接收PING数据包同时也发送PING数据包。

- 报警规则为每分钟进行一次检测，若在**检测时间范围(Check Period)**内出现**发生次数(Occur Times)**以上，丢包率高于**丢包率(Loss Percent)**或延迟高于**平均延迟(Average Delay)**则报警,默认报警保存 **存档天数(Archive Days)** 日。

- 进行修改后，左上角输入密码即可生效（默认密码为smartping）

##　备注
- 首次运行SmartPing时，SmartPing默认优先读取conf/config.json文件，若无此文件，则读取conf/config-base.json文件
- 若需要修改密码，需要手工修改conf/config.json或conf/config-base.json文件中的password字段，并重启SmartPing