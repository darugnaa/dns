# dns
List of addresses to include in a machine's "hosts" file for a better life.

The *hosts* file in **Windows** is located in the following path `%SystemRoot%\system32\drivers\etc\hosts`.
After editing the file (you will need Administrator's privileges) refresh the DNS cache with `ipconfig /flushdns`.

The *hosts* file in **OSX** is located in the following path `/etc/hosts`.  
The file can be edited from Terminal with `sudo vim /etc/hosts` or `sudo nano /etc/hosts`.


    # Block generic ads
    0.0.0.0     ad.doubleclick.net
    
    # Block Spotify banner ads
    0.0.0.0     pubads.g.doubleclick.net
    0.0.0.0     securepubads.g.doubleclick.net
 
    # Block Skype banner ads
    0.0.0.0     rad.msn.com
    0.0.0.0     g.msn.com

I didn't include the following addresses (yet).  
List taken from http://superuser.com/questions/547807/how-to-disable-the-skype-ads-advertisement

    127.0.0.1     live.rads.msn.com
    127.0.0.1     ads1.msn.com
    127.0.0.1     static.2mdn.net
    127.0.0.1     ads2.msads.net
    127.0.0.1     a.ads2.msads.net
    127.0.0.1     b.ads2.msads.net
    127.0.0.1     ac3.msn.com
    127.0.0.1     ec.atdmt.com
    127.0.0.1     msntest.serving-sys.com
    127.0.0.1     sO.2mdn.net
    127.0.0.1     aka-cdn-ns.adtech.de
    127.0.0.1     secure.flashtalking.com
    127.0.0.1     cdn.atdmt.com
    127.0.0.1     apps.skype.com

### 127.0.0.1 vs 0.0.0.0
Which value to use? I'm doing some research on the topic.  
`127.0.0.1` is the local machine itself.
