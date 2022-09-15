# Building a Solar Server 🌞

Running notes on how to build a solar server from the perspective of someone that's never built a server or anything solar powered.

---

## Getting Solar Power 🔌

This seems fairly straight forward but will have unforseen issues I'm sure if I ever actually give it a shot.

* get a solar panel with a charge controller
* the charge controller regulates the output power
* hook this up (directly?) to a car battery
* get a power inverter to convert dc to ac power
* hook this up (directly?) to the car battery
* you now have normal ac power

---

## Making a Simple Website 📄

This might be a more a stylistic choice than anything else but it will limit the power it takes to service a request. Also Lowtech Magazine is a really inspiring solar powered server project so going through their advice on low-tech web design might provide unforseeable insight.

[link to full article](https://solar.lowtechmagazine.com/2018/09/how-to-build-a-lowtech-website/)

* a charge controller directly hooked up to a server via usb
* battery maybe optional

#### Why a Low-tech Website?
* lowtech design meant to radically reduce server energy use
* internet meant to [dematerialise society and decrease energy use](https://www.bcg.com/publications/2012/energy-environment-technology-industries-smarter-2020-role-ict-driving-sustainable-future.aspx)
* internet is a [large / growing consumer of energy](https://solar.lowtechmagazine.com/2015/10/can-the-internet-run-on-renewable-energy.html)
* the internet uses three times more energy than all current wind and solar power (source?)
* almost all pv solar panels are produced in china
* chinese energy grid is twice as carbonized and half as effecient as europe's
* web content is becoming increasingly resource intensive
* video and website size is to blame
* average web page was .45 MB in 2010 and 1.7-2.9 MB in 2018
* average mobile 'page weight' was .15 MB in 2011 to 1.6 MB in 2018
* [growth in web traffic surpasses increases in energy efficiency](https://www.researchgate.net/publication/224224694/download)
* heavier / larger sites also shorten hardware lifetimes
* manufacturing computers is [extremely energy-intensive](https://solar.lowtechmagazine.com/2009/06/embodied-energy-of-digital-technology.html)
* mobile devices create the need for an 'always-on' internet
* always-on internet access accompanies a cloud computing model
* cloud computing model decreases user device energy consumption but increases data center and network energy use
* once offline activities like file access now often require network access

#### Low-tech Web Design
