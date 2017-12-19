# pubkeyphishy


Simple phishing page functionality in PHP that will take harvested credentials and then encrypt them with your public key, and then write them to a file for later retrieval with your private key.

Useful for a scenario where you host a phishing page on a VPS that you don't *totally* control, and want at least some peace of mind for credential storage, versus just letting them sit on the filesystem in cleartext.

Don't know of many harvesters that do this but then again, I didn't bother looking too hard. Any excuse to write something silly like this is good enough for me.

shoutout to my homeboi dash1b.

# 
