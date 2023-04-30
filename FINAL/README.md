**DOCUMENTATION**

**Documentation of My Process**

1. Development of My Midterm Proposal 

Since I planned to continue with my midterm project for my final website, I began with brainstorming ideas, exploring new features that I can add to the website, and researching other similar-themed websites for inspiration such as the official Animal Crossing and Nintendo websites. During the brainstorming process, I thought about the new exciting javascript components and features I want to incorporate, such as a music player, calculator, and image galleries. Since my knowledge of javascript was very limited when I was working on my midterm project, I felt like I didn’t have many options to play with. I now feel pretty confident with my HTML/CSS skills and believe that I have a solid understanding of basic javascript, I definitely want to explore and add more javascript features to my final website. I jotted down my abstract ideas and most importantly, I played Animal Crossing which highly helped me to think about the new content I could put on the website. I recently bought an extension pack of Animal Crossing, Animal Crossing Happy Home Paradise, which focuses on building dream vacation homes for various villagers while working at the company “Happy Home.” I definitely wanted to develop a new page dedicated to this content. 

2. Developing Sketches and Wireframes 

When I had a list of potential ideas and layouts, I started to make low-fidelity sketches and wireframes. Since I tend to focus better when I sketch with a pen on paper, I started sketching wireframes very roughly just to have a clearer understanding of my ideas and the potential layout of the website. I then started to build low-fidelity wireframes using Figma, building the overall structure and layout of the new features and pages. While I was developing wireframes, I came up with a new idea for the Happy Home page. I decided to make the page an informational page about what a “Happy Home” is, its interior design team, its values, and built vacation homes by Happy Home. I developed a low-fidelity wireframe for this page as well. 

3. Building Skeletons 

After creating low-fidelity sketches and wireframes, I started building skeletons and frameworks. I focused on creating the structure and layout using HTML and Javascript. 

4. Developing & Incorporating Bootstraps 

Once I had a basic framework in place, I started adding and developing more functionality using Javascript and Bootstrap. Since I was not that familiar with Bootstrap, I spent a whole day browsing through different Bootstrap features and components. I incorporated several Bootstrap components into the website, such as the carousel gallery, cards, and pop-up modals. I was truly surprised by how easy and convenient Bootstrap is. When I was learning Bootstrap during class, I felt a bit lost since it is my first time using Bootstrap, but once I got used to it, I found it to be a very powerful and flexible tool which made it easy for me to create complex features. When I was developing the Turnip Calculator, I relied on my class notes which helped me understand the logistics much better. I also implemented and modified the tab gallery feature on W3 Schools to make the page more interactive instead of just scrolling through one single image. 

5. Finding the Right Color Schemes & CSS

After building the framework, I began to apply CSS to add design and modify the default Bootstrap CSS. Since I want my website to be pastel-themed, I used Coolors, which is a color scheme generator, to get inspiration for the right color scheme. I screenshotted every color scheme that I liked and saved them on Figma so that I can easily use the spoiler to get the HEX code of each color. For the Happy Home pages, I wanted it to be tropical-themed as it focuses on building vacation homes on a tropical island, I created a mood board to get a better understanding of the style and the color scheme that I am aiming for. I also used many online tools such as Coolor and Adobe Color to experiment with different combinations and generate tropical color palettes. After finding the right color schemes, I started to apply them to the website using CSS.

6. Making It Responsive & Media Query

Once I completed building the website, I began to focus on making it responsive using media queries. Since everything was built on a desktop-sized screen, I had to adjust a lot of elements based on the size of the mobile screen, such as the font size, line height, box size, image size, etc. 

7. Consistency 

After completing the website’s development, I focused on achieving consistency throughout the website. I made sure to use the same fonts, colors, and styling throughout the website. I used a consistent color palette and typography, and I made sure that every header had the same margins and paddings. I also made sure the layout and design of each page followed a consistent structure, and that the cards, boxes, and images are spaced out evenly.


**Explanation of Interesting Source Codes**

1. Music Player

