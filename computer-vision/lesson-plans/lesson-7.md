# lesson-7

🎙Remarks
Yesterday we learned about the pixels and the information that they can contain. We are going to build upon our knowledge about pixels in order to envision how we might use filters to change the values stored within pixels in order to make the information more useful for computer vision applications.






🖼️ Display & Read: The prompt for the brainstorming activity.

✅ **Do This:** Have students think for 30 sec to a minute about their response to the brainstorm prompt.


✅ **Do This:** Students will get up and circulate around the room, sharing their favorite filter from various applications and what they like about it. 

🔁 **Circulate:** Listen to student conversations that are taking place, and use some of the responses that you hear to help highlight certain applications in the class discussion that will occur next.

Teaching Tip
Give One, Get One is an excellent way to get students excited and sharing. Make sure that you click the sound icon present on the slide in order to play an accompanying song. When the song ends (48 sec.), then the students will return to their seats. Encourage them to move quickly from person to person, and challenge them to speak to at least two other classmates before the activity ends.


💬 **Discuss:** What does your favorite filter do to an image? There will be many different responses to this question. Use what you overheard when circulating the classroom to prime possible responses if the discussion becomes too focused on one type of filter. Possible filter ideas include:
Beauty Filter – smoothes one’s face, giving a more youthful appearance
Vintage Filter - uses sepia or other tones to make the image seem older
Funny Face Filter - distorts a face that is detected in an image in a variety of ways
Dance Light Filter - A filter that uses lighting and flashes inspired by one’s hands
Animal Filter - Overlays a person in the image / video with some type of trait from an animal
Artistic Filter - Changes an image into an interpretation of a classic or neo art style.

**Discussion Goal:** The main goal with the conversation is to activate prior knowledge from students and to get them thinking about filters that they already know in practice. 

💬 **Discuss:** “How long does it take to process?” 

**Discussion Goal:** Many filters these days are very quick! It may appear as though the filter is instant. However, other more complex filters might have a brief delay before the image is rendered completely. Students might point out that the size of the image affects how long it takes to process – the bigger the image, the slower the processing. It might also depend on the device that is used. Chromebooks, iPads, phones, and MacBook Pros all have different speeds that they can process information. Students might also point out that processing a video takes longer than an image since each frame of a video is essentially an image in and of itself.

🎙Remarks
Just like we have our own favorite filters, image detection applications have their own filters that they prefer as well. Today, we are going to take a look at one of the more common filters: edge detection.





🖼️ Display & Read: Consider having student volunteers read the bulleted objectives


🖼️ Display & Read: Consider having a student volunteer read the Question of the Day


🎙Remarks
Today, you will be working in a group, you will be working on developing the steps that might go into an algorithm for separating different objects within an image. For this activity, we will focus only thinking about images, but the processes involved in your algorithm might also apply to analyzing video as well.

Teaching Tip
The recommendation is to have a group of 3-4 students in order to maximize personal contribution vs. time expenditure on the task


🎙Remarks
You and your partner are going to decompose and outline the steps necessary to create one of the most important filters in computer vision applications: the edge detection filter. You can see what one example of the filter might look like in the image seen here.

✏️ **Vocabulary:** Edge Detection Filter - A method of modifying pixels within an image in order to approximate where edges might be found


⏳ Type & Time:  Unplugged Activity (no computers needed). 10 minutes per section (2 sections total).

📄 **Distribute:** For this activity, students will need access to two different colored sticky notes and a writing utensil at their desk.

📄 Class Resource: There is a set of scaffolded hint cards that can help groups that are stuck get back on track. There should be one set for the classroom, and their location should be shared with the class. 



✅ **Do This:** Students will spend 10 minutes in their group, creating an algorithm that can be used to detect edges within an image. They should put each step of their algorithm on its own post-it note. Students should be encouraged to add sticky notes as ideas pop up, remove sticky notes that no longer seem applicable, and move them around as the steps and process evolve.

🔁 **Circulate:** Spend some time with each group listening to their conversations and seeing the algorithms that develop. Encourage the students to use the Algorithm Hint Cards that you set up if they appear stuck in their thinking or need a nudge to crystallize a concept. 

Teaching Tip
For the hint cards, you might consider taping them backwards and upside-down to a whiteboard or at the front of the room. That way, students can come up and flip the hint that they need. The back should be numbered 1 through 4 to let them know the order with which they should flip the cards. The hints are scaffolded in such a way as to gradually release more and more pertinent and directive advice as they are revealed.

There are two different sets of Hint Cards (algorithm and efficiency) for the two steps in this activity. Make sure that students know which one is which!

If you do not have access to different colored sticky notes, possible revisions of the activity include:
Use a singular color sticky, but put the heading “Algorithm” at the top the sticky notes used in this first part.
You might use cut up strips of paper as well to accomplish the same task.



✅ **Do This:** Have the students hold up their fingers to show how many sticky notes they used to “make” their edge detection filter💬 **Discuss:** What were some of the important steps in your algorithm?
**Discussion Goal:** Students will come up with different algorithms, and have different steps involved. Some of the more important ones to discuss and point out are as follows:
Looking for Changes in Brightness– edges are often delineated visually, and examining the underlying brightness of pixels might be important
From this discussion point, students might ponder which color they should investigate since there are red, green, and blue values in each pixel. This is a good point and we will circle back around to this when students look to revise their algorithms.
Students might also point out that differences in brightness might occur horizontally or vertically.
Set a threshold value– if a pixel’s value is below (or above) the threshold value, then it is discarded. In this way, we can begin to segment or slice up an image. Finding a good threshold value might be a challenge.
Use a grid to overlay the image so that you are focused on a small space at a time

