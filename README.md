# dns

I switched from manually editing my local hosts file to using [Pi-hole](https://pi-hole.net/). Pi-hole is a [DNS sinkhole](https://en.wikipedia.org/wiki/DNS_sinkhole) that runs on local hardware (for example a Raspberry-Pi or an old laptop). The advantage is that it can block ads and tracking for all other devices in your local network. Exactly, that means smartphones too!

[Pi-hole](https://pi-hole.net/) offers cool stats, a one click "block this domain" functionality and general peace of mind as it has a big list of denied trackers. Combined with a browser like [Vivaldi](https://vivaldi.com/) it makes the modern web less annoying.

## Why should I do this?
I recommend reading ["The Age of Surveillance Capitalism: The Fight for a Human Future at the New Frontier of Power"](https://www.goodreads.com/book/show/26195941-the-age-of-surveillance-capitalism) by Soshana Zuboff. It's an accurate description of what is happening: we are tracked online and offline to be sold as "data" to create personalized advertisement to modify our behavior.  
I am not against online ads per se, but the privacy invasion is huge. I like my privacy.

An easier-to-digest alternative is ["The Great Hack"](https://www.netflix.com/title/80117542) on Netflix about the scandal of Cambridge Analytica and Facebook.

## Previous content
List of addresses to include in a machine's "hosts" file for a better life.

The *hosts* file in **Windows** is located in the following path `%SystemRoot%\system32\drivers\etc\hosts`.
After editing the file (you will need Administrator's privileges) refresh the DNS cache with `ipconfig /flushdns`.

The *hosts* file in **OSX** is located in the following path `/etc/hosts`.  
The file can be edited from Terminal with `sudo vim /etc/hosts` or `sudo nano /etc/hosts`.


    ## Invasive Adware
    # Block Spotify ads blocker (video + banner)
    0.0.0.0 ads.pubmatic.com
    0.0.0.0 spclient.wg.spotify.com
    0.0.0.0 www.googletagservices.com
    0.0.0.0 pubads.g.doubleclick.net
    0.0.0.0 securepubads.g.doubleclick.net
    0.0.0.0 gads.pubmatic.com
 
    # Block Skype banner ads
    127.0.0.1   rad.msn.com
    127.0.0.1   g.msn.com
    127.0.0.1   live.rads.msn.com
    127.0.0.1   apps.skype.com
    # SKYPE NEW  7.27.64.101
    127.0.0.1   s0.2mdn.net
    127.0.0.1   s1.2mdn.net
    127.0.0.1   ad.doubleclick.net
    127.0.0.1   secure.adnxs.com
    127.0.0.1   ib.adnxs.com
    127.0.0.1   pixel.alephd.com
    127.0.0.1   cdn.at.atwola.com
    # SKYPE NEW  7.30.64.105
    127.0.0.1    sgreen.erne.co
    127.0.0.1    dps.bing.com
    
    # BitComet (torrent client)
    127.0.0.1	inside.bitcomet.com
    
    ## Tracking/ads/unwanted content
    # Google ADS
    127.0.0.1	partner.googleadservices.com

    # DoubleClick
    127.0.0.1	ad.doubleclick.net
    127.0.0.1	static.doubleclick.net
    127.0.0.1	partnerad.l.doubleclick.net
    127.0.0.1	pubads.g.doubleclick.net
    127.0.0.1	stats.g.doubleclick.net
    127.0.0.1   cm.g.doubleclick.net

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
    127.0.0.1     aka-cdn-ns.adtech.de
    127.0.0.1     secure.flashtalking.com
    127.0.0.1     cdn.atdmt.com


### 127.0.0.1 vs 0.0.0.0
Which value to use? I'm doing some research on the topic.  
`127.0.0.1` is the local machine itself.
`0.0.0.0` is a non-routable address http://superuser.com/a/592566
