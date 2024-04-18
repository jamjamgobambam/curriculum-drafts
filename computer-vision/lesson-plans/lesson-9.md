# Lesson 9

## Warm Up (10 mins)

> 🎙️ **Say:** We are going to start today with a game of bingo. But rather than the classic version with letters and numbers, you will be given a bingo card with a variety of statements. Your job is to walk around the classroom, talk with your classmates, and find people who agree that one of the statements describes something that they might think or do. If there is a match, have them put their initials in the box. Once you have that classmate’s initials, move on to a different person– try not to have the same set of initials twice on your card. Try not to overthink it; if the description feels generally true, then go ahead and initial it. Once you have a horizontal, vertical, or diagonal line, call out “Bingo!”

📄 **Distribute:** Give each student a bingo card.

☑️ **Do This:** Direct students to walk around and find classmates who agree with statements on their bingo card. Once they have formed a line, they should yell out "Bingo!"

💬 **Discuss:** _The boxes on the bingo cards all described different scenarios. Was there any pattern or connection between them?_

**💡 Discussion Goal:** All of the descriptions read described a situation where some level of bias might have been an influencing factor. The descriptions provided were all intended to be low risk and low impact forms of bias that are common for people to adopt without realizing that their decisions are being subtly biased.

☑️ **Do This:** Define bias.

> 🎙️ **Say:** Just like we sometimes have subtle or hidden bias that can influence our decisions or actions, so, too, can datasets and computer vision applications also have bias. Today we are going to be looking at how that might manifest while using data to train a computer vision model and discuss ways that we might be able to remedy or reduce bias so that any model that we train has a higher probability of acting in the manner which we expect that it might.

## Activity (30 mins)

🎥 **Video:** Show the video "Training Data & Bias" (0:00 to 0:50)

💬 **Discuss:** _What are some ways that data might be collected for training models?_

**💡 Discussion Goal:** The video references a few examples– pointing out that the Captcha images that are used to verify whether we are humans or bots on websites are often used to crowdsource large datasets, usually connected to an image-related task. It also introduces the idea that video streaming services collect user preference data, and uses this information, along with the preferences of like-minded users, to generate recommendations.

{% hint style="info" %}
**Teaching Tip**

Encourage students to think of some examples that exist outside of those mentioned in the video. If they cannot think of anything explicitly, you can prompt them to imagine a way to collect data from users. For example: What data do users give freely to apps like social media? How can your shopping patterns in an online store best used?
{% endhint %}

> 🎙️ **Say:** One thing to keep in mind is that the less intrusive the data-collection process is for people, the more likely they are to participate in it, and to give accurate information.

🎥 **Video:** Show the video "Training Data & Bias" (0:50 to 2:39)

💬 **Discuss:** _What are some other examples of bias in data that might exist in one of these sources:_

* _Facial recognition_
* _Voice recognition systems_
* _Social Media feeds_

**💡 Discussion Goal:** The video walks the students through an example of how medical imaging data that only uses x-rays from men might be biased and unreliable when it comes to making diagnoses on women’s x-rays. Here are some other examples that students might come up given the scenarios above: Facial recognition software - if models are trained on a variety of different ethic groups, then it might not work as intended Voice recognition systems - might be biased around certain types of accents over others Social media feeds - might only show information, groups, and stories based on what the algorithm judges as most likely to engage the user

☑️ **Do This:** Introduce the Auto-Doggie Door scenario.

💻 **Transition:** Direct students to Level 1 to access MediaPipe's Object Detection model and to download the image files to test the model with.

> 🎙️ **Say:** Upload the images one-by-one and examine the results of the object detection algorithm. Remember that you can adjust max results and score threshold to change the output of your results. You can also try changing the model / inference type that is being used within the model. If you have extra time at the end of the exploration, see if you can find your own image of a dog and upload it.
>
> As you explore these images, remember the original premise of the scenario: we are building an Auto-Dog Door that will unlock when the camera built into the door recognizes a dog and stay locked if it doesn’t recognize a dog. Therefore, you should pay close attention to the confidence score that is related to the dog images that you are uploading into the model.

☑️ **Do This:** Have students explore these images. Should they have extra time, encourage them to test more and varied images to see what the output might be. They can find additional options searching an image search tool that is available on your campus (Google Images / Pexels / Pixabay / Flickr).

🔁 **Circulate:** Assist students who are having difficulties with finding / uploading images. Point out the various settings that they can adjust while on the model and encourage them to try different combinations.

