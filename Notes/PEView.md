# PEview
A portable executable is a giant array of bytes  
The first line of the file gives away the type of file that it is  

**Image File Header**  
1. Go to Image_NT_Headers>>Image_FILE_HEADER
2. This will have the time date stamp. This MAY tell you when it was compiled
3. Older time stamp may indicate maliciousness.
   -Boreland Delphi compiler will always have a timestamp of 1992

**Image Section Header**
1. Go to IMAGE_SECTION_HEADER .text section
2. Check the virtual size and size of raw data. These are written in hexidecimal
3. Use the hexidecimal calculator. Verify if the size is the same

**IMPORT Address Table**
1. Go to the section .rdata>>>IMPORT_ADDRESS_TABLE
2. Check for URLDownloadToFileW and ShellExecuteW
