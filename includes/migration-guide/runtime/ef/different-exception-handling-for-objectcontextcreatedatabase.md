### <a name="different-exception-handling-for-objectcontextcreatedatabase-and-dbproviderservicescreatedatabase-methods"></a>不同的例外狀況處理 ObjectContext.CreateDatabase 和 DbProviderServices.CreateDatabase 方法

|   |   |
|---|---|
|詳細資料|從 .NET 4.5 開始，如果資料庫建立失敗，<code>CreateDatabase</code> 方法會嘗試卸除空白資料庫。 如果該作業成功，則會傳播原始 <xref:System.Data.SqlClient.SqlException?displayProperty=name> (而不是在 .NET 4.0 中一律擲回的 <xref:System.InvalidOperationException?displayProperty=name>)|
|建議|攔截時<xref:System.InvalidOperationException?displayProperty=name>執行時<xref:System.Data.Objects.ObjectContext.CreateDatabase>或<xref:System.Data.Common.DbProviderServices.CreateDatabase(System.Data.Common.DbConnection,System.Nullable{System.Int32},System.Data.Metadata.Edm.StoreItemCollection)>，SQLExceptions 應該現在也攔截。|
|範圍|次要|
|版本|4.5|
|類型|執行階段|
|受影響的 API|<ul><li><xref:System.Data.Objects.ObjectContext.CreateDatabase?displayProperty=nameWithType></li><li><xref:System.Data.Common.DbProviderServices.CreateDatabase(System.Data.Common.DbConnection,System.Nullable{System.Int32},System.Data.Metadata.Edm.StoreItemCollection)?displayProperty=nameWithType></li></ul>|

