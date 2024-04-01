# Lesson 6

> 🎙️ **Say:** Today we are going to begin an in-depth study of some of the foundational technologies and ideas that go into creating some of the computer vision applications that we have examined in the case studies at the beginning of our previous lessons. The first concept that we need to understand is how computers actually “see” images. So today, we are going to take a look at the most basic units that make up images within a computer – whether on a monitor, in memory/storage, or through the lens of a digital camera.

> 🎙️ **Say:** Let’s start by investigating the Super Color Cube. Navigate to Level 1 in this lesson and click the link that you see there in order to be brought to the cube. You can drag your mouse over top in order to spin the cube around. As you interact with it, I want you to consider a few guiding questions.

☑️ **Do This:** Have students navigate to Lesson 6, Level 1. Once students have navigated to the proper level, display the next slide for discussion questions.

Teaching Tip: Title If students cannot access the Super Color Cube to interact with it themselves, then you can use the GIF supplied off of the slide frame to show the features of the app.

💬 **Discuss:** How does it appear as though the colors in the cube are organized? What do the + / - images around the cube represent?

💡 **Discussion Goal:** Students might realize that each axis (X, Y, and Z) of the cube in 3-D space represents a different color. The colors that are represented in the cube are red, green, and blue. The +/- image attached to each side of the cube represents which color belongs to which axis. It also shows how much of the color is present (full value towards the + side, lesser values towards the -) Each part of the cube shows the effect of blending these three colors together, and the new color that results from it. As such, a rainbow of possible colors can be seen.

The students will be watching three clips of a longer video about RGB colors and how they are used to comprise pixels.

🎥 **Video:** Play Clip One.

💬 **Discuss:** How are images displayed on a computer screen?

💡 **Discussion Goal:** Pixels are displayed by a combination of pixels that make up a monitor/screen. Each pixel contains a red, green, and blue light within. The blending of these colors together form every color that is visible on the screen.

Teaching Tip If students are interested in learning more about Pixels and the RGB color mode, then they can watch the whole video here: https://www.youtube.com/watch?v=15aqFQQVBWU

🎥 **Video:** Play Clip Two

💬 **Discuss:** How do computers represent the colors in pixels?

💡 **Discussion Goal:** Pixels are made up of a combination of red, green, and blue light. The intensity of that light is measured as a number from between 0 (completely off) to 255 (as bright as it can be). The blending of different intensities of red, green, and blue makes all of the hues of color on a monitor that we are familiar with.

🎥 **Video:** Play Clip Three.

💬 **Discuss:** What is the relationship between RGB values and binary?

💡 **Discussion Goal:** Since computers store information as binary numbers, we can also store the RGB color value of pixels as a series of 3 bytes (a byte contains 8 bits, representing 1s or 0s). This would mean that it would take 24 bits (8 bits x 3 colors) to store the color information of one pixel.

> 🎙️ **Say:** Lesson Objectives

> 🎙️ **Say:** Question of the Day

> 🎙️ **Say:** Today we will start by examining a computer vision technology that we see almost everyday- the QR Code? Most of us have a QR code scanner built right into our phones and our computers.

💬 **Discuss:** Where have you seen QR (Quick Response) Codes before? What function did they serve?

**Discussion Goal:** The goal here is to activate prior knowledge about QR Codes in practice. Some examples that students might share include: Payments and Transactions Event Tickets and Boarding Passes Restaurant Menus Public Transport Educational Resources and Libraries Product Information and Reviews Social Media Augmented Reality Experiences

☑️ **Do This:** Put students in pairs or groups of three for this Investigation activity.

📄 **Distribute:** Give each group the four different Sample QR Code Cards and blank paper if necessary.

💬 **Discuss:** What patterns repeat across the cards and what purpose do they serve?

