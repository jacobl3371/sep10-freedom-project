# Entry 5
##### X/X/XX

### Finishing learning my tool
In the time given for the Freedom Project, I had to continue learning the tool I chose, which in my case was the CSS framework Tailwind, documenting it in a seperate learning-log in the tool folder. I had already built a responsive navbar and added a carousel following [this code](https://github.com/JAFSCodeSchool/multi-card-carousel-using-tailwind-and-javascript/tree/master) on Github, which I had to make some minor adjustments to in order to make it function properly, like getting rid of the autoplay feature:

    ```
    function autoPlay(){     prev()      if (+slider.style.marginLeft.slice(0, -2) === -cardWidth * (cards.length - elementsToShow)){         slider.style.marginLeft = "0px";     }      setTimeout(() => {         autoPlay();     }, 3000); }
    ```

but this was just Javascript and not Tailwind CSS code. The carousel is ultimately not responsive and the navbar-menu, when the elements are collapsed on a small display, overlaps the other content and looks like this:

![fp-temp](https://github.com/jacobl3371/sep10-freedom-project/assets/146866607/01bb43d5-1337-4c5a-8c71-875c4b2dd67b)

I am definitely going to have to rebuild atleast the navbar if not the carousel as well.

What I did have a lot of success in learning and felt was a lot easier than Bootstrap was Tailwind's responsive grid system. I copy and pasted the code from [this link](https://github.com/Crackiii/custom-tags-input/blob/master/responsive-grid/grid.html) and tinkered with the code changing the display which is in the format screen-size:row/col-span-number, where the row/col value indicates wheter to occupy space along the horizontal x-axis (col) or vertical y-axis(row), the span value makes that objedt span accross teh entire specified display, and the nuber after that dictates how many columns or rows that object takes up.

example:

    ```
    lg:col-span-3
    ```
In order to learn my tool I usually watched video documentation and copy and pasted code, which was usually linked within those same videos, for specific components that I wanted to include in my webpage and eventually my Freedom Project. I examined and tinkered with the code and looked in the comment section for any suggestions to improve the code such as swapping the incorrectly placed 'next' and 'prev' values of a carousel to make the right arrow go right and left arrow go left.

There is not much you can accomplish in learning specific Tailwind code, you can only really get a feel for it like any other CSS-based framework or coding language. To understand Tailwind CSS fully, you need to learn CSS in general, and with Tailwind's responsive grid system which only utilizes vanilla CSS while using Bootstrap's familiar format, Tailwind is a lot easier to understand and use than Bootstrap.

            Original code for Tailwind grid:                        What I changed:

                

### Freedom Project MVP

### Skills

[Previous](entry04.md) | [Next](entry06.md)

[Home](../README.md)
