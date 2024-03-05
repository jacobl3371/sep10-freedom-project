# Entry 4

### Context
For this unit of the Freedom Project, I had to find a software tool which I will incorporate into my Freedom Project website. Instead of continuing to learn about my chosen topic for the project which I was writing about in the first three blogs, I instead had to use that time to learn a new software tool, tinkering and looking at documentation and video tutorials to get a feel for the tool and eventually be able to solidify one to build the Freedom Project website.

### Choosing my Tool
To find the right tool, I had to consider what I wanted it to do. I needed a tool to build webpages with different icons and custom CSS which are used to illustrate the software which I am discusing in my freedom project. I want to design my website to illustrate for example, the way sites such as the Google classroom login can be accessed even through Tor browser by having the IP address which the server sees being the VPN's. The type of tool I need is further narrowed down when considering the way I aim to showcase the future inventions I am thinking about for this project. I want to integrate the software which search engines such as Startpage use on their site to have the user access a proxy within the browser by clicking a button, though my website will just have the CSS icon and is not going to lead to any proxy. I will try to make the button lead to another webpage to symbolize how the software works but this may require more extensive knowledge of Javascript so I might end up just doing a diagram with purely icons and CSS elements.

I looked at many other software tools on the list, but I couldn't figure out how to set up any of them except for TailwindCSS which I struggled with at first despite numerous attempts and video tutorials, since the npm setup didn't work for my Virtual Studio Code enabled IDE, most likely due to an error on my part which I can't figure out, and other videos only mentioned setups for completely different IDEs like React. I finally stumbled upon [this video](https://www.youtube.com/watch?v=vYowvsUiChs) which showed me how to setup a webpage with a responsive navbar using only the Tailwind CSS play CDN script in one HTML file. 

Everything else initially worked but I was unable to configure the menu to be clickable and display the hidden elements. So I instead followed [this tutorial](https://www.youtube.com/watch?v=X6CsbhSVUEc) and I was finally able to build a responsive navigation bar which collapes all of its displayed text when the screen-width is as narrow as a phone, turning into a menu which is clickable via the Javascript code, upon which it displays those collapsed elements and an 'x' icon to close out the menu. I also used [this code checker](https://zzzcode.ai/) to debug my broken code.

  - HTML:
    
![html](https://github.com/jacobl3371/sep10-freedom-project/assets/146866607/8d3bdd98-4390-42d7-b52f-54fa1b3481cd)

  - Javascript:
    
![java](https://github.com/jacobl3371/sep10-freedom-project/assets/146866607/8b116bd3-a35c-499a-965f-2f4054d7d814)

  - Webpage:
    
![preview](https://github.com/jacobl3371/sep10-freedom-project/assets/146866607/01152434-e5dc-4d42-965f-6c8d11d15fc9)

### Engineering Design Process
I paused in my engineering design process since I took the time to research and tinker with different tools until finding TailwindCSS and getting it to work. I did do some research on crypto currency since my last blog, looking into its compatability with the only OS, Tails, which works with the VPN (anonymous VPN) needed for this project. I found that more specifically than the OS, the actual stock, approved cryptocurrency application for Tails, Electrum Bitcoin, is not compatible with any crypto except Bitcoin, being named so becuase it is only a Bitcoin wallet and can not hold any other crypto currencies. I was under the false assumption until a couple months ago that I could only buy whole crypto currencies, so I had to settle for some exponentially less valuable, obscure crypto which I didn't even know wasn't compatible with any secured trustworthy wallet on the operating system that every other aspect of this project relies on. 

Coming to the conclusion that I could buy fractions of a crypto coin, I intended to buy a more trustworthy and known crypto currency like Ethereum, before I was doing some research on transferring crypto to Electrum Bitcoin and watched [this video](https://www.youtube.com/watch?v=AV_w5scAXMQ) and also [this tutorial](https://www.youtube.com/watch?v=O5EjCL56rRg) which I found later and was more in tune with my use case as it mentions maintaining anonymity through the use of Tor, aside from the two step-verification process which is unessesary and unrequired, not being shown in the first video which is a year newer. Both of these videos gave me a lot of insight on how to attain crypto currency which is usable anonymously over Tor in Tails, following a simple and quick graphical-user-interface-enabled setup which I will be going over in Blog 5.

### Skills
1. I improved my **logical reasoning** skills as though I did not know and had never used Javascript before, I was able to follow the directions and make the navigation menu work with Javascript. I also saw that the first setup did not work in making the menu clickable and interactive, and I decided to try the other video which after following its instructions, finally produced a working menu and navigation bar.
   
2. I learned to **embrace failure** and keep on trying to set up my tool even though it was very overwhelming at the start and the first tutorial which I managed to get to work didn't produce the expected outcome. I kept on trying despite failure and using what I learned to ultimately use the tool to achieve my desired outcome, getting the navigation bar to work.

[Previous](entry03.md) | [Next](entry05.md)

[Home](../README.md)
