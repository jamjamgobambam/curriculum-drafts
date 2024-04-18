# Lesson 6

## Warm Up (10 mins)

> 🎙️ **Say:** Today we are going to explore how computers actually "see" images. We'll take a look at the most basic units that make up images within a computer – whether on a monitor, in memory/storage, or through the lens of a digital camera.

🎥 **Video:** Show the video "Images, Pixels, and RGB" (0:43 to 1:36).

💬 **Discuss:** _How are images displayed on a computer screen?_

💡 **Discussion Goal:** Pixels are displayed by a combination of pixels that make up a monitor/screen. Each pixel contains a red, green, and blue light within. The blending of these colors together form every color that is visible on the screen.

{% hint style="info" %}
**Teaching Tip**

If students are interested in learning more about Pixels and the RGB color mode, then they can watch the whole video here: https://www.youtube.com/watch?v=15aqFQQVBWU
{% endhint %}

🎥 **Video:** Show the video "Images, Pixels, and RGB" (2:07 to 5:50).

💬 **Discuss:** _How do computers represent the colors in pixels?_

💡 **Discussion Goal:** Pixels are made up of a combination of red, green, and blue light. The intensity of that light is measured as a number from between 0 (completely off) to 255 (as bright as it can be). The blending of different intensities of red, green, and blue makes all of the hues of color on a monitor that we are familiar with.

🎥 **Video:** Show the video "Images, Pixels, and RGB" (3:32 to 4:01).

💬 **Discuss:** _What is the relationship between RGB values and binary?_

💡 **Discussion Goal:** Since computers store information as binary numbers, we can also store the RGB color value of pixels as a series of 3 bytes (a byte contains 8 bits, representing 1s or 0s). This would mean that it would take 24 bits (8 bits x 3 colors) to store the color information of one pixel.

## Activity (30 mins)

> 🎙️ **Say:** Let's start by examining a computer vision technology that we see almost everyday- the QR Code? Most of us have a QR code scanner built right into our phones and our computers.

💬 **Discuss:** _Where have you seen QR codes before? What function did they serve?_

💡 **Discussion Goal:** The goal here is to activate prior knowledge about QR Codes in practice. Some examples that students might share include: Payments and Transactions Event Tickets and Boarding Passes Restaurant Menus Public Transport Educational Resources and Libraries Product Information and Reviews Social Media Augmented Reality Experiences

Group: Place students in pairs or small groups of 3.

💬 **Discuss:** _What patterns repeat across the cards and what purpose do they serve?_

💡 **Discussion Goal:** It is likely that most students have seen QR Codes before, but they are now being asked to compare and find patterns that exist between all of the samples that they are shown. The first pattern that they may see is the bullseye-looking one in the upper left/right and bottom left corners. These are called Position Markers. Students might realize that they are there to help align the image when it is scanned so that the scanner knows which end is up and which end is down. On the larger QR Codes, they might also see smaller bullseye patterns repeating at regular intervals. These are designed to help the QR Code scanner normalize an image – that is, correct is perspective if the camera takes an image at an angle and warps the QR square.

💬 **Discuss:** _How do you think QR codes store information?_

💡 **Discussion Goal:** Discuss the structure of QR codes, including the black and white squares, and how these patterns translate into digital data that can be read by a scanner or smartphone camera. Since there are only filled and non-filled squares, make a connection to the Warm-up in which you discussed bits (binary digits). The squares could represent 1s or 0s if they are filled or not filled. Some students might point out that you need set an order in which to “read” the bits of data, otherwise any binary message that is contained in the QR Code would get scrambled. Therefore, it is important to agree to a set of rules that helps us to encode and decode the bits in a certain order.

🎥 **Video:** Show the video "How do QR Codes Work: Explained in Minutes"

💬 **Discuss:** _What surprises you about how QR codes work?_

💡 **Discussion Goal:** Students highlight different aspects of QR codes that surprised them, such as the different elements, error correction, or how it encodes data.

{% hint style="info" %}
**Teaching Tip**

