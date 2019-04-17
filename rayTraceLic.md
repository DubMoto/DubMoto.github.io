## Enable select studio licenses (temporarily) in NX

The "NX Advanced FEM Bundle" includes two different "Studio" licenses.
To enable and utilize these licenses, the "Siemens PLM Software Licensing Tool" must be used to "apply" the bundle, enabling the licenses.

### Procedure for temporarily enabling this bundle:

1. Necessary to close other instances of NX before starting this procedure? untested.
2. Open licensing tool  
  - Windows 10, search for "licensing tool"  
2. From the "Available Bundles" column, select the `NX Advanced FEM` bundle, then select the arrow to move it to the "Applied Bundles" column.
2. From the "Applied Bundles" column, select the `NX Advanced FEM` bundle, then select `apply`.
2. Leave the Licensing Tool window open, while you start NX
2. Once NX is started, immediately un-apply that bundle, and closed the licensing tool. **<-- not obvious. Moving it back to "available" is the same as un-apply?**  

to be continued...  That will ensure that you will not automatically grab the FEM bundle, then next time that you start NX.
