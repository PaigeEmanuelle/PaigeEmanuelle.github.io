##Overview

Name: Paige O'Connor
Date: March 4, 2019
Project Title: HCI-TC-2
Goal: Create a website for a fake artist with Jekyll + Github Pages

##Usage

You can reach my site at https://paigeemanuelle.github.io
Navigate the site by using the menu buttons in the upper-right corner
The titles on the journal page are clickable and will lead you to posts

##Design Decisions

One deliberate design decision I made was to have the main navigation menu (in the header) be available no matter where the user is on the site, making it easy to move from page to page without clicking the back button. The name of the artist is featured prominently in the upper-left corner of the header to catch the user's attention; this is also present on every page.

The minimalistic and mysterious design of the homepage is one that I would not use for a corporate site, but I thought would be interesting and unique for an artist.

The menu buttons turn black when hovered over, creating a more responsive feel for the user.

I tried to keep the site visually consistent and appealing by limiting myself to two fonts: a more decorative one for the artist name and journal title, and a sans-serif font for the rest of the text. Similarly, I limited the text to two colors: white for the menu items, and black for everything else. I chose these because I have a fairly colorful gradient background and I didn't want the colors to become overwhelming.

I created two primary layouts
(1) "page": this is the layout I used for each page of my site (Home, About, Music, Journal). It is quite basic; it includes the main header with the artist name and menu, and creates a specific header based on the title of that given page.
(2) "post": this appears to be a commonly used layout for Jekyll, because Jekyll is good for hosting blogs. I found out how to make the post folder and layout by looking at an example (see credits below). This layout includes a special post header (which just says "Journal Entry", but could be expanded) as well as the title of that particular post (e.g. Drvengrad).

If I had more time, I would have liked to create a special album layout for the Music page of my website.

To challenge myself with CSS for this project, I did some image formatting by creating cards (I've used cards with frameworks like Bootstrap and Angular but had not made them on my own). I also challenged myself to use flexbox formatting instead of specifying pixels for sizing and spacing.


##Challenges

It took me quite a while just to download Jekyll, and to figure out how to run it locally on my computer. Despite reading about the benefits in the documentation provided, I still wasn't really sure why we were using it; I did not understand how layouts differed from templates.

I started out with a config.yml file that had many more fields than I needed or knew what they were doing. Once I got farther into the project, I did my best not to include any code until I understood it. However, sometimes not following an example exactly came back to bite me; for instance, I spent multiple hours wondering why my posts weren't showing up (despite having included markdown files in the post folder) until I realized that I hadn't used the date in the name of my post files.

Another tricky part was figuring out the hierarchy of my "layouts" and "includes", especially since I used Liquid templating. Using Liquid was really cool because it made my layouts more powerful (e.g. pulling titles from file names), but it took some thinking to determine what should be nested in what. I wasted some time trying to do this by trial and error, and then sped up the process by actually drawing out the hierarchy.

Another part that confused me was the site folder. I didn't realize that this was something that Jekyll generated, and I kept trying to put my files in there.

Finally, even though I thought I had set up Github Pages right from the beginning, I had a tough time publishing my locally-developed site with Github Pages. I thought I was pushing to the right repository from the beginning, but it turned out I was pushing to a regular directory, not the github.io one that would allow me to have a live link. Once I pushed from the master branch instead of trying to use a gh-pages branch, I was able to publish the site easily and it was simple to push new changes from Atom, where I developed my code.

I think the sink-or-swim approach to this project made it a bit frustrating (there were multiple new technologies introduced at once, online tutorials differed to a large degree), but now that I am at the end of it I feel that I have a good sense of the advantages of using layouts and of static site generation. I still don't quite understand how Ruby plays a role in this project and what the Gems are doing.

##Deficiencies

Things that I think are not great about my site / would improve:
- The layout is not completely responsive when the window is resized
- The site should have a footer with contact information, copyright
- I could not figure out how to remove the underlines from the post Links on the Journal page
- The designs of the About and Music pages could be more visually appealing
- Perhaps there should be more interactive parts besides the menu

##Further Development

After this is graded I might actually try to turn this into a portfolio website for myself. I didn't realize that Github Pages existed and that you can use it host a site for free. Jekyll seems especially good for an informational/resume site that does not involve much user interaction. I ended up looking at fairly basic examples of layouts so that I could accomplish creating one, but I would be interested to see more extensive uses of layouts.

##Credits

Where I got my images:
https://theculturetrip.com/europe/serbia/articles/the-12-most-beautiful-towns-and-villages-in-serbia/
https://barrydownepaint.com/collections/color-trends-2019/products/af-165-kona?variant=46055857031

How I learned to make cards for the album covers:
https://www.w3schools.com/css/tryit.asp?filename=trycss_ex_images_card

Helped me understand the structure of a Jekyll site and layouts:
https://github.com/victorvoid/space-jekyll-template