💡 **Discussion Goal:** It is likely that most students have seen QR Codes before, but they are now being asked to compare and find patterns that exist between all of the samples that they are shown. The first pattern that they may see is the bullseye-looking one in the upper left/right and bottom left corners. These are called Position Markers. Students might realize that they are there to help align the image when it is scanned so that the scanner knows which end is up and which end is down. On the larger QR Codes, they might also see smaller bullseye patterns repeating at regular intervals. These are designed to help the QR Code scanner normalize an image – that is, correct is perspective if the camera takes an image at an angle and warps the QR square.

🟡 Click the animation

💬 **Discuss:** How might a QR Code store useful information?

💡 **Discussion Goal:** Discuss the structure of QR codes, including the black and white squares, and how these patterns translate into digital data that can be read by a scanner or smartphone camera. Since there are only filled and non-filled squares, make a connection to the Warm-up in which you discussed bits (binary digits). The squares could represent 1s or 0s if they are filled or not filled. Some students might point out that you need set an order in which to “read” the bits of data, otherwise any binary message that is contained in the QR Code would get scrambled. Therefore, it is important to agree to a set of rules that helps us to encode and decode the bits in a certain order.

Teaching Tip: Extra Enrichment If you would like for students to get hands on practice with normalizing an image, then students can complete the QR Code Extra Enrichment activity which asks them to normalize the Position Markers in a QR Code using a warping tool. The goal of the activity is to normalize the QR Code enough so that it is able to be scanned and read.

Say: You did an excellent job in your exploration of QR Codes and brought up many interesting and important observations! Within a QR Code, data is encoded using bits (1s & 0s) represented by white and black colors. Here we can see that the black squares represent a 0 and the white squares represent a 1.

> 🎙️ **Say:** Knowing the order that these bits are read in a QR Code is important! Here in the GIF on the screen, we can see one of the ways that bytes of data can be read from a QR Code. The pattern through which the data is read is important. Look at how it zig-zags back and forth in each block of data. The order that the QR Code bits are read represents a corresponding place in a binary number, starting with the left-most digit and moving right.

As we saw in the Warm-up today, when we have a byte of information, we can represent a number from between 0 and 255.

> 🎙️ **Say:** We are now going to complete an activity in which we work to decode and encode data into this QR Code format.

📄 **Distribute:** QR Code Exploration Activity Guide.

> 🎙️ **Say:** The diagrams for how to decode these bytes of data are available in your QR Code Exploration Activity Guide for reference. Work with your group to first decode the binary number that is encoded in the data, and then to convert that binary number into a base-10 number. There is a link available within the lesson that will convert these numbers for you.

Teaching Tip: Binary to Base 10 Modeling This might be a good place to model how to input binary numbers into the resource website that is provided in order to make the conversion between binary and base 10. If this particular site is blocked on your campus, Google “Binary to Base 10”-- there are a number of alterate sites that might be available for use.

As students work through the decoding,consider the following roles: have one group member use their finger to trace the zig zag pattern, have another group member call out whether it is a 1 (white) or a 0 (black) and have a third student jot down the digit in the proper location within binary string (starting on the left, moving to the right). Have the team members switch roles for every QR Code byte that they are decoding.

🔁 **Circulate:** Circulate around and check that students are using the proper decoding patterns.

💬 **Discuss:** What numbers did we decode?

💡 **Discussion Goal:** 0, 173, and 188.

🟡 Click the animation

💬 **Discuss:** What can be represented with 3 numbers?

💡 **Discussion Goal:** These numbers could reference a lot of things. It could represent the three different color values (red, green, and blue) contained within in a pixel. It could represent different numbers in the ASCII table - a table that contains numerical representations of character such as 'a' or '@' or an action of some sort. In short, it could represent anything, as long as the scanner is programmed how to translate the value shown into a different representation.

☑️ **Do This:** Instruct students to follow the link within the lesson, or to use Google to search “Color picker”. Then, have them put the three values, in order, into the RGB box to reveal the mystery color that was encoded into this QR Code.

💬 **Discuss:** What color do we get?

💡 **Discussion Goal:** In this case, we are treating these bytes of data as colors (remember that there are other options as well!) By entering them into the color picker, we receive the famous Code.org Teal color– the same one present in the header of this slide.

