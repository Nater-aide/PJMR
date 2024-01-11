# Analyzing a reverse shell

NEVER GET BOGGED DOWN IN THE FINER DETAILS

1. Run Floss utility against the file
2. Check in PE Studio
3. Run remnux with inetsim running
4. Run wireshark
5. Detonate file

You may not see everything in the static analysis. This is due to the strings being built at the time of execution. Dynamic analysis and wireshark will show you this  

If you get a domain name/A record, you can update your host file to point to your local machine
1. Open Cmder as administrator
2. nano C:\Windows\System32\drivers\etc\hosts
3. add 127.0.0.1 and the domain name
4. Launch procmon
5. set Process Name (name of binary) and Operation (to TCP)
6. run

1. Open terminal
2. run ```nc -nvlp 443```
