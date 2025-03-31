# StormMonaco - Tutorial

## Firstly you can check out my Tutorial on YouTube

https://www.youtube.com/watch?v=omDBpgKnIlo&t=5s

## Written info (same like in the vid)

=== NuGet Packs ======
- `WebView2`
- `Newtonsoft.Json`

=== References =======
- Your based API (Based on Nezur or Xeno)

=== Bin ==============
- Nezur bin (my case)
- Xeno

=== Monaco + Tab + AutoSave Link

https://mrnoxy.github.io/StormMonaco/

=== Clear button =====
```csharp
await webView23.ExecuteScriptAsync("SetText('');");
```
=== Execute button ===
```csharp
var result = await webView23.ExecuteScriptAsync("GetText();");
// Use JsonConvert to deserialize the string (removes escaping and extra quotes automatically)
string cleanResult = JsonConvert.DeserializeObject<string>(result);
SpaceAPIb.API.Execute(cleanResult); // Use ur own API call function.
```
