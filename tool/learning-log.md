# Tool Learning Log

3/4/24

* Used TailwindCSS to create a responsive navbar webpage
    * Collapses the displayed links on the navbar
        * Affected when the screen size is less than or equal to medium
        * Those links are hidden within the toggleable menu icon
        * When the menu icon is toggled the collapsed elements appear
        * The icon also turns into a close button
            * This requires some javascript
            * I used [this video](https://www.youtube.com/watch?v=X6CsbhSVUEc) for the setup
            * The Javascript which was provided did not work
            * The menu icon wasn't even toggleable
            * Since I couldn't find any documentation I had to use a code debugger similar to Replit
                * This did help me understand somewhat better how the tool works, aswell as how to incorporate it into   HTML, CSS and Javascript
            * In the future though, I must utilize the Slack channel for TailwindCSS
            * I will use it to ask any questions and debug my code
            * Which will help me understand it a lot better than an automated debugger
        * Available at: https://jacobl3371.github.io/tool/
        * Next Steps:
            * Try to setup a webpage/website components using TailwindCSS
            * Doing this by *only* watching or reading documentation
            *  If I really can't figure it out, I will **ask the slack channel**


3/11/24

* I learned on my own how to create a carousel in TailwindCSS
* Following [this tutorial](https://www.youtube.com/watch?v=QXUM_AycJEc)
* At [this point](https://youtu.be/QXUM_AycJEc?si=eUoUFKJAeCWoR2an&t=408) in the video I changed the img class
    * I only set the class to cover instead of h-full and w-full as well
    * The cover option worked better for my image
    * I couldn't get the image used in the video since it is not a link
    * The image was n the form of a file which existed locally
* Either in their account-based IDE or on their hard drive (VS code desktop)* When adding the other two images for the carousel I had to add back the w-full and h-full classes
* But I had to remove the object-cover class to keep the images from overlapping
* This also made each image take up a proportionate height and width
    * At this point my h2 elements were all overlapping since they were in the center of the page
* I ultimately got rid of the headings
* The video explained everything else except for how to add the headings properly
    * [Result](carousel.html)


3/16/24

* Used Tailwind and Javascript to create a multi-card slideshow carousel
    * Followed [this code](https://github.com/JAFSCodeSchool/multi-card-carousel-using-tailwind-and-javascript/tree/master)
        * I replaced all of the instances of image 1, 2, and 3 in the html with the links to the raw github image files
        * Swapped the words: next and prev in JS button functions
        * This makes the left and right buttons scroll in their specified direction
        * I noticed that as soon as you click to scro2F146866607ll, it brings you back. So you have to click twice just to even scroll once
        * Let alone the fact that there is a few second timeout in which the slide goes back to the previous one after clicking
        * The user can click very fast to get from Heading 1 to Heading 8
            * It is really annoying if they are clicking at a *constant* not-fast-enough-speed
                * Especially after heading 4
                * If the user doesn't click fast enough they will be sent to the previous slide in an instant
                    * At least if they click very fast they don't get interrupted and pushed back mid-scroll
            * I was tinkering around with the code
            * The first line of Javascript

    ```
    let sliderContainer = document.getElementById('sliderContainer');
    ```

* Can have the code within the parenthesis changed to only slider to reference only the ul element the elements forming the cards are inside and not the overlaying div
            * Making no difference in the output


3/24/2024
* Combining my carousel and navbar
    * Tinkering with freedom project webpage layout/wireframe
    * I was examining the Javascript for the carousel and found that by removing this entire function:

    ```
    function autoPlay(){     prev()      if (+slider.style.marginLeft.slice(0, -2) === -cardWidth * (cards.length - elementsToShow)){         slider.style.marginLeft = "0px";     }      setTimeout(() => {         autoPlay();     }, 3000); }
    ```

* The carousel no longer autoplays and stays permanently fixed on the slide the user had clicked on
    * The slide only changes when the user clicks on the left or right arrow
  * (*More than enough time to take a screenshot of a far-right slide since no faulty javascript function brings the user back to the first one automatically)
![carousel](https://github.com/jacobl3371/sep10-freedom-project/assets/146866607/d93cb809-216d-414a-82f9-3b85a2e5537d)

   * Surpisingly enough, I expected that by changing the the function prev to next in the above code snippet,

    ```
    function autoPlay(){     prev()      if (+slider.style.marginLeft.slice(0, -2) === -cardWidth * (cards.length - elementsToShow)){         slider.style.marginLeft = "0px";     }      setTimeout(() => {         autoPlay();     }, 3000); }
    ```

   * The carousel would function the exact same way but at least autoplay in the right direction
    * This made the entire carousel be displayed wrong and not scroll at all, contradicting the rest of the code.
* I do intend to add some sort of function similar to this autoplay function, one that allows the user to scroll infinitely
    * Not having to go back if they reach the very right-most slide or are even at the starting slide
* [Combing responsive navbar with toglleable menu icon and carousel](fp-temp.html)


3/25/2024
* Fixing fp-temp.html
    * Right now, my freedom project website template is not at the minimum viable product stage
        * The menu is not outputted properly and flows over the content like the carousel
        * I tried to add a section to make space between the dropdown menu panel and the content
            * This didn't stop the menu from overlapping over *all* of the content including the carousel

             ![fptemp](https://github.com/jacobl3371/sep10-freedom-project/assets/146866607/0ccc0b19-62a2-499d-8c6d-372c4097e6a7)

            * This overlapping also made it so that the text can not be highlighted when hovered over
                * This function works when the navbar is expanded and none of the content overlaps each other
        * I also saw that you could scroll infinitely in borth directions
        * There would be no slides, just blank space
            * And since you could scroll infinitely, you had to scroll infinitely to get back to the slides!
        * Wrapping the entire navbar in a div and adding the css:

        ```
        div {
        margin: 10px;
        padding-top: 10px;
        padding-bottom: 10px;
        }
        ```

        * Makes it so that the user can't scroll past the 8th slide or before the 1st
            * But the carousel is not fully responsive yet and the user can't scroll to the 8th slide on the smallest screen size.

4/3/2024
* Making a responsive grid using tailwindcss
* [grid](tailwind-grid.html)
    * Tailwind uses a CSS grid similar to bootstrap but only utilizes vanilla CSS
        * sm, md, lg, xl, 2xl followed by a colon and either row for vertical and col for horizontal and then span (to span accross the display) and the number of horizontal or vertical columns that div elements should occupy
        * I added the classes

        ```
        lg:col-span-3
        md:col-span-3
        ```

        * Which made the item which only took up one box take up all three available, leaving no empty space and being fully responsive to look good when the actual content is added.
        * At one point item 6 and 7 did not span as far down vertically as item 8, so I changed the grid number from xl:row-span-6 to xl:row-span-7
        * This cuased those items to take more vertical rows on the 2xl display as well, and adding row classes for the 2xl display for items 1 and 5 which were too short didn't work
        * I had to declare the number of rows that item 8 occupies on an xl display

        ```
        xl:row-span-1
        ```

        * Which made all of the items aligned on all of the displays
        * I couldn't figure out how to add space between the horizontally stacked items on the small display without it causing the first item to take up more rows than the other items

        ```
        screen-y-1
        ```

        * worked in creating the desired spacing on the smallest display but made the first item misaligned on all other displays
        * So I set the class for the overlaying div containing all of the items in the grid to

        ```
         flex justify-center
        ```

        * Which made all of the items aligned horizontally and centered on the smallest display, and the very leats aligned and centered on all displays.
        * [Original code](https://github.com/Crackiii/custom-tags-input/blob/master/responsive-grid/grid.html) for comparison

