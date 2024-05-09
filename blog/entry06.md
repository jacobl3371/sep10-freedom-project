Entry 6
##### X/X/XX

### Crafting my website MVP

<ins>Style:</ins>

For my entire Freedom Project website, I am using the CSS framework Tailwind along with basic HTML and CSS to make my website populated with responsive components and be responsive as a whole using the Tailwind CSS responsive grid system, which is much easier to undertsand and implement than Bootstrap's grid system, as Tailwind only uses vanilla CSS. As a whole, I found using Tailwind to be a lot easier than bootstrap when building components and making responsive gid systems to make the content be displayed *exactly* how you want it to be, while it is very hard to achieve these specific layouts with Bootstrap.

For example, you can use specific, breakpoint-specified classes, to control how many rows and cols an item spans as well as which row and which col that element starts spanning from, which greatly affect how elements are responsively displayed corresponding to the width of the screen which they are being displayed on.

```
<div class="sm:grid grid-cols-2 grid-rows-2 p-8">
    <div class="sm:col-span-2 sm:row-span-1 md:col-span-1 md:row-span-1 md:col-start-1 md:row-start-1 space">
         <p>An innovation for the future of accessing services which block Tor would be any easy to use, in-browser accessible free VPN or proxy network that could be used in Tor Browser to effectively hide from the website that the user is actually accessing the website from the overlaying Tor network.</p>
    </div>
    <div class="sm:col-span-2 sm:row-span-1 md:col-span-1 md:row-span-1 md:col-start-2 md:row-start-1 space">
        <p>An innovation for the future of accessing services which block Tor would be any easy to use, in-browser accessible free VPN or proxy network that could be used in Tor Browser to effectively hide from the website that the user is actually accessing the website from the overlaying Tor network.</p>
    </div>
    <div class="sm:col-span-2 sm:row-span-1 md:col-span-1 md:row-span-1 md:col-start-1 md:row-start-2 space">
        <p>An innovation for the future of accessing services which block Tor would be any easy to use, in-browser accessible free VPN or proxy network that could be used in Tor Browser to effectively hide from the website that the user is actually accessing the website from the overlaying Tor network.</p>
    </div>
    <div class="sm:col-span-2 sm:row-span-1 md:col-span-1 md:row-span-1 md:col-start-2 md:row-start-2 space">
        <p>An innovation for the future of accessing services which block Tor would be any easy to use, in-browser accessible free VPN or proxy network that could be used in Tor Browser to effectively hide from the website that the user is actually accessing the website from the overlaying Tor network.</p>
    </div>
</div>
```
The "grid" utility class declares a grid which will be composed of elements nested within the parent element with the grid class. The "sm:grid" class makes it so that the elements of the grid stack on top of each other, conforming to the smallest default sm-display. The "grid-cols-2" and "grid-rows-2" declare the number of rows and columns composing the grid. This way I was able to make a completely responsive, and custom tailored website, using the Tailwind CSS grid to have my content be displayed exactly how I want it to, using a far more straight forward grid system than Bootstrap which actually allows me to configure extremely specific layouts that are inarguably much easier to achieve using Tailwind than by using Bootstrap, the latter requiring much more extensive knowledge of Bootstrap and CSS in general than it takes to learn how to code the exact same responsive layout in Tailwind CSS. At first, I was going to use Bootstrap along with Tailwind, as I had a broken navbar made with Tailwind CSS which I wanted to replace with a perfectly functioning Bootstrap navbar that I had already built, but combining the elements and their corresponsing CDN links was ineffective in making the Bootstrap navbar which I had added to my Tailwind CSS webpage be displayed, and only caused obstruction to the other elements. So I instead decided to stick with Tailwind as the responsive CSS framework for my entire Freedom Project website.

<ins>Content:</ins>

I organized my Freedom Project website into four different html files. One being the overlaying Freedom Project index.html file which the user is brought to when they open up the preview of my Freedom Project (jacobl3371.github.io/sep10-freedom-project), and three seprate files for the actual content of my Freedom Project, the overview, currently existing innovations in my topic, and the future inventions I have come up with for my topic.

My overview provides the context for the topic of my Freedom Project, which is that many services educational web applications which students must use every day, block the heart of anonymity on the internet, Tor, and make it so that nobody can access these services without having all of their data mined and collected. My obverview addresses the issue and states my goal. The currently existing inventions section discusses what services (sofware) are used to facilitate education online and that block privacy softwares from entering the site, as well as possible alternatives to proprietary learning services which I have researched applying a FOSS standard, some of these alternatives being services which educators could look into. In my future innovations file I discuss the future of in-browser VPNs and in-browser virtual machines that would be built and configured for Tor Browser to effectively hide from a website which blocks Tor, the fact that you are entering from an IP Address which originates from the Tor network, and the web app mimics the behaviour of a browser liek Firefox, so website servers do not think anything of it. An in-browser virtual machine would allow students to use services like Edpuzzle which only work on the third-party cookie facilitating browser, chrome, and by loading an entire other operating system within a virtual machine built to work with Tor browser, the user could access these services like edpuzzle anonymously over Tor, in the amnesic Tor browser, as Edpuzzle only sees the chrome browser which you are accessing their site from, and not the non-third-party-cookie-supporting firefox-based Tor browser.

### Engineering Design Process


### Skills

[Previous](entry05.md) | [Next](entry07.md)

[Home](../README.md)