💬 **Discuss:** What are some of the challenges that remain?
**Discussion Goal:** Students might point out that there seems to be a lot of computations that are happening, but they are unclear what those are (This is to be expected!). Students might bring up the fact that some images have lots of noise in them, especially older or low light images, and it might be hard to find distinct edges when looking for differences in brightness. 

🎙Remarks
Another challenge that remains for us is how we deal with lots of large images. The bigger the image, the more processing power it will take to compute our algorithms. Let’s think about that point for a moment…





🎙Remarks
Let’s see if we can figure out a way to try to make our algorithm run more efficiently, so that we can perform our edge detection on lots of images (or even video) almost instantaneously.


✅ **Do This:** Students will spend 10 minutes in their group. In this activity, students will use the other color sticky note to denote that they are making a revision to their original algorithm. This will require moving around sticky notes and revisiting parts of their previous algorithm.

🔁 **Circulate:** Spend some time with each group listening to their conversations about proposed efficiencies. Freely encourage the students to use the Efficiency Hint Cards that you set up to give them a nudge towards a concept to explore. 






💬 **Discuss:** What were some of the revisions that you made to your algorithm?

**Discussion Goal:** There will be many possible student responses made here, but the two most important to bring up in discussion would be the following:
Shrink the image size - rather than looking at a high resolution image, we can sample pixels to reconstruct a smaller version of the image. This greatly boosts performance of filtering algorithms.
Reduce the color values - we learned that all pixels contain at least a red, green, and blue value (some also include an alpha, or transparency value). We can average the three values together to form one number which will display as grayscale (0 - black / 255 - white / all other values - shades of gray).

💬 **Discuss:** To increase the processing speed of your algorithm, was there a compromise that needed to be made elsewhere?

**Discussion Goal:** An important point here is that introducing efficiencies often means reducing the fidelity of the image in some way. In the two examples referenced above, sampling an image permanently gets rid of lots of pixels within an image, and while we can infer what those might be, it is impossible to recover that data. This is similar to working with color. When we convert an image to grayscale, we lose the unique color values that are present in the pixels. 

🎙Remarks
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.


🎙Remarks
Two of the most common efficiences that we can take advantage of in computer vision are sampling images in order to make the file size smaller, as well as converting the image to grayscale or even black & white. An edge detection algorithm does not require a full color, high resolution image in order to process. Quite the opposite! 

Teaching Tip
If you would like to model what sampling looks like for the class, this widget will allow you to load an image and adjust the sample size in pixels. The result is a downscaled image that would process much faster than the full image. In this widget, we zoom in on the downscaled image so that the individual pixels are easily seen rather than simply showing a smaller version.


🖥️ Model: Use this widget to load an image and to to demonstrate how we find edges by finding differences in pixel values. The GIF has also been sampled and had its color reduced to grayscale.

Teaching Tip
There are several different sample images that you can use to illustrate edge detection can work by finding differences in pixel values. Presenting this widget to students to experiment with would be an excellent enrichment for this lesson.


Your camera takes in a lot of info besides the QR code- how does it know to focus in on that?  What is your idea going to focus on?  How will the image need to be normalized?

✏️ **Vocabulary:** Lorem ipsum dolor sit amet, consectetur adipiscing elit
🔁 **Circulate:** Lorem ipsum dolor sit amet, consectetur adipiscing elit
📄 **Distribute:** Lorem ipsum dolor sit amet, consectetur adipiscing elit
✅ **Do This:** Lorem ipsum dolor sit amet, consectetur adipiscing elit
💬 **Discuss:** Lorem ipsum dolor sit amet, consectetur adipiscing elit
**Discussion Goal:** Lorem ipsum dolor sit amet, consectetur adipiscing elit
🖥️ Model: Lorem ipsum dolor sit amet, consectetur adipiscing elit
🎥 **Video:** Lorem ipsum dolor sit amet, consectetur adipiscing elit
> 🎙️ **Say:** Lorem ipsum dolor sit amet, consectetur adipiscing elit
🖼️ Display: Lorem ipsum dolor sit amet, consectetur adipiscing elit

🎙Remarks
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.

Teaching Tip
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Aliquam etiam erat velit scelerisque in dictum non. (DELETE IF NOT NEEDED)

Assessment Opportunity
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Aliquam etiam erat velit scelerisque in dictum non. (DELETE IF NOT NEEDED)


🎙Remarks
We are continuing our work from yesterday with the Ideate Stage from the Design Thinking Process. As you brainstorm today, discuss if edge detection filtering might be necessary for your proposal, and what efficiences you might want to pursue as a result.

📄 Resource: The Lotus Blossom brainstorming document. Students can also work on it digitally, or create their own version of it on a blank sheet of paper.

Teaching Tip
This is day 2 of 3 for the Ideate Phase of the PBL work days. Students should aim to add additional possible solutions and details to their brainstorm.



🖼️ Display: A sample brainstorm using the Lotus Blossom technique. The problem statement that this group has identified is "Gardeners always mention a lack of time, and wish for a smart solution to know how to best tend to their crop". There are many ideas that are generated as possible solutions. 

Teaching Tip
Notice that there is no need to come up with one solution that solves every possible problem. The problem statement can and should be broken up into many solutions that each tackle one aspect of the larger problem which the community faces.










> 🎙️ **Say:** We will finish our work with our Lotus Blossom diagrams, focusing on adding more ideas / solutions and providing greater depth and supporting details to those that we have uncovered thus far.


🖼️ Display: The day’s learning


🖼️ Display: The Question of the Day


🖼️ Display: The key vocabulary from today’s lesson


