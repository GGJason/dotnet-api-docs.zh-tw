### <a name="some-net-apis-cause-first-chance-handled-entrypointnotfoundexceptions"></a>某些.NET Api 原因第一個可能發生的 （處理） EntryPointNotFoundExceptions

|   |   |
|---|---|
|詳細資料|在.NET Framework 4.5，少量的.NET 方法皆已開始擲回第一個可能發生<xref:System.EntryPointNotFoundException?displayProperty=name>s。 這些例外狀況在 .Net Framework 中已處理，但可能會中斷未預期第一個可能發生例外狀況的測試自動化。 這些相同的 API 會在啟用 HighVersionLie 時中斷一些 ApiVerifier 案例。|
|建議|您可以升級至 .NET Framework 4.5.1 來避免此錯誤 (bug)。 或者，可以測試自動化更新成第一個可能發生在不中斷<xref:System.EntryPointNotFoundException?displayProperty=name>s。|
|範圍|Edge|
|版本|4.5|
|類型|執行階段|
|受影響的 API|<ul><li><xref:System.Diagnostics.Debug.Assert(System.Boolean)?displayProperty=nameWithType></li><li><xref:System.Diagnostics.Debug.Assert(System.Boolean,System.String)?displayProperty=nameWithType></li><li><xref:System.Diagnostics.Debug.Assert(System.Boolean,System.String,System.String)?displayProperty=nameWithType></li><li><xref:System.Diagnostics.Debug.Assert(System.Boolean,System.String,System.String,System.Object[])?displayProperty=nameWithType></li><li><xref:System.Xml.Serialization.XmlSerializer.%23ctor(System.Type)?displayProperty=nameWithType></li></ul>|

