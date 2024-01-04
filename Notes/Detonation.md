# Initial Detonation & Triage: Hunting for Network Signatures
Make sure your tools are up and running while you are detonating. If this is the only copy of the sample, you will need to track down once more.

1. Run ```Inetsim``` in remnux
2. Launch wireshark ```sudo wireshark```

Use your static analysis info that was located to look for information within the dynamic testing.  
screenshot the packet(s) that are located

What to look for in wireshark  
1. detonate file
2. wireshark search query -- ```http.request.full_uri contains (info to search)```
