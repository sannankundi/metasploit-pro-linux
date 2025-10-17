# metasploit-pro-linux

1. This is a cracked version of Metasploit Pro for Linux. The version is 4.22.2.
2. The setup is pretty simple. Download the release zip file.
3. Sudo install the bin file(lol). Then execute(./) the "_inst.sh" file.
4. After that is done, you're good to go.

BUT you may encounter a problem. I will not go into what the error is specifically because I forgot(😅).

BUT here's the fix:

In the metasploit folder that will be in /opt, you'll have to run "ctlscript.sh restart" or maybe you'll have to sudo it.

This will restart all the related services to make metasploit pro work correctly.

Now, the last thing you may have to do is... you can setup...(I forgot dumb stuff a lot) the script to run at startup using Cron.

Here's what you gotta do in terminal:

`sudo crontab -e`
then add this line(presuming you installed in /opt/metasploit)
`@reboot /opt/metasploit/ctlscript.sh`

## To Use

Type `msfpro` in terminal to work in cli mode. OR just go to the specific port you used for it in a web browser. E.g. https://localhost:3790
