# lesson-1







Warm Up (10 mins)


> 🎙️ **Say:** Today marks the beginning of our explorations with computer vision. We’re going to peel back the curtain and see how computers use images & video to “see” the world around them, turning pixels into patterns, and patterns into predictions. It’s a field of study that is ongoing, current, and with many applications now and in the near future that promise to change the way that society looks and functions.

💬 **Discuss:** How might we create an algorithm so that a computer can see the difference between “X” and “O”?
**Discussion Goal:** A simple algorithm that students might come up with is to test whether the corners are filled in; if so, then it must be an X. They might also suggest to test to see if the lines present cross each other. Encourage students to come up with as many rules / steps as they are able to in the amount of time given. Teaching Tip
Consider having students talk to a shoulder partner for a minute or two to discuss and work out an algorithm before beginning a whole class discussion. 



💬 **Discuss:** Does your algorithm work for the examples of an “X” seen here? Why or why not?

💡 **Discussion Goal:** No matter how detailed the algorithm was that students created previously, it is highly likely that it didn’t account for some variation of the ‘X’ seen here. And even if it did, it was also likely that there could be an ‘X’ drawn that did not account for the algorithm. Traditional algorithmic thinking has specific conditions to check for, but even in an example as small as this 9x9 grid, we can see that it is difficult, if not impossible, to account for all of the variations. It is important to point out that one of the main goals of computer vision technologies is to be able to train computers to recognize an “X”-- in addition to other objects– in new and novel implementations..  

> 🎙️ **Say:** Throughout this module we will be learning how computer scientists are developing sophisticated computer vision algorithms utilizing AI and data. By training these models with loads of data, the computer itself begins to write and tweak its own algorithms to help it decode and understand what an “X” might be. Even if it sees a version that it has never seen before, if the training was thorough enough, it should be able to recognize the letter. That is one of the goals of computer vision: to train computers to see and interpret the world around them just like we are able to do as human beings.



> 🎙️ **Say:** Let’s take a look at an introductory video that details the basics of what computer vision is, how it differs from traditional programming / algorithm development, and what some uses might be. 

🎥 **Video:** How AI Works: Computer Vision (2:24 to 3:46)

💬 **Discuss:** When teaching a computer to “see”, how does machine learning differ from traditional programming?

💡 **Discussion Goal:** With traditional programming, we often hard-code in certain assumptions and conditions– like it might be an X shape if the center pixel filled in. However, that doesn’t account for situations where the X shape is askew or transformed across the canvas. Machine learning allows a computer to use data to develop an algorithm for itself. The more data that the computer has, the more accurate the guess that it can make becomes. Machine learning finds patterns by learning from its mistakes.

Teaching Tip
The introduction of the speakers in this video have been truncated for the sake of pacing; however, if you would like students to know who these speakers are, consider showing them from 0:00 - 1:14 of the video.



🎥 **Video:** How AI Works: Computer Vision (4:16 to 6:25)

💬 **Discuss:** What does a computer have to do to recognize complex shapes?

💡 **Discussion Goal:**  A computer often begins by looking at the edges within an image, and then to break down what is left into smaller, simpler patterns. An eye, in the example given, can have its edges highlighted to reveal that it contains two arcs with two concentric circles inside. By training a machine learning model using lots of data, the computer can keep increasing its accuracy with its guesses until it learns how to “see” correctly.









Activity (30 mins)


Group: Place students in pairs or small groups of three.

📄 **Distribute:** Give each student a copy of The Search for Pixel activity guide.

Teaching Tip
The Search for Pixel activity is an interactive mystery game in which students will use a clickable slideshow that will navigate them to various locations around a fictional town. The goals of the activity are to:
Learn about and experience various computer vision techniques
Use those techniques to find out what happened to Pixel

The game is divided into 6 rounds – each should take about 5 minutes to complete. We recommend modeling the first round to demonstrate how to interact with the slideshow.



> 🎙️ **Say:** In order to learn a bit more about computer vision, you are all going to assume the roles of digital detectives today. Pixel the cat has gone missing! You will visit different locations around the city, searching for information about what happened to the cat, and aided by use of computer vision techniques to reveal these clues.


💻 **Transition:** Direct students to Level 1 to complete The Search for Pixel activity.

Teaching Tip
It might be helpful to assign roles in the group. In a group of three, those roles might look as follows:
Driver - Responsible for clicking and navigating the group; 
Narrator - Reads important directions and clues that pop up on the screen
Scribe - Takes notes about what the team has discovered on the activity guide.

Set up the clue cards at the front of the room. There are two cards for each round (a total of 12 cards). Clue 1 for each round hints at the solution, while Clue 2 walks through how to solve the round. You might suggest that students send up a representative to read what is on the card, rather than taking the card back to their work stations. This way, you only need to print one community set of cards for everyone to use. The cards should be printed double-sided, if possible, so that they can be laid face down and the students know which one to flip over.



Wrap Up (5 mins)








💻 **Transition:** Direct student to Level 2 to complete the reflection question. 
What is your definition of computer vision?

💡 Reflection Goal: Allows students to share what they have constructed as their working definition of computer vision thus far. This definition is sure to evolve and grow as the module progresses. Some possible examples for a working definition might include:
Computer vision is like when your computer tries to figure out what's in a picture, kind of like how we recognize our friends' faces or stuff in photos
Computer vision helps computers 'see' and understand the images and videos like we do, but through cameras and algorithms
It's like teaching a computer to see and interpret the world around it, so it can recognize objects, people, and even actions
It's a part of artificial intelligence where computers are trained to interpret and understand the visual world

Assessment Opportunity: Formative Assessment
It might prove to be an interesting experience to revisit these student responses to this question at the end of the module to see what has changed and why.