Firstly, I want to talk about my music player source code. I learned the .play() and .pause() methods through W3 Schools and Youtube tutorials. It was very interesting as I was surprised by how straightforward it was to make a music player. When I had very limited knowledge about creating music players, I believed that it would be very complex and I would have to manipulate different functions. However, it was a very straightforward process as I just had to get two different icons, the play button, and the pause button, and use Javascript to manipulate the audio element and the icons. It was truly fascinating how a few lines of code can create a functional music player. I used conditional statements, if, and else to manipulate the audio file and switch the icons. If the audio is paused, the play() method is called on the audio element to start playing, and the icon changes from the play button to a pause button, indicating that the audio is currently playing. If else, when the audio is not paused (currently playing), the pause() method is called and the audio will stop playing, and the icon changes from the pause button to the playing button. This code creates a simple button that allows users to control the audio. 

 ```
  icon.onclick = function(){ 
    if(song.paused) {
      song.play();
      icon.src = "song/pause.png"
    } else {
      song.pause();
      icon.src = "song/play.png"

  }
  ```

2. Bootstrap Cards vs Manual Cards

I wanted to point out the difference between Bootstrap cards and manual cards. Using Bootstrap cards was very convenient and easy to use as I simply had to use the pre-built HTML and CSS to create responsive cards. It is very flexible and it includes a lot of options for headers and footers and a wide variety of content. I was also able to simply replace the default thumbnail image by plugging in my images to the default src. Using this saved a lot of time and effort as I did not have to design and style the cards from scratch. The only thing I had to do is modifying the default CSS, remove the border, and change the content, font styles, and sizes. In contrast, creating manual cards required a lot of time and effort as I had to build them from scratch. While this gives greater control over the appearance and functionality of cards, it can be highly time-consuming. I used Flexbox to make the cards beside each other and had to manually create the box width and height to contain its content. I also customized every aspect of the card, including its image size, box size, header, and paragraph styles. While Bootstrap cards can save a lot of time and provide a solid foundation, manual cards offer greater control and flexibility for more unique designs.  

Bootstrap Cards - Built-in HTML

  ```
  	<div class="card-container">
	<div class="card-deck">
  <div class="card">
    <img class="card-img-top" src="images/book.jpg" alt="Card image cap">
    <div class="card-body">
      <h5 class="card-title">Hayo's Relaxing Reading House</h5>
      <p class="card-text">Hayo's Relaxing Reading House boasts a warm and inviting interior design, featuring comfortable seating, soft lighting, and natural wood accents that create a cozy atmosphere perfect for unwinding with a good book.</p>

    </div>
  </div>
  </div>
  </div>
  
  ```
  
 Manual Cards 
  ```
 		<div class="articles">
			<img src="news/fishing.png" alt="fishing photo">
			<h4>Fishing Contest</h4> 
			<p>April 22, 2023</p>
			<div class="text">
				<p>Get ready to cast your lines! A fishing contest is set to take place this weekend, offering participants the chance to win exciting prizes and rare items. Don't miss out on the fun and show off your angling skills to take home the grand prize.</p>
			</div>
		</div>
  ```


3. Popup Modal 

Another very interesting part of my source code is the popup modal component. I used the Bootstrap’s modal plugin to create a pop-up contact page. Since Bootstrap only offers the pre-built modal box, I manually added a function alert() to the submit button, displaying an alert box that says “you have successfully submitted your request” to the users when they submit their information. I also modified the default CSS by changing the background color of the box and the font styles of headers and paragraphs, and the design of the inputs and buttons. 
  ```
 <div id="myModal" class="modal fade" role="dialog">
  <div class="modal-dialog">

    <!-- Modal content-->
    <div class="modal-content">
      <div class="modal-header">
        <h4 class="modal-title">Contact Us</h4>
      </div>
      <div class="modal-body">
      	<label for="fname">Full Name</label><br>
  			<input type="text" id="fname" name="fname"><br><br>
  			<label for="lname">Email</label><br>
  			<input type="text" id="email" name="email"><br><br>
  			<label for="lname">Nook Phone Number</label><br>
  			<input type="text" id="phone" name="phone"><br><br>
  			<label for="lname">Details</label><br>
  			<input type="text" id="details" name="details"><br><br>
  			<div class="submit"><input type="submit" value="Submit" id="submit" onclick="myFunction2()"></div>
      </div>
      <div class="modal-footer">
        <button type="button" class="btn btn-default" data-dismiss="modal" id="close">Close</button>
      </div>
    </div>

  </div>
</div>

function myFunction2 () {
	alert("You have successfully submitted your request");
}

  
  ```
  
**Issues and Challenges I Encountered**


1. Design & Color Schemes

