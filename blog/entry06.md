# Entry 6
##### X/X/XX

### Attaining compartmentalized, pseudonomymous access to your education in a digital online era; crafting my website MVP
For my entire Freedom Project website, I am using the CSS framework Tailwind along with basic HTML and CSS to make my website populated with responsive components and be responsive as a whole using the Tailwind CSS responsive grid system, which is much easier to undertsand and implement than Bootstrap's grid system, as Tailwind only uses vanilla CSS. As a whole, I found using Tailwind to be a lot easier than bootstrap when building components and making responsive gid systems to make the content be displayed *exactly* how you want it to be, while it is very hard to achieve these specific layouts with Bootstrap.

For example, you can use specific, breakpoint-specified classes, to control how many rows and cols an item spans as well as which row and which col that element starts spanning from, which greatly affect how elements are responsively displayed corresponding to the width of the screen which they are being displayed on.

```
<div class="sm:grid grid-cols-2 grid-rows-2 p-8">
            <div class="sm:col-span-2 sm:row-span-1 md:col-span-1 md:row-span-1 md:col-start-1 md:row-start-1 space">
                <img src="" class="text-center" alt="img">
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

### Engineering Design Process

### Skills

[Previous](entry05.md) | [Next](entry07.md)

[Home](../README.md)
