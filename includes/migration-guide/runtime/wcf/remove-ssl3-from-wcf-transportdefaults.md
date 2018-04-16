### <a name="remove-ssl3-from-the-wcf-transportdefaults"></a>從 WCF TransportDefaults 移除 Ssl3

|   |   |
|---|---|
|詳細資料|當使用 NetTcp 搭配傳輸安全性和憑證類型的認證時，SSL 3 通訊協定已不再是用來交涉安全連接的預設通訊協定。 在大部分情況下應該不會影響到現有的應用程式為 TLS 1.0 一律已包含在通訊協定清單的 NetTcp。 所有現有的用戶端應該能夠使用至少 TLS 1.0 來交涉連接。|
|建議|如果需要 Ssl3，使用下列組態的機制的其中一個 Ssl3 加入交涉通訊協定清單。<ul><li><xref:System.ServiceModel.Channels.SslStreamSecurityBindingElement.SslProtocols></li><li><xref:System.ServiceModel.TcpTransportSecurity.SslProtocols></li><li>[<](~/docs/framework/configure-apps/file-schema/wcf/transport-of-nettcpbinding.md)</li><li>[&lt;sslStreamSecurity&gt; section of &lt;customBinding&gt;]~/docs/framework/configure-apps/file-schema/wcf/sslstreamsecurity.md)</li></ul>|
|範圍|Edge|
|版本|4.6.2|
|類型|執行階段|
|受影響的 API|<ul><li><xref:System.ServiceModel.Channels.SslStreamSecurityBindingElement.SslProtocols?displayProperty=nameWithType></li><li><xref:System.ServiceModel.TcpTransportSecurity.SslProtocols?displayProperty=nameWithType></li></ul>|