[**This article**](https://typefully.com/DanHollick/qr-codes-T7tLlNi) is also a helpful resource for explaining how QR codes work. You may want to share this article with the class, focusing specifically on the section starting at "Finally we get to the actual data" to highlight how the data is encoded into the QR code.
{% endhint %}

> 🎙️ **Say:** Within a QR code, data is encoded using bits (1s & 0s) represented by white and black colors. Here we can see that the black squares represent a 0 and the white squares represent a 1.

> 🎙️ **Say:** Knowing the order that these bits are read in a QR code is important! Here is one of the ways that bytes of data can be read from a QR Code. The order that the QR code bits are read represents a corresponding place within a binary number, starting with the left-most digit and moving right.

🟡 Click the animation

**Group:** Place students in pairs or small groups of 3.

📄 **Distribute:** Give each pair a copy of the QR Code Exploration activity guide.

☑️ **Do This:** Direct students to complete the QR Code Exploration activity guide.

{% hint style="info" %}
**Teaching Tip**

This might be a good place to model how to input binary numbers into the resource website that is provided to make the conversion between binary and base 10. If this particular site is blocked on your campus, search for “Binary to Base 10”-- there are a number of alternate sites that might be available for use.

As students work through the decoding, consider the following roles: have one group member use their finger to trace the zig zag pattern, have another group member call out whether it is a 1 (white) or a 0 (black) and have a third student jot down the digit in the proper location within binary string (starting on the left, moving to the right). Have the team members switch roles for every QR Code byte that they are decoding.
{% endhint %}

> 🎙️ **Say:** As we wrap up this portion of the lesson today, an important takeaway is the following – All computer vision applications are created upon the same foundation: Being able to identify, manipulate, and make predictions about the data stored in the pixels that make up images and video.

> 🎙️ **Say:** Today, we will move on from the second step in the Design Thinking Process: Defining. In that step, we gathered data, made visualizations that helped us extract insight and meaning, and then used those insights to craft user personas that help create a hypothetical users in our target community. From our user personas, we created a problem statement to help clarify what might be in issue of greatest need for those users. Now we are moving onto Ideating. In this step, we will take the user personas that we have created and will brainstorm many different solutions that we might address the problem statement and provide a value for our users.

> 🎙️ **Say:** Ideate involves us coming up with creative ideas that will address the problem we’ve defined..

**Group:** Place students in their project groups.

📄 **Distribute:** Give each group a copy of the Lotus Blossom Diagram activity guide.

{% hint style="info" %}
**Teaching Tip**

There are three project work days that are devoted to this Ideating phase, so students will not need to complete this activity in class today. The next lessons build in more time to add and refine what they begin today.
{% endhint %}

☑️ **Do This:** Introduce the first two steps of creating the lotus blossom.

☑️ **Do This:** Introduce the next two steps of creating the lotus blossom.

> 🎙️ **Say:** Here we can see a sample brainstorm using the Lotus Blossom technique. The problem statement that this group has identified is "Gardeners always mention a lack of time and wish for a smart solution to know how to best tend to their crop". There are many ideas that are generated as possible solutions.

{% hint style="info" %}
**Teaching Tip**

Notice that there is no need to come up with one solution that solves every possible problem. The problem statement can and should be broken up into many solutions that each tackle one aspect of the larger problem which the community faces.
{% endhint %}

☑️ **Do This:** Direct students to work on their Lotus Blossom activity guide.

## Wrap Up (5 mins)

💻 **Transition:** Direct student to Level 3 to complete their reflection question.&#x20;

* _Considering what you've learned about pixels and RGB values, what kinds of information do you think computer vision algorithms can extract from images, and for what purposes?_

💡 **Reflection Goal:** Encouraging students to think broadly about the applications of computer vision, including color detection, pattern recognition, and object identification, and how these capabilities can serve various purposes across industries.

{% hint style="success" %}
**Assessment Opportunity**

The responses in the level can be used to formatively assess how well students have met the objectives of the lesson.
{% endhint %}
