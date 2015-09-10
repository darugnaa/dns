# dns
List of addresses to include in a machine's "hosts" file for a better life.

The *hosts* file in **Windows** is located in the following path `%SystemRoot%\system32\drivers\etc\hosts`.
After editing the file (you will need Administrator's privileges) refresh the DNS cache with `ipconfig /flushdns`.

The *hosts* file in **OSX** is located in the following path `/etc/hosts`.  
The file can be edited from Terminal with `sudo vim /etc/hosts` or `sudo nano /etc/hosts`.


    # Block Spotify banner ads
    127.0.0.1     pubads.g.doubleclick.net
    127.0.0.1     securepubads.g.doubleclick.net
 
    # Block Skype banner ads
    127.0.0.1   rad.msn.com
    127.0.0.1   g.msn.com
    127.0.0.1   live.rads.msn.com
    
    # Google ADS
    127.0.0.1	partner.googleadservices.com

    # DoubleClick
    127.0.0.1	ad.doubleclick.net
    127.0.0.1	static.doubleclick.net
    127.0.0.1	partnerad.l.doubleclick.net
    127.0.0.1	pubads.g.doubleclick.net
    127.0.0.1	stats.g.doubleclick.net

    # General blocking
    127.0.0.1       b.scorecardresearch.com
    127.0.0.1       condenastitalia01.wt-eu02.net
    127.0.0.1       cx.atdmt.com
    127.0.0.1       sync.liverail.com
    127.0.0.1       tvzap.kataweb.it
    127.0.0.1       imageceu1.247realmedia.com
    127.0.0.1       pixel-geo.prfct.co
    127.0.0.1       secure.adnxs.com
    127.0.0.1       imp2.bizographics.com
    127.0.0.1       ad.crwdcntrl.net
    127.0.0.1       cdn.krxd.net
    127.0.0.1       cdn.gigya.com

I didn't include the following addresses (yet).  
List taken from http://superuser.com/questions/547807/how-to-disable-the-skype-ads-advertisement

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
`0.0.0.0` is a non-routable address http://superuser.com/a/592566
