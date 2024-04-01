# lesson-17

> 🎙️ **Say:** Today marks the beginning of our explorations with computer vision. We’re going to peel back the curtain and see how computers use images & video to “see” the world around them, turning pixels into patterns, and patterns into predictions. It’s a field of study that is ongoing, current, and with many applications now and in the near future that promise to change the way that society looks and functions.






💬 **Discuss:** How might we create an algorithm so that a computer can see the difference between “X” and “O”?  (2 min)
**Discussion Goal:** A simple algorithm that students might come up with is to test whether the corners are filled in; if so, then it must be an X. They might also suggest to test to see if the lines present cross each other. Encourage students to come up with as many rules / steps as they are able to in the amount of time given. Teaching Tip
Consider having students talk to a shoulder partner for a minute or two to discuss and work out an algorithm before beginning a whole class discussion. 




💬 **Discuss:** Does your algorithm work for the examples of an “X” seen here?  Why or why not? (2 min)

**Discussion Goal:** No matter how detailed the algorithm was that students created previously, it is highly likely that it didn’t account for some variation of the ‘X’ seen here. And even if it did, it was also likely that there could be an ‘X’ drawn that did not account for the algorithm. Traditional algorithmic thinking has specific conditions to check for, but even in an example as small as this 9x9 grid, we can see that it is difficult, if not impossible, to account for all of the variations. It is important to point out that one of the main goals of computer vision technologies is to be able to train computers to recognize an “X”-- in addition to other objects– in new and novel implementations..  

> 🎙️ **Say:** Throughout this module we will be learning how computer scientists are developing sophisticated computer vision algorithms utilizing AI and data. By training these models with loads of data, the computer itself begins to write and tweak its own algorithms to help it decode and understand what an “X” might be. Even if it sees a version that it has never seen before, if the training was thorough enough, it should be able to recognize the letter. That is one of the goals of computer vision: to train computers to see and interpret the world around them just like we are able to do as human beings.



> 🎙️ **Say:** Let’s take a look at an introductory video that details the basics of what computer vision is, how it differs from traditional programming / algorithm development, and what some uses might be. 

🎥 **Video:** How AI Works: Computer Vision

💬 **Discuss:** When teaching a computer to “see”, how does machine learning differ from traditional programming?

💡 **Discussion Goal:** With traditional programming, we often hard-code in certain assumptions and conditions– like it might be an X shape if the center pixel filled in. However, that doesn’t account for situations where the X shape is askew or transformed across the canvas. Machine learning allows a computer to use data to develop an algorithm for itself. The more data that the computer has, the more accurate the guess that it can make becomes. Machine learning finds patterns by learning from its mistakes.

Teaching Tip: Title
The introduction of the speakers in this video have been truncated for the sake of pacing; however, if you would like students to know who these speakers are, consider showing them from 0:00 - 1:14 in the video.


💬 **Discuss:** What does a computer have to do in order to recognize complex shapes?

💡 **Discussion Goal:**  A computer often begins by looking at the edges within an image, and then to break down what is left into smaller, simpler patterns. An eye, in the example given, can have its edges highlighted to reveal that it contains two arcs with two concentric circles inside. By training a machine learning model using lots of data, the computer can keep increasing its accuracy with its guesses until it learns how to “see” correctly.






> 🎙️ **Say:** Read the Lesson Objectives 





> 🎙️ **Say:** Question of the Day

> 🎙️ **Say:** At the end of class today, we will revisit the objectives and the question of the day in order to assess how far we’ve come in our understanding of computer vision.


📄 **Distribute:** “The Search for Pixel” Activity Guide

Teaching Tip
“The Search for Pixel” activity is an interactive mystery game in which students will use a click-able slideshow that will navigate them to various locations around a fictional town. The goal of the activity is twofold: first and foremost, students will learn about and experience various computer vision techniques; second, students will attempt to use those techniques to help solve a mystery, finding out what happened to Pixel, a beloved, but missing cat. The game is divided into 6 rounds and each should take about 5 minutes to explore and complete. Using the first round as a model for how to interact with the interface is advisable. It is also recommended that you group students in pairs or triads in order to aid in the exploration and to make it more time-efficient.

The Activity Guide that will be given to students provides them with the instructions on how to navigate through the activity, and provides them a space to document their findings and make inferences/draw conclusions based on clues and data gathered. 

In addition to the Activity Guide, there are Clue Cards which serve as a walkthrough for each round of the activity. These should be made available as a community resource to consult as needed; not every group should have their own copy.





