---
layout: post
title: Rodolfo's Book Box
description: A hyper personal design.
img: /img/bb1.jpg
---
<img class="center" src="{{ site.baseurl }}/img/bb1.jpg" alt=""/>
# Background
I worked on this box for a project in Critical Practices, a graduate level design course offered through the Berkeley Center for New Media. We were asked to create a hyper personal product - a product that is designed with the needs of a single user in mind.

Our first step was finding our user. 

We brainstormed potential people in our community outside of our immediate social circles and came up with a list that included UC Berkeley professors, staff at places we volunteered, and local artists. During this search we met Rodolfo Córdova, a musician and student instructor. We were inspired by his dedication to his craft and decided to create something for him for this project.

**But first, who is Rodolfo?**

Rodolfo is a graduate student in composition at Mills College. He was trained at a music conservatory in Puerto Rico and draws inspiration for his compositions from the literature and soundscapes of his homeland. He prefers to work away from digital distractions, but finds this difficult at times. Time management is important to him, and he frequently tries different methods to maximize his time and focus. 

We ended up building him a **book shaped lock box with a timer feature** that plays Puerto Rican bird sounds when the timer goes off. He can specify the amount of time he wants to work using the touch sensor "bookmark" and then store his phone in the box as he focuses on composing. 

The book shape of the box relates to his love of literature and contrasts with the digital distraction of the phone within. The bird sounds of the timer are some of the sounds from nature that inspire him and spur on his creative process.

My role in this project was working on the box design in Adobe Illustrator, laser cutting the box prototypes, and helping test the code for the light display. I also contributed to the final product assembly and process documentation. 

<img class="center" src="{{ site.baseurl }}/img/bb2.jpg" alt=""/>

# Concept
This book shaped lock box can hold Rodolfo's phone for a specified amount of time as he works on his music. The box has a timer feature that is programmed to play bird calls when the time is up. The timer can be set in five minute increments using the bookmark touch sensor and the light display. When the alarm goes off, it randomly plays one of ten sounds personalized to Rodolfo. We set Puerto Rican bird calls as the original sounds, but the sounds can be easily customized by uploading new ones to the SD card. The box has a removable false bottom that hides the electronics and battery, as well as an on/off switch so the system saves energy when not in use.

# Process
#### Ethnographic Interviews
We visited Mills College two times to interview Rodolfo. Initially, we knew very little about him - just that he was a musician and student instructor. We were curious about his creative process and motivation - where did he find inspiration? What drove him to create? What was his daily life like?

An excerpt from the first interview (edited for clarity):

> Q: What is your composing process?
>
> A: I turn off my phone, keep it away, and... it usually starts with texts. I explain what I'm doing and what I want to do. Having titles... I did this one piece called "savage matter" and that informed the shape of the work. Working around words, and synonyms around that, informed what was happening with the instruments. 
>
> I transcribe bird songs. I looked into databases for songs of birds from Puerto Rico and transcribed them. I also use breath a lot and also growls. 
>
> The text informs what I do. Once I have a conceptual background, it's on to the music.

We learned that he spends most of his time teaching or working on his compositions, and he is deeply inspired by nature and literature. He told us he didn't like using his computer when he composed - he preferred the physicality of paper and pencil. 

With our second interview, we hoped to learn more about what he struggled with. How did he deal with distractions or overcome creative blocks? We found that he utilizes various time management methods (like the Pomodoro technique), but still struggles with electronic distractions. At this point, we knew we wanted to design a product that would aide both his time management and his creative process. After about a week of ideation, we came up with the initial concepts for our book box.

#### Box Design
<img class="center" src="{{ site.baseurl }}/img/bb3.jpg" alt=""/>
We decided on a book shaped box because Rodolfo drew inspiration from literature, and we liked how the physical book shape contrasted with the concept of digital distractions.

I started with a box template from Thingiverse and modified it using Adobe Illustrator. I adapted a living hinge, added a hidden shelf for the electronics, and cut holes for the accessories (speakers, bookmark, and the on/off switch). I also etched page texture for the sides and tested different numbers of finger joints for a clean look.

Some of the things that changed between box prototypes...

* **Speaker placement**: Initially, there were holes for the speaker sounds to come through the cover. However, that made the speakers very visible when the box was open. We wanted the box to look empty when it was open, so I added cut outs inside of the box so the speakers could nest against the living hinge and the sound could come through there.

* **Cover design**: My initial design for the cover had some text engraved on it, as well as a different timer display. I eventually removed the text for a cleaner look and tested different timer displays to work with the electronics.

* **The hidden shelf**: My original hidden shelf was fixed in place. But we realized the user might need to access the battery or SD card, so I added a mechanism so the shelf could slide out.

After laser cutting our final box on sheets of 12x24x.125 inch plywood, we sanded it, painted it black, and used wood glue to reinforce the finger joints.

<div class="img_row">
	<img class="col one" src="{{ site.baseurl }}/img/bb4.png" alt=""/>
	<img class="col one" src="{{ site.baseurl }}/img/bb5.jpg" alt=""/>
	<img class="col one" src="{{ site.baseurl }}/img/bb6.jpg" alt=""/>
</div>
<div class="col three caption">
	L to R: laser cutting the box, testing a false bottom prototype, painting the box
</div>

We had to create a light filtering/diffusing system because we discovered that the Neopixel ring was very bright. In our original box prototypes, I cut out a large circle for the light ring - however, it was just too bright. After testing different light filtering designs, I found that a ring of small circles diffused the light the best. The lights were important because they let the user know how much time had been added to the timer.

<div class="img_row">
	<img class="col nine" src="{{ site.baseurl }}/img/bb8.jpg" alt=""/>
	<img class="col ten" src="{{ site.baseurl }}/img/bb7.jpg" alt=""/>
</div>
<div class="col three caption">
	Light filtering ideas
</div>

#### Electronic Components
The timer, light, and touch sensors were all programmed together using an Arduino.

The sound was handled by two separate breakout boards, one acting as a sound source/handler to generate signals and the other acting as an amplifier to drive the speakers.

<div class="img_row">
	<img class="col nine" src="{{ site.baseurl }}/img/bb9.jpg" alt=""/>
	<img class="col ten" src="{{ site.baseurl }}/img/bb10.jpg" alt=""/>
</div>

# Giving Rodolfo the Box

After several box prototypes and a lot of electronics testing, we were ready to give the box to Rodolfo. The video below includes a clip of when we went back to Mills to give Rodolfo his hyper personal product!

<div class="videoWrapper">
<iframe width="560" height="315"  src="https://www.youtube.com/embed/Z0gybnT4GPk" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>

<div class="col three caption">
	Team: Rebecca Milman, Seiyoung Jang, Malika Imhotep, Maisha Kabir
</div>

Usually with product design, you're designing for a wide user base so you have to consider different personas and make sure your product has broad appeal. With this project, we got the chance to create something very specific that likely only resonates with Rodolfo. 

After we gave Rodolfo the box, I reflected on the experience of designing for a single user. I wondered if all hyper personal designs had a degree of impracticality to them.  Where is the line between customization and hyper personal design? And what would a hyper personal product made for me look like?

