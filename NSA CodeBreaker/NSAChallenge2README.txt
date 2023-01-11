A2:
Looked for hidden files in root directory provided.
Found .cert.perm file from the root directory with ls -la. 
Uploaded it as an RSA key file for tls protocol in Wireshark.
Followed the trace of the one http packet that showed up (changed after adding the RSA key file).
Used the first plain text word that looked like a username. 
Flag: SoreWetCard
