#Conversion of part units
NX 12.0, Windows 10

1. Open command prompt  
2. Navigate to C:\Program Files\Siemens\NX 12.0\NXBIN

Using "Windows powershell"  
start menu > type "powershell" > [enter] to select "Windows PowerShell" app  
`cd 'C:\Program Files\Siemens\NX 12.0\NXBIN\'`

Using "Command Prompt"  
start menu > type "shell" > [enter] to select "Command Prompt" app  
`cd "Program Files\Siemens\NX 12.0\NXBIN"`

```
usage: ug_convert_part [options]

options:
  [-in <filename>]    converts file <filename> to inches
  [-mm <filename>]    converts file <filename> to millimeters
  [-d]                sets the current directory as the source
  [-d <dirname>]      sets directory <dirname> as the source
  [-o <dirname>]      sets existing directory <dirname> as the destination
  [-s]                traverses subdirectories
  [-u]                converts udf files
  [-uo]               converts udf files only
  [-x]                exports the expressions of the converted part
  [-y]                converts entire assembly
```

examples (PowerShell):
```
PS C:\Program Files\Siemens\NX 12.0\NXBIN> .\ug_convert_part.exe -mm 'M:\caduser\cwiggins\project\clas12_study\nx\in\svt_study.prt'

NX Units Conversion Program

Opening: M:\caduser\cwiggins\project\clas12_study\nx\in\svt_study.prt
Converting: M:\caduser\cwiggins\project\clas12_study\nx\in\svt_study.prt
 Conversion SUCCESS
Saving: M:\caduser\cwiggins\project\clas12_study\nx\in\svt_study.prt
Looking for config file: tessUG.config
Looking for config file: tess.config
Looking for config file: C:\Program Files\Siemens\NX 12.0/pvtrans/tessUG.config .... Found!
Translator Log File created at: C:\temp\svt_study.log

1 file successfully converted
0 files generated warnings
0 files failed to convert
```
In addition to unit-configuration and filename, the following command defines input (-d) & output (-o) paths
```
PS C:\Program Files\Siemens\NX 12.0\NXBIN> .\ug_convert_part.exe -mm 'M:\caduser\cwiggins\project\clas12_study\nx\in\svt_study.prt'

```

examples (Command Prompt):
```
C:\Program Files\Siemens\NX 12.0\NXBIN>ug_convert_part.exe -mm "M:\caduser\cwiggins\project\clas12_study\nx\in\svt_study_orig_mm.prt"

NX Units Conversion Program

Opening: M:\caduser\cwiggins\project\clas12_study\nx\in\svt_study_orig_mm.prt
Converting: M:\caduser\cwiggins\project\clas12_study\nx\in\svt_study_orig_mm.prt
*** WARNING: no conversion required

1 file required no conversion
0 files successfully converted
0 files generated warnings
0 files failed to convert
```
In addition to unit-configuration and filename, the following command defines input (-d) & output (-o) paths
```
C:\Program Files\Siemens\NX 12.0\NXBIN>ug_convert_part.exe -mm "svt_study_orig_mm.prt" -d "M:\caduser\cwiggins\project\clas12_study\nx\in" -o "M:\caduser\cwiggins\project\clas12_study\nx"
```

Right-click component > properties > [units] to verify unit conversion