The first challenge that I encountered while developing the website was choosing the right color scheme. Although I used several online tools to help me pick different color schemes, I had to change the color scheme numerous times until I found the right one that fit the website’s theme and mood. I kept experimenting with different color combinations until I found the right one that looked engaging and visually appealing. It was definitely a trial-and-error process. 

2. Consistency 

One of the significant issues that I encountered was achieving consistency throughout the website. When I was developing the pages, I didn’t focus a lot on the consistency of the design and layout. After completing the development of the website, it looked chaotic as all elements looked inconsistent and every page lacked a clear visual hierarchy. Every header and photo had different font sizes, paddings, and margins, which disrupted the look of the website. To solve this issue, I created a style guide in my notebook and wrote down all the design elements and attributes that needed to be consistent throughout the website such as font sizes, colors, margins, paddings, and line heights. For example, all h3 must be 38px and the font family should be Fink Heavy. All subheaders should be 20px and explanation paragraphs should be 16px. Following the style guide, I went back to each page and carefully examined and adjusted every element to ensure that they were consistent. I also checked the margins and paddings of all elements to make sure that they were consistent throughout the website. I repeated this process for the mobile screen using media query.


3. Bootstrap CSS

Another issue that I encountered was modifying the default Bootstrap CSS. When I first incorporated Bootstrap components, I realized that the default Bootstrap CSS was messing up a lot of my design elements. For example, its default navbar, paragraph, footer elements’ margins, and padding settings were causing many layout and design issues. The hardest challenge was that the default Bootstrap CSS had the same navbar class name as my CSS, .navbar, and it had its navbar class set under flex-wrap. It was overriding my CSS as I applied CSS through my header and nav ul, not to the navbar class. Therefore, it completely changed the look of my navbar and I was highly struggling to resolve the issue. I spent a vast amount of time reading through the Bootstrap documentation to understand its default design settings and how my CSS can override the default CSS. I also used Chrome DevTools to inspect the issues. I solved the navigation problem by setting the navbar class flex-wrap to unset which removed the default flex-wrap. I learned that specificity in CSS is highly important to ensure that my CSS would take precedence over the default Bootstrap CSS. 


4. Media Query

The hardest challenge while working on the project was making the website responsive and working with media queries. It was highly overwhelming as I had to fix and adjust almost every element of the website to make it compatible with the mobile screen size. I had to redo the layout, font sizes, margins, and paddings for almost every element. When I started to work on mobile size, I realized that everything looked cramped and cluttered. Everything was out of place. I continuously had to fix, adjust, and test how it looked on the mobile screen.


**What I Learned to Accomplish the Project**

1. More Bootstrap Components

To accomplish the project, I spent a lot of time exploring the different Bootstrap components that I could incorporate into my website. I found that Bootstrap had numerous components and features that could help me create a more professional-looking website without having to start from scratch. It helped me to create complex features very easily such as the carousel image gallery, image cards, and pop-up modals. Learning more about Bootstrap components and features made the website development process much easier and more efficient as they are responsive as well. 

2. More Javascript Components

Besides revisiting my class notes, I also spent a lot of time exploring and learning new javascript components and functions to add to my website. I watched many youtube videos and read about Javascript How To on W3 Schools. I learned how to make a tab image gallery where you tap through different image thumbnails and the website displays the expanded image. Watching a youtube video about creating a music website also taught me how to create a basic audio player with basic controls and how to manipulate the audio and icons using Javascript. Learning new Javascript features was really mind-blowing and implementing new Javascript features and functions helped me to add more interactivity and functionality to my website. 

3. Input and Forms 

When I was working on the midterm project, I had a very limited understanding of input and forms. I revisited class notes and read much documentation on HTML form and input attributes on w3schools. I learned about many more form elements and input types which helped me to create the subscribe section and contact page. 


**Next Steps**

1. More Pages 

If I had more time and tools, I definitely want to continue expanding the website by developing more engaging yet interactive pages. I want to develop another page that describes the overall process of building vacation homes at Happy Home. I also want to create individual pages dedicated to villagers’ homes, showing more details about the house. 

2. Turning Into an Online Shop

I also want to expand the website by turning it into an actual online shop where customers can browse through different items at the Nook Shop, add items to their cart, and check them out through the website. I want to rebuild the website and make it into an e-commerce website. 


3. Animation Using Greensock

Learning about Greensock animation in class was very cool and I definitely want to implement some Greensock Web Animation into my website, animating various HTML and CSS elements and properties to make my website more interactive and engaging. 




