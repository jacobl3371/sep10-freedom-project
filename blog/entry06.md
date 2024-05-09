1# Entry 6
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
The "grid" utility class declares a grid which will be composed of elements nested within the parent element with the grid class. The "sm:grid" class makes it so that the elements of the grid stack on top of each other, conforming to the smallest default sm-display. The "grid-cols-2" and "grid-rows-2" declare the number of rows and columns composing the grid. This way I was able to make a completely responsive, and custom tailored website, using the Tailwind CSS grid to have my content be displayed exactly how I want it to, using a far more straight forward grid system than Bootstrap which actually allows me to configure extremely specific layouts that are inarguably much easier to achieve using Tailwind than by using Bootstrap, the latter requiring much more extensive knowledge of Bootstrap and CSS in general than it takes to learn how to code the exact same responsive layout in Tailwind CSS. At first, I was going to use Bootstrap along with Tailwind, as I had a broken navbar made with Tailwind CSS which I wanted to replace with a perfectly functioning Bootstrap navbar that I had already built, but combining the elements and their corresponsing CDN links was ineffective in making the Bootstrap navbar which I had added to my Tailwind CSS webpage be displayed, and only caused obstruction to the other elements. So I instead decided to stick with Tailwind as the responsive CSS framework for my entire freedom project website.



### Engineering Design Process


### Skills

[Previous](entry05.md) | [Next](entry07.md)

[Home](../README.md)