> 🎙️ **Say:** Here you can see that by treating these three bytes of data as a pixel, we can extract a color from it! Here are the binary numbers that you should have decoded, along with the base-10 equivalents.

> 🎙️ **Say:** We’ve learned how to decode data, so let’s go the other way and try our hand at encoding data into this QR Code format.

☑️ **Do This:** Have students continue on to the next section in the Activity Guide. They will be asked to choose their favorite color to encode, using the Google Color Picker to select it. After jotting down the RGB number equivalents of their color, they will convert these three numbers into their binary equivalents using the same link that they used previously. Last, they will create a QR code representation using the diagram within the Activity Guide.

Teaching Tip: Update the Converter Since students are now going to be converting from base-10 to binary, have them select the appropriate options in the drop down menus within the converter.

As an enrichment, students can trade their favorite colors with another classmate to have them decode. You could also create a “QR Wall” in the classroom in which students cut out their RGB QR Code images and tape them up, so that other students see and decode their classmates’ favorite colors.

> 🎙️ **Say:** As we wrap up this portion of the lesson today, an important takeaway is the following –

All computer vision applications are created upon the same foundation: Being able to identify, manipulate, and make predictions about the data stored in the pixels that constitute images and video.

> 🎙️ **Say:** Today, we will move on from the second step in the Design Thinking Process: Defining. In that step, we gathered data, made visualizations that helped us extract insight and meaning, and then used those insights to craft user personas that help create a hypothetical users in our target community.From our user personas, we created a problem statement to help clarify what might be in issue of greatest need for those users.

🟡 Click the animation

> 🎙️ **Say:** Now we are moving onto Ideating. In this step, we will take the user personas that we have created and will brainstorm many different solutions that we might address the problem statement and provide a value for our users.

> 🎙️ **Say:** Make sure that you and group members have access to the user personas and problem statement that you created previously. We will be working with these artifacts in order to begin our brainstorming process.

📄 **Distribute:** The Lotus Blossom brainstorming document. Students can also work on it digitally, or create their own version of it on a blank sheet of paper.

Teaching Tip: Time to Ideate! There are three project work days that are devoted to this Ideating Phase, so students will not need to complete this activity in class today. The next lessons build in more time to add, to hone and to refine what they begin today.

☑️ **Do This:** Have students navigate to Lesson 6, Level 3 .

This page contains a walkthrough of how to implement the Lotus Blossom brainstorming technique. If you desire to walk them through the initial steps of the process, the next few slides model the process.

> 🎙️ **Say:** Put the problem statement that your group developed in the Define phase in the center-bottom box– the one ringed with five spaces. These five boxes will blossom out into unique ideas and solutions as you ideate. No idea is too wild! Brainstorming involves letting one’s mind drift and expand, and it is useful to include possibilities that might seem outlandish at first.

✅ **Do This:** Students take the most promising ideas that their group came up with and transfer them into the center of a new Lotus Blossom square. For each of these ideas, they will dig deeper into exploring it as a possible solution. Students should surround each of these “blossoms” with: Supporting details Questions that arise Issues that they foresee Far-fetched wishes Links to resources

The more detail, the better! Students have plenty of time to do a thorough job ideating solutions that are aligned with the greatest need of their target community.

> 🎙️ **Say:** Here we can see s sample brainstorm using the Lotus Blossom technique. The problem statement that this group has identified is "Gardeners always mention a lack of time, and wish for a smart solution to know how to best tend to their crop". There are many ideas that are generated as possible solutions.

Teaching Tip: No One-Size-Fits-All Solutions! Notice that there is no need to come up with one solution that solves every possible problem. The problem statement can and should be broken up into many solutions that each tackle one aspect of the larger problem which the community faces.

> 🎙️ **Say:** We will continue our work with our Lotus Blossom diagrams, focusing on adding more ideas / solutions and providing greater depth and supporting details to those that we have uncovered thus far.

> 🎙️ **Say:** Lesson objectives

> 🎙️ **Say:** Question of the Day

> 🎙️ **Say:** Key vocabulary
