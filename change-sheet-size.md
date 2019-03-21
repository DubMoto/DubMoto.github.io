[ Back to index ](README.md)
# NX - CHANGE OUT SHEET SIZE
Changing an existing document border-format to another (ex: C-size to D-size).

### Process:
1. Isolate format layers; `CTRL-L` (Layer Settings).  
  2. Change Work Layer from 1 to 199 (or other empty layer) by double-clicking.  
  2. Shift-Select & turn off layers 1 – 247.
  2. Shift-Select and turn on layers 248 – 256.
2. Window-select (drag) & delete everything in current sheet.  

2. Edit Sheet / select new Sheet size.  
2. Import new format  
  File > Import > part  
    2. Uncheck `Create Named Group`
    2. Set Layer to `Original`
    2. Select Part from `TeamCenter`  

2. Search for `*noviews*` & choose size.  E templates are separated into “Major” (Sheet 1) and “Minor” (Sheets 2, etc.).  
2. Restore layers; `CTRL-L`
  2. Change Work Layer to Layer 1.
  2. Return Layers to original visibility settings or set visibility as needed.
  2. Set `format` layer to ‘Visible Only.’
  
[ Back to index ](README.md)
