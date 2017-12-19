# pubkeyphishy


Simple phishing page functionality in PHP that will take harvested credentials and then encrypt them with your public key, and then write them to a file for later retrieval with your private key.

Useful for a scenario where you host a phishing page on a VPS that you don't *totally* control(who trusts 'em, right?), and want at least some peace of mind for credential storage, versus just letting them sit on the filesystem in cleartext.

Don't know of many harvesters that do this but then again, I didn't bother looking too hard. Any excuse to write something silly like this is good enough for me.

shoutout to my homeboi dash1b.
works with PHP 5.x to current(7.0.x at this time)

# pubkeycrypt.php
Functionality outlined above

# pubdcrypt.php
This is the script that will decode and then decrypt the harvested data from the results file. It will print the decrypted results out in a *username, pass* format. Should go without saying that your private key shouldn't be on the same host as pubkeycrypt.php(something something about storing the key with the lock). 
