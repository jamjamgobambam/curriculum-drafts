# Lesson 7

## Warm Up (10 mins)

> 🎙️ **Say:** In the previous lesson, we learned about the pixels and the information that they can contain. We are going to build upon our knowledge about pixels in order to envision how we might use filters to change the values stored within pixels in order to make the information more useful for computer vision applications.

☑️ **Do This:** Have student consider their favorite image filters that they use on social media or camera apps and what they like about those filters. They will share these with classmates in the next activity.

☑️ **Do This:** Direct students to participate in a Give One, Get One by sharing their favorite filter from various applications and what they like about it.

🔁 **Circulate:** Listen to student conversations that are taking place, and use some of the responses that you hear to help highlight certain applications in the class discussion that will occur next.

{% hint style="info" %}
**Teaching Tip**

Give One, Get One Give One, Get One is an excellent way to get students excited and sharing. Make sure that you click the sound icon present on the slide in order to play an accompanying song. When the song ends (48 sec.), then the students will return to their seats. Encourage them to move quickly from person to person, and challenge them to speak to at least two other classmates before the activity ends.
{% endhint %}

💬 **Discuss:** _What does your favorite filter do to an image?_

💡 **Discussion Goal:** There will be many different responses to this question. Use what you overheard when circulating the classroom to prime possible responses if the discussion becomes too focused on one type of filter. Possible filter ideas include: Beauty Filter – smoothes one’s face, giving a more youthful appearance Vintage Filter - uses sepia or other tones to make the image seem older Funny Face Filter - distorts a face that is detected in an image in a variety of ways Dance Light Filter - A filter that uses lighting and flashes inspired by one’s hands Animal Filter - Overlays a person in the image / video with some type of trait from an animal Artistic Filter - Changes an image into an interpretation of a classic or neo art style. The main goal with the conversation is to activate prior knowledge from students and to get them thinking about filters that they already know in practice.

🟡 Click the animation

💬 **Discuss:** _How long does it take to process?_

💡 **Discussion Goal:** Many filters these days are very quick! It may appear as though the filter is instant. However, other more complex filters might have a brief delay before the image is rendered completely. Students might point out that the size of the image affects how long it takes to process – the bigger the image, the slower the processing. It might also depend on the device that is used. Chromebooks, iPads, phones, and MacBook Pros all have different speeds that they can process information. Students might also point out that processing a video takes longer than an image since each frame of a video is essentially an image in and of itself.

> 🎙️ **Say:** Just like we have our own favorite filters, image detection applications have their own filters that they prefer as well. Today, we are going to take a look at one of the more common filters: edge detection.

## Activity (30 mins)

> 🎙️ **Say:** Today, you will be working with a partner to develop the steps that might go into an algorithm for separating different objects within an image. For this activity, we will only focus on images, but the processes involved in your algorithm might also apply to analyzing video as well.

**Group:** Place students in pairs or small groups of 3.

☑️ **Do This:** Have students take out a piece of paper or distribute a scrap piece of paper to each pair.

☑️ **Do This:** Direct students to create an algorithm that can be used to detect edges within an image.

🔁 **Circulate:** Spend some time with each group listening to their conversations and seeing the algorithms that develop. Encourage the students to use the Algorithm Hint Cards if they appear stuck.

{% hint style="info" %}
**Teaching Tip**

For the hint cards, you might consider taping them backwards and upside-down to a whiteboard or at the front of the room. That way, students can come up and flip the hint that they need. The back should be numbered 1 through 4 to let them know the order with which they should flip the cards. The hints are scaffolded in such a way as to gradually release more and more pertinent and directive advice as they are revealed.

You can also lay them face down, flipping up only the edge with the number on it to reveal the numbering of the clue (1 - 4)

There are two different sets of Hint Cards for the two parts of this activity (algorithm and efficiency) for the two steps in this activity. Only lay out one set at a time, or make sure that the students know which ones to consult.
{% endhint %}

