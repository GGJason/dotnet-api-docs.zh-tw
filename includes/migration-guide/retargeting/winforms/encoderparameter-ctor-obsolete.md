### <a name="encoderparameter-ctor-is-obsolete"></a>EncoderParameter ctor 已過時

|   |   |
|---|---|
|詳細資料|<xref:System.Drawing.Imaging.EncoderParameter.%23ctor(System.Drawing.Imaging.Encoder,System.Int32,System.Int32,System.Int32,System.Int32)> 建構函式現在已淘汰，如果使用，就會產生建置警告。|
|建議|雖然<xref:System.Drawing.Imaging.EncoderParameter.%23ctor(System.Drawing.Imaging.Encoder,System.Int32,System.Int32,System.Int32,System.Int32)>建構函式將繼續運作，應該改為使用下列建構函式，以避免重新編譯使用.NET 4.5 工具的程式碼時的過時的建置警告： <xref:System.Drawing.Imaging.EncoderParameter.%23ctor(System.Drawing.Imaging.Encoder,System.Int32,System.Drawing.Imaging.EncoderParameterValueType,System.IntPtr)>。|
|範圍|次要|
|版本|4.5|
|類型|正在重定目標|
|受影響的 API|<ul><li><xref:System.Drawing.Imaging.EncoderParameter.%23ctor(System.Drawing.Imaging.Encoder,System.Int32,System.Int32,System.Int32,System.Int32)?displayProperty=nameWithType></li></ul>|

