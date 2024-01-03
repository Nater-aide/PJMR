# Packing malware
Packing is an encrpytion mechanism to make malware look different than its source.  

UPX -- popular packing program.
1. Take piece of malware
2. UPX is going to blow it up. It will put a packer stub
3. The compression stub is going to take the code that is located below a point, and crunch it down.
4. When Compressed, the resulting program looks alot smaller into 3 parts
   - Original header
   - The compression stub
   - tiny piece of code
 5. The stub looks at the small piece of code and expands it
 6. When it inflates, it can go back to original state and bypass AV

Look for LoadLibraryA and GetProcAddress -- two api calls used to identify other imports at runtime  