💬 **Discuss:** _What were your results? Which dogs would this model let in or locked out?_&#x20;

* Discuss as a small group first, and then bring to a whole class discussion.

💡 **Discussion Goal:** Students should note which images yield high or low confidence scores. They should share their findings about the model's accuracy in identifying different dogs and any potential patterns or biases in its decisions. Students may also bring up that they notice certain types of dogs (breed, size, face shape, color etc.) were detected less often, which could be an opportunity to reinforce the concept of bias.

💬 **Discuss:** _How might we mitigate some of the bias that we witnessed?_

💡 **Discussion Goal:** Since this is the Object Detection model, it was trained using the COCOs image dataset. That might seem to suggest that the image dataset is not robust enough to account for the variety of dogs that might need to be identified. Adding more training images of different breeds, sizes, colors, face shapes, etc. could go a long way towards alleviating low confidence scores that certain images received.

> 🎙️ **Say:** Today, we will be sharing the results of our design work thus far and getting feedback from our classmates about it. These checkpoint moments in the process of creating a project are important to learn about how you might continually iterate on your project to make it the best version possible.

📄 **Distribute:** Give each project group a copy of the Idea Outlines activity guide.

☑️ **Do This:** Have students work with their group to complete their Idea Outline activity guide.

{% hint style="info" %}
**Teaching Tip**

The Idea Outlines will be revisited in Lesson 14, so you may consider collecting these at the end of class.
{% endhint %}

☑️ **Do This:** Have students walk around the room and give general feedback to other groups’ projects. Instruct them to use one sticky note per idea that they share so that it becomes easier to sort and parse through the feedback.

{% hint style="info" %}
**Teaching Tip**

There are going to be two rounds of feedback in this activity. If you have multiple colors of sticky notes available for students, it would be a great idea to color-code the type of feedback that students are providing. For example, students can put things that they notice on yellow sticky notes, while posing their wonders / questions on blue sticky notes. This will help differentiate the types of feedback that different projects are receiving. Halfway through the activity, you can instruct students to pay attention to the predominant type of feedback that projects are receiving and to begin to provide the other type in order to achieve better balance.
{% endhint %}

☑️ **Do This:** Have students make another pass at projects, except this time they will be focusing on identifying possible sources of bias that might exist in student proposals. They can also provide suggestions for how to mitigate that bias.

{% hint style="info" %}
**Teaching Tip**

If you have a third color of sticky notes available, this activity would benefit from being differentiated by color as well. If you only have two colors of sticky notes available, consider just color-coding the feedback by round.
{% endhint %}

{% hint style="success" %}
**Assessment Opportunity**

As you make your way around the room to examine the different Idea Outlines, this would be a good time to see if students recognized the need for diverse and representative sources of data based on what sources they mention need to be collected.
{% endhint %}

## Wrap Up (5 mins)

> 🎙️ **Say:** In the next class session, please come prepared with any media that you might need to train a sample model for your computer vision application. This can take the form of physical objects, images, video, sounds, music, etc. The more data that you bring, the better the model will likely perform. If the model does not perform as well as you thought it might, there will be opportunities during upcoming project time when you can make adjustments and tweaks to your model.

💬 **Discuss:** _What physical objects, images, video, or other artifacts are you going to bring to class next to help train your model?_

💡 **Discussion Goal:** This is a good time to make sure that students are clear that they will need to be responsible for bringing training data for their model in the next class period. For example, if a student is making proposing an application that would help zookeepers know how many bananas a gorilla has eaten on a given day, then they would need to bring in a banana to train their model with– likely one that is undisturbed, and one that has been eaten and just the peel remains. Using this object, students could train a model to recognize both forms of banana, and could then use this model as a part of their application.

💻 **Transition:** Direct student to Level 1 to complete their reflection question.

* _How might bias in computer vision applications impact users differently based on their background or characteristics? How can bias in the data used to train computer vision models affect the performance and reliability of these systems?_

💡 **Reflection Goals:** To evaluate students' understanding of the differential impacts of bias, such as how facial recognition systems may perform poorly on certain demographic groups due to underrepresentation in training datasets. Students should discuss how biased training data can lead to computer vision systems that are unfair or inaccurate, particularly by failing to recognize or improperly categorizing objects or people not adequately represented in the training data.

{% hint style="success" %}
**Assessment Opportunity**

The responses in the levels can be used to formatively assess how well students have met the objectives of the lesson.
{% endhint %}
