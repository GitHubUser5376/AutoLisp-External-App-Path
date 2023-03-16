# AutoLisp-External-App-Path

To use this code, load it into a cad application. Call the code with "(fcnAppPath [extension (string)] )" and use an extension associated with a valid application. By default, if a drawing extension of "dwg" or "dwt" is supplied, the cad application execution path and executable is returned. If a Microsoft product extension is recognized, then the associated application path and executable is used, and if a "pdf" extension is used, then Adobe's is path and executable is returned. If either an invalid extension is supplied or the associated application is not found in the regristry, then the function will return nil as the output.

This function does not start, modify, or close the external applications; it only supplies the path and name to them. Additional conditions may need to be added to the code if the desired application is not found. 
