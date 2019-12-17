# Unit One - Quantitative

![](https://github.com/mi-desai/Major-Studio-1/blob/master/final-documentation/quantitative.png)

![](https://github.com/mi-desai/Major-Studio-1/blob/master/final-documentation/MS1%20Quantitative%20Visualization.jpg)

![](https://github.com/mi-desai/Major-Studio-1/blob/master/final-documentation/quant-excel.png)


The project here was designed to estimate the spending by department on acquired artwork in a given year by the Metropolitan Museum of Art. 

Using the CSV, I narrowed everything down to "Credit Line" which included a property showing if the artwork was acquired or donated, and then assigned them to the appropriate department, all using Excel. Then I took the Met spending levels and divided them by objects acquired in that particular year. 

As this was my first-ever data visualization assignment, I used a tool I was familiar with at the time (Excel) to create a TreeMap. 


# Unit Two - Qualitative

Listening to the Met describe their tagging system is what made me choose this project. I wanted a visualization that would allow for an elegant design for comparing and ranking categories, which is why I settled on a bump chart made in D3. 

![](https://github.com/mi-desai/Major-Studio-1/blob/master/final-documentation/qualitative.PNG)

Once again, I used the CSV to narrow the data down to paintings and then took stock of all their tags and arranged them in a matrix where they could be counted. I used this matrix to create a json that I loaded into the qualitative project and used one of Mike Bostock's bl.ocks as inspiration for the chart, which I was able to reuse and assign some unique color patterns to in order to complete the project.The visualization is not interactive. 

# Unit Three - Interactive

<b>Repository</b>: https://github.com/mi-desai/met-in-the-money <br>
<b>Site</b>: https://mi-desai.github.io/met-in-the-money/ <br>

## Stage One - Searching for Subject Matter

I've wanted to engage data visualization on subjects that I know a little bit about - so after doing a fair amount of research and seeing that the Met had gone through a restructuring of its finances and undergone a leadership change in 2016. Given my focus in my professional career, I decided this would be a perfect subject to explore through design and visualization. 

## Stage Two - Designing and Re-Designing

I really struggled to come up with a design for this project that would tell the entire story of the restructuring. Originally I wanted to do one SVG-based visualization  in D3, but I couldn't think of a way to explore the Met's finances in a single SVG that would have worked for every topic I wanted to cover. 

I worked on three design 'themes' that I think are necessary for financial data: 

<ul>
  <li>Parts of a Whole</li>
  <li>Trend over Time</li>
  <li>Modularity - elements in isolation vs. integrated together</li>
  <li>Absolute vs relativze sizes and changes</li>
  <li>Context & Comparability</li>
  <li>Narrative/So What?</li>
</ul>

I decided to keep it simple and divide everything I wanted/could discuss into separate slides to achieve modularity, and for the graphs to make sure I was expressing parts of a whole.

![](https://github.com/mi-desai/Major-Studio-1/blob/master/final-documentation/slide-example.PNG)

## Using TUI.Charts to Overcome a Hurdle

I used a library called tui-charts to overcome the hurdle of having to make multiple, stateful D3 graphs with limited experience in the library. 

https://github.com/nhn/tui.chart

Because my design focus kept changing over what I wanted to do with the Met financial data, I used this chart to take a "shortcut" over this technical part of the process to create "Met in the Money."

Please see either the live website above, or look at the video (met-in-the-money.mp4) to get an idea of the full functionality of this project.

# Unit Four - Mobile

<b>Repository</b>: https://github.com/mi-desai/met-mobile <br>
<b>Site</b>: https://mi-desai.github.io/met-mobile/ <br>

I wanted to continue my work that I had started on the subject matter and presentation method in my Interactive Project and wanted to incorporate the design feedback I received at the end of the interactive project. There were two stages to this project. Stage 1 was incorporation of feedback. Stage 2 was optimizing the website for mobile. 

## Stage One: Incorporating Feedback

The main elements of the feedback for the last project were: 
<ul>
<li>Bring the color scheme and font in the graphs in line with the rest of the website</li>
<li>Change the title from 2016-Present to reflect its limited time-period, likelihood of getting out of date</li>
<li>Remove work-in-progress sections</li>
<li>Bold white type on a black background - change it up or bring it in line with an overall color aesthetic</li>
<li>Grey title above the black text boxes is a jarring change</li>
<li>Incorporate a visual hierarchy</li>
<li>Incorporate a next button or a scroll functionality, not a drop-down</li><br>

I addressed each element here by matching up the typography on each "slide" in the desktop version and getting a unified color palette going, which can be seen below. Where other colors were required, I used complementary colors with a softened hue or slightly darker versions of the same colors. I wanted to make sure the color palette was somewhat in line with the appearence of the Met website which has a grey/red color scheme. 

Color palette (From Coolors.co): 

![](https://github.com/mi-desai/Major-Studio-1/blob/master/final-documentation/mobileC.png)

By increasing the size of the typography of each of the graph titles, the viewer knows exactly where to look first, creating a visual hierarchy.

Instead of having multiple text boxes, I incorporated a card flip in CSS to show more text in a reduced space. 

Additionally, I rewrote most of my jQuery to get the site working with 'next' and 'previous' buttons instead of a drop-down.

## Stage Two: Optimization for Mobile

I used Bootstrap.js to reconstruct the "Met in the Money" website from the ground-up for mobile. I decided to approach it that way since my styles and html for the desktop website was already extremely complicated and many of its rules re: styling would have overlapped or conflicted with Bootstrap. Additionally, there was no need for much of the functionality I created in Jquery for the drop-down, or next buttons on mobile, since SCROLLING is the best way to progress through a long article-like piece like this one. Primarily, it would have conflicted with the numerous CSS Flex Containers I had set up in the desktop version.

![](https://github.com/mi-desai/Major-Studio-1/blob/master/final-documentation/mobileA.png)

In fact, using Bootstrap for a scrolling-only experience simplified the website significantly. I decided against many columns since width was limited, and the only flaws appear in the SVG charts, whose legend appears to edge over the right margin, which I tried to correct but couldn't. Still, the scrolling experience may in fact be a better way to proceed through a project like this.

In the future, I plan on utilizing Bootstrap to construct any websites I build because of its mobile support. When I asked family to test out to see if they could view my project, they all tried to look at the desktop version on their phone and complained that everything appeared to be a mess. It may make sense, therefore, to design any information-intensive apps or articles like "Met in the Money" for mobile first and for the desktop as a secondary concern.

![](https://github.com/mi-desai/Major-Studio-1/blob/master/final-documentation/mobileB.png)

WHEN VIEWING THIS PROJECT, PLEASE USE A MOBILE VIEW ON INSPECTOR.
