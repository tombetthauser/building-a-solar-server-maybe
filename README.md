# Building a Solar Server 🌞

Running notes on how to build a solar server from the perspective of someone that's never built a server or anything solar powered.

---

## 1. Get Solar Power 🔌

This seems fairly straight forward but will have unforseen issues I'm sure. It seems like it's just a $100 amazon solar panel with a standard built-in charge controller hooked up to a car battery hooked up to a standard $60 power inverter for a car hooked up to whatever old laptop is running the server. Could it be that simple?

<details>
<summary><strong>
  More Solar Power Notes
</strong></summary><br>

* get a solar panel with a charge controller
* the charge controller regulates the output power
* hook this up (directly?) to a car battery
* get a power inverter to convert dc to ac power
* hook this up (directly?) to the car battery
* you now have normal ac power

</details>

---

## 2. Make a Simple Website 📄

In a nutshell, making your website small saves power. To make a small website no react, no javascript, dither your images, default serif font, no google analytics, no cookies, no ads.

[link to full article on lowtech magazine](https://solar.lowtechmagazine.com/2018/09/how-to-build-a-lowtech-website/)
  
<details>
<summary><strong>
  Hardware Observations
</strong></summary><br>
  
* a charge controller directly hooked up to a server via usb
* battery maybe optional
  
<br></details>

<details>
<summary><strong>
  Why a Low-tech Website?
</strong></summary><br>

* lowtech design meant to radically reduce server energy use
* internet meant to [dematerialise society and decrease energy use](https://www.bcg.com/publications/2012/energy-environment-technology-industries-smarter-2020-role-ict-driving-sustainable-future.aspx)
* internet is a [large / growing consumer of energy](https://solar.lowtechmagazine.com/2015/10/can-the-internet-run-on-renewable-energy.html)
* the internet uses three times more energy than all current wind and solar power (?)
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
  
<br></details>

<details>
<summary><strong>
  Lowtech Web Design
</strong></summary><br>
  
* the internet is not an autonomous being
* rising power consumption comes from choices web developers make
* converting a basic blog to a lowtech design decreases average page size by a factor of five
* average page weight is .77 MB
* less than half the page weight of the average site in 2018
* number of requests has also been decreased fivefold
* dowload speed has increased tenfold
* site is designed for low energy use not speed
  
<br></details>

<details>
<summary><strong>
  Static Site
</strong></summary><br>
  
* building a static site was a fundamental move
* most websites build pages on the fly after querying a database
* every request (repeats included) is generated on demand
* static sites generate pages once
* then static files live on the server's hard disk
* static sites are based on file storage
* dynamic sites depend on recurrent computation
* static sites require less processing power and less energy (?)
* a normal blog site like lowtech magazine would take up too much power to run on solar power if it were a dynamically rendered data-driven website
* it would require too much energy (?)
* it would also be a security risk
* there are fewer hacking attack routes for static sites
* damage to a static site is also more easily fixed
  
<br></details>


<details>
<summary><strong>
  Dithered Images
</strong></summary><br>
  
* images take up most of the bandwidth on a site like lowtech magazine (?)
* options are eliminate images, have fewer or make them smaller
* dithering images can make them ten times less resource intensive
* dithering is considered an obsolete image compression technique (?)
* image size is determined by file format, resolution and color count
* all images on lowtech magazine are converted to black and white with four levels of gray in between, meaning 6 value levels in total (?)
* all images seem to be black and white pngs 600~650px wide that are colored by using the background-color CSS property
* the color they choose in lowtech magazine is based on their content category (?)
* they are compressed through a dithering plugin (?)
  
<br></details>


<details>
<summary><strong>
  Default Typeface / No Logo
</strong></summary><br>
  
* lowtech magazine simply doesn't use the font-family CSS attribute
* they use a typographic logo rather than font or imagery (LOW←TECH)
  
<br></details>

<details>
<summary><strong>
  No Third-Party Tracking / Advertising / Cookies
</strong></summary><br>
  
* google analytics records what happens on a website
* many companies offer similar services
* which pages are viewed / where visitors come from etc.
* 
  
<br></details>
  
  
---

```
⚠️ work in progress, still actively adding notes...