> 🎙️ **Say:** In order to learn a bit more about computer vision, you are all going to assume the roles of digital detectives today. You see, Pixel the cat, world famous for her thirty second advertisement for YumYumFishy Cat Bites, has gone missing! You will use an interactive Google Slide in order to visit different locations around the city, searching for information about what happened to the cat, and aided by use of computer vision techniques to reveal these clues. Have your Activity Guide and “The Search for Pixel” slide show on your computers. 



> 🎙️ **Say:** Have your Activity Guide and “The Search for Pixel” slideshow ready to go on your group’s computers. 

You will have thirty minutes to get as far as you can through the mystery. There are six rounds– and you should click on them on the main menu screen in order. Don’t try to jump ahead! As you attempt to solve the mystery, you might get stuck. If so, come up and grab one of these Clue Cards– after all, even the best detectives need a little nudge every now and again. There are two clues for each round of the mystery. Use Clue 1 first, and if you need more help, use Clue 2. If you don’t solve the mystery in the time allotted, don’t worry! Everyone will move at their own pace.

As you work through the mystery, make sure to take track of your findings and the important information that you learn about how computer vision has aided in the investigation in the Activity Guide. The best detectives always take the best notes. 

Teaching Tip
“The Search for Pixel” is a hosted slide experience on the first level within this lesson. You can also provide the slidedeck to students so that they can run it locally on their machines, but it will need to be run in Slideshow mode. It might be helpful to assign roles in the group. In a group of three, those roles might look as follows:
Driver - Responsible for clicking and navigating the group; 
Narrator - Reads important directions and clues that pop up on the screen
Scribe - Takes notes about what the team has discovered in the Activity Guide.

Set up the Clue Cards at the front of the room. There are two cards for each round (a total of 12 cards). Clue 1 for each round hints at the solution, while Clue 2 walks through how to solve the round. You might suggest that students send up a representative to read what is on the card, rather than taking the card back to their work stations. This way, you only need to print one community set of cards for everyone to use. The cards should be printed double-sided, if possible, so that they can be laid face down and the students know which one to flip over / reveal.







> 🎙️ **Say:** Let’s take a look at Round One together briefly. Let’s start by navigating to the the first scene.

✅ **Do This:** Have the groups navigate to the slideshow available as a link in Level 1. Read the directions screen (as a group or whole class). Have students navigate to the first scene by clicking on the Round One button and then on the icon of the house. 

> 🎙️ **Say:** The first thing that you should do in every new location that you visit is to click the [???] icon at the top-right of the screen. That will teach you what Computer Vision technique is available to use within that location. Once you know what Computer Vision technique you are using, click on the magnifying glass to use that technique within the scene and to search for clues!

✅ **Do This:** Students should attempt to find two clues within the first location– they are located on View 2 and 3. In order to find the clues, students must click the magnifying glass to trigger the heatmap, and then click on the red area that is shown. 

✅ **Do This:** Once students find these two clues, instruct them to return to the Main Map and begin Round Two. Each round will add one more location for the students to explore as they follow the clues leading to the missing cat. 

🔁 **Circulate:** While the students work, walk around and help as needed with groups. Familiarity with the material that is present on the Clue Cards will help you to assist students in a subtle way without giving away the answer. It is highly recommended to review them before the activity.

Teaching Tip
It might be useful to set a visible timer for 30 minutes so that students have a frame of reference for how long they have to solve the mystery.


> 🎙️ **Say:** You did it, detectives! Pixel the cat has been safely returned to her owner and can continue her brilliant career in cat food commercials.






💬 **Discuss:** Have students navigate to the Free Response level and reflect on the following question: 
What is your definition of computer vision?

💡 **Discussion Goal:** Allow students to share what they have constructed as their working definition of computer vision thus far. This definition is sure to evolve and grow as the module progresses. Some possible examples for a working definition might include:
Computer vision is like when your computer tries to figure out what's in a picture, kind of like how we recognize our friends' faces or stuff in photos
Computer vision helps computers 'see' and understand the images and videos like we do, but through cameras and algorithms
It's like teaching a computer to see and interpret the world around it, so it can recognize objects, people, and even actions
It's a part of artificial intelligence where computers are trained to interpret and understand the visual world

Assessment Opportunity: Formative Assessment
It might prove to be an interesting experience to revisit these student responses to this question at the end of the module to see what has changed and why.


> 🎙️ **Say:** Read the Learning Objectives


> 🎙️ **Say:** Review Question of the Day


✏️ **Vocabulary:** Review Key Vocabulary for the day. The specific techniques that were introduced in this mystery activity will be explored more in detail as the module progresses.



