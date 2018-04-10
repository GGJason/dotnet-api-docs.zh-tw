### <a name="xslt-style-sheet-exception-message-changed"></a>變更的 XSLT 樣式表例外狀況訊息

|   |   |
|---|---|
|詳細資料|在.NET Framework 4.5 中，當 XSLT 檔太複雜時的錯誤訊息文字是&quot;樣式表太過複雜。&quot;在舊版中，錯誤訊息為&quot;XSLT 編譯錯誤。&quot;倚賴錯誤訊息文字的應用程式程式碼將無法運作。 不過，例外狀況類型會保持不變，因此這項變更應該不會產生實際影響。|
|建議|更新任何應用程式程式碼，根據來自這個錯誤狀況的例外狀況訊息，預期新的訊息，或 （更好的） 更新程式碼以只相依於例外狀況類型 (<xref:System.Xml.Xsl.XsltException?displayProperty=name>)，其中沒有變更。|
|範圍|Edge|
|版本|4.5|
|類型|執行階段|
|受影響的 API|<ul><li><xref:System.Xml.Xsl.XslCompiledTransform.Load(System.String)?displayProperty=nameWithType></li><li><xref:System.Xml.Xsl.XslCompiledTransform.Load(System.Type)?displayProperty=nameWithType></li><li><xref:System.Xml.Xsl.XslCompiledTransform.Load(System.Xml.XmlReader)?displayProperty=nameWithType></li><li><xref:System.Xml.Xsl.XslCompiledTransform.Load(System.Xml.XPath.IXPathNavigable)?displayProperty=nameWithType></li><li><xref:System.Xml.Xsl.XslCompiledTransform.Load(System.Reflection.MethodInfo,System.Byte[],System.Type[])?displayProperty=nameWithType></li><li><xref:System.Xml.Xsl.XslCompiledTransform.Load(System.String,System.Xml.Xsl.XsltSettings,System.Xml.XmlResolver)?displayProperty=nameWithType></li><li><xref:System.Xml.Xsl.XslCompiledTransform.Load(System.Xml.XmlReader,System.Xml.Xsl.XsltSettings,System.Xml.XmlResolver)?displayProperty=nameWithType></li><li><xref:System.Xml.Xsl.XslCompiledTransform.Load(System.Xml.XPath.IXPathNavigable,System.Xml.Xsl.XsltSettings,System.Xml.XmlResolver)?displayProperty=nameWithType></li></ul>|

