Logs here are written to standard out, as normal.
But you can also see them in a datagrid, in the app!
Logs are also sent to a ring buffer that caches the last dozen so logs.
The ring buffer has a synchronized view so that the UI is notified as logs are added and pushed out.

Tech Stack:
- [Cysharp's ObservableCollections](https://github.com/Cysharp/ObservableCollections)
- [Serilog](https://github.com/serilog/serilog)
- [Avalonia.Controls.TreeDataGrid](https://github.com/AvaloniaUI/Avalonia.Controls.TreeDataGrid)
- [native aot](https://learn.microsoft.com/en-us/dotnet/core/deploying/native-aot/?tabs=net8plus%2CmacOS)
- [xaml hot reload](https://github.com/Kir-Antipov/HotAvalonia)
