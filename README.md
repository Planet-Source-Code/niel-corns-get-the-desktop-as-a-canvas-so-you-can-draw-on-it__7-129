<div align="center">

## Get the desktop as a CANVAS \(So you can draw on it\!\)


</div>

### Description

Want to draw on the desktop like a Canvas? You can now! Simply use the proecedre below!
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Niel Corns](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/niel-corns.md)
**Level**          |Advanced
**User Rating**    |3.8 (23 globes from 6 users)
**Compatibility**  |Delphi 5, Delphi 4
**Category**       |[Windows API Call/ Explanation](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/windows-api-call-explanation__7-39.md)
**World**          |[Delphi](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/delphi.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/niel-corns-get-the-desktop-as-a-canvas-so-you-can-draw-on-it__7-129/archive/master.zip)





### Source Code

```
function windowsDesktopCanvas: TCanvas;
var
  DC: HDc;
begin
   DC := getWindowDC ( GetDeskTopWindow );
   result := TCanvas.Create;
   result.Handle := DC;
end;
```