☑️ **Do This:** Direct students to partner with another group to compare and contrast the algorithms that they have constructed thus far.

💬 **Discuss:** _What were some of the steps in your algorithm?_

💡 **Discussion Goal:** Students will come up with different algorithms, and have different steps involved. Some of the more important ones to discuss and point out are as follows: Looking for Changes in Brightness– edges are often delineated visually, and examining the underlying brightness of pixels might be important From this discussion point, students might ponder which color they should investigate since there are red, green, and blue values in each pixel. This is a good point and we will circle back around to this when students look to revise their algorithms. Students might also point out that differences in brightness might occur horizontally or vertically. Set a threshold value– if a pixel’s value is below (or above) the threshold value, then it is discarded. In this way, we can begin to segment or slice up an image. Finding a good threshold value might be a challenge. Use a grid to overlay the image so that you are focused on a small space at a time.

> 🎙️ **Say:** Now let’s see if we can figure out a way to try to make our algorithm run more efficiently, so that we can perform our edge detection on lots of images (or even video) almost instantaneously. As before, there are hint cards that are available if you get stuck and need some guidance.

☑️ **Do This:** Direct students to modify their algorithm to make it more efficient.

🔁 **Circulate:** Spend some time with each group listening to their conversations about proposed efficiencies. Encourage the students to use the Efficiency Hint Cards that you set up to give them a nudge towards a concept to explore.

💬 **Discuss:** _What were some of the revisions that you made to your algorithm?_

💡 **Discussion Goal:** There will be many possible student responses made here, but the two most important to bring up in discussion would be the following: Sample the image - rather than looking at a high resolution image, we can sample pixels to reconstruct a smaller version of the image. This greatly boosts performance of filtering algorithms. Reduce the color values - we learned that all pixels contain at least a red, green, and blue value (some also include an alpha, or transparency value). We can average the three values together to form one number which will display as grayscale (0 - black / 255 - white / all other values - shades of gray).

💬 **Discuss:** _To increase the processing speed of your algorithm, was there a compromise that needed to be made elsewhere?_

💡 **Discussion Goal:** An important point here is that introducing efficiencies often means reducing the fidelity of the image in some way. In the two examples referenced above, sampling an image permanently gets rid of lots of pixels within an image, and while we can infer what those might be, it is impossible to recover that data. This is similar to working with color. When we convert an image to grayscale, we lose the unique color values that are present in the pixels.

> 🎙️ **Say:** Imagine you have a huge, detailed wall mural, and you want to recreate a smaller version of it on a piece of paper. You can't capture every single detail because your paper is much smaller, so you decide to pick just the most important bits to draw.
>
> When we take digital pictures or videos, we're capturing a vast amount of visual information. But sometimes, we need to reduce the size of these images for various reasons—maybe to save space on our phones, or to make websites load faster online. When we do this, we're faced with a challenge similar to shrinking our mural: we need to decide which details are crucial to keep and which ones we can leave out.

> 🎙️ **Say:** We are continuing our work from the previous lesson with the Ideate stage. As you brainstorm today, discuss if edge detection filtering might be necessary for your computer vision application.

☑️ **Do This:** Direct students to continue brainstorming ideas for their project.

## Wrap Up (5 mins)

💻 **Transition:** Direct student to Level 1 to complete their reflection questions on Levels 1 and 2.

* _Explain the concept of edge detection in computer vision and its importance in image processing._
* _How might edge detection filters be utilized in the computer vision application you're developing?_

💡 **Reflection Goals:** Students should be able to define edge detection as a technique used to identify the boundaries or edges within images, highlighting its significance in distinguishing objects from their background, which is crucial for various computer vision applications. Encourages students to think about the practical application of edge detection in their own computer vision projects, discussing how it could improve object recognition, tracking, or other functionalities.

{% hint style="success" %}
**Assessment Opportunity**

The responses in the levels can be used to formatively assess how well students have met the objectives of the lesson.
{% endhint %}
