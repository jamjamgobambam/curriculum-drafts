# Lesson 9

## Overview (Teacher)

**How might bias affect users who engage with computer vision applications?**

Students will engage with the concept of bias, first by hearing about and generating examples of it in the decision-making process. This concept will then be applied to the data on which computer vision models are trained. The importance of having a diversity and depth of data is emphasized. While working on the module project, students can share their project brainstorms and solicit feedback from their peers.

## Overview (Students)

Today you are going to examine and expience how bias might influence the decision-making process of a program using machine learning.. The importance of having a diversity and depth of data is emphasized. While working on the module project, you will share your project brainstorms with your peers and solicit feedback from them.



{% tabs %}
{% tab title="Slides" %}
{% embed url="https://docs.google.com/presentation/d/1WCPTEuqRy5oG7rVbA9ZfKj_0Iyla5POTSMhgcTg3GiA/edit?usp=sharing" %}
{% endtab %}

{% tab title="Standards" %}
| AI4K12 (3-C-iii) | Investigate imbalances in training data in terms of gender, age, ethnicity, or other demographic variables that could result in a biased model, by using a data visualization tool. |
| ---------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| CSTA: 3A-IC-25   | Test and refine computational artifacts to reduce bias and equity deficits                                                                                                          |
{% endtab %}

{% tab title="Objectives" %}
Students will be able to:

* Identify potential bias in computer vision systems
* Interpret how bias might best be mitigated
* Evaluate the results of the Ideating phase of the Design Thinking Process
{% endtab %}

{% tab title="Preparation" %}
* Print out the Bingo cards for the lesson’s warm-up.
* Double-check that students can access the MediaPipe website and download the dog images provided.
{% endtab %}

{% tab title="Links" %}
For the teachers

* [Blind Spots Exposed](https://docs.google.com/presentation/d/1WCPTEuqRy5oG7rVbA9ZfKj\_0Iyla5POTSMhgcTg3GiA/edit?usp=sharing)- Slides
* [AI: Training Data & Bias](https://youtu.be/x2mRoFNm22g?feature=shared) - Video
* [Bingo Cards](https://docs.google.com/document/d/1CVVcl57spqa4X1NZvio48RGahtt03Ic5BIV38t527Lo/edit?usp=sharing) - Key

For the students

* [Dog Images](https://drive.google.com/file/d/1dnhvbfde7zKupHwz6LjTGTP\_OGbp3wPp/view) - Resource
{% endtab %}

{% tab title="Vocabulary" %}
Bias - Decisions that favor some things and deprioritize or exclude others.
{% endtab %}
{% endtabs %}

> 🎙️ **Say:** To begin with today, we are going to play a little bingo game. But rather than the classic version with letters and numbers, you will be given a Bingo card with a variety of statements. Within a set time limit, your job is to circulate around the classroom, talk with your classmates, and find people who agree that one of the statements describes something that they might think or do.

If there is a match, have them put their initials in the box. Once you have that classmate’s initials, move on to a different person– try not to have the same set of initials twice on your card.

Try not to overthink it; if the description feels generally true, then go ahead and initial it.

Once you have a horizontal, vertical, or diagonal line, call out “Bingo!”

📄 **Distribute:** Bingo Cards.

💬 **Discuss:** The boxes on the Bingo card all described different scenarios, but was there any pattern or connection between them?

**Discussion Goal:** All of the descriptions read described a situation where some level of bias might have been an influencing factor. Bias is defined as having a tendency to prefer one’s own viewpoint / outlook towards a particular subject. The descriptions provided were all intended to be low risk and low impact forms of bias that are common for people to adopt without realizing that their decisions are being subtly biased.

> 🎙️ **Say:** Just like we sometimes have subtle or hidden bias that can influence our decisions or actions, so, too, can datasets and computer vision applications also have bias. Today we are going to be looking at how that might manifest while using data to train a computer vision model and discuss ways that we might be able to remedy or reduce bias so that any model that we train has a higher probability of acting in the manner which we expect that it might.

✏️ **Vocabulary:** Bias - when a decision favors some things and deprioritizes or excludes others.

🖼️ Display: Lesson Objectives

🖼️ Display: Question of the Day

🎥 **Video:** Training Data & Bias, Part 1 of 2

💬 **Discuss:** What are some ways that data might be collected for training models?

**Discussion Goal:** The video references a few examples– pointing out that the Captcha images that are used to verify whether we are humans or bots on websites are often used to crowdsource large datasets, usually connected to an image-related task. It also introduces the idea that video streaming services collect user preference data, and uses this information, along with the preferences of like-minded users, to generate recommendations.

Extension: Encourage students to think of some examples that exist outside of those mentioned in the video. If they cannot think of anything explicitly, you can prompt them to imagine a way to collect data from users. For example: What data do users give freely to apps like social media? How can your shopping patterns in an online store best used?

> 🎙️ **Say:** One thing to keep in mind is that the less intrusive the data-collection process is for people, the more likely they are to participate in it, and to give accurate information.

🎥 **Video:** Training Data & Bias, Part 2 of 2

> 🎙️ **Say:** This video mentions one potential example of bias that exists in data, but let’s dig a little deeper and see if we can think of some more.

💬 **Discuss:** What are some other examples of bias in data that might exist in one of these sources: Facial recognition Voice recognition systems Social Media feeds

**Discussion Goal:** The video walks the students through an example of how medical imaging data that only uses x-rays from men might be biased and unreliable when it comes to making diagnoses on women’s x-rays. Here are some other examples that students might come up given the scenarios above: Facial recognition software - if models are trained on a variety of different ethic groups, then it might not work as intended Voice recognition systems - might be biased around certain types of accents over others Social media feeds - might only show information, groups, and stories based on what the algorithm judges as most likely to engage the user

> 🎙️ **Say:** Let’s examine a hypothetical usage of computer vision to solve a problem that may be of interest to dog lovers the world over.

☑️ **Do This:** Have a student volunteer read the Auto-Doggie Door scenario

> 🎙️ **Say:** We are going to revisit Mediapipe’s Object Detection model in order to see how well it might accomplish the task of identifying dogs for the Auto-Doggie Door.

☑️ **Do This:** Have students navigate to Mediapipe’s Object Detecton site.

> 🎙️ **Say:** There is another series of images for you to download, and they are located within the Dogs resource folder. There are three different images for you to test.

☑️ **Do This:** Have students download the images from the Dogs folder (3) in order to test them.

> 🎙️ **Say:** Upload the images one-by-one and examine the results of the object detection algorithm. Remember that you can adjust max results and score threshold to change the output of your results. You can also try changing the model / inference type that is being used within the model. If you have extra time at the end of the exploration, see if you can find your own image of a dog and upload it.

As you explore these images, remember the original premise of the scenario: we are building an Auto-Dog Door that will unlock when the camera built into the door recognizes a dog and stay locked if it doesn’t recognize a dog. Therefore, you should pay close attention to the confidence score that is related to the dog images that you are uploading into the model.

☑️ **Do This:** Have students explore these images. Should they have extra time, encourage them to test more and varied images to see what the output might be. They can find additional options searching an image search tool that is available on your campus (Google Images / Pexels / Pixabay / Flickr)

🔁 **Circulate:** Assist students who are having difficulties with finding / uploading images. Point out the various settings that they can adjust while on the model and encourage them to try different combinations.

💬 **Discuss:** What were your results? Which dogs would this model let in or locked out? Discuss as a small group first, and then bring to a whole class discussion.

💡 **Discussion Goal:** Students should note which images yield high or low confidence scores. They should share their findings about the model's accuracy in identifying different dogs and any potential patterns or biases in its decisions. Students may also bring up that they notice certain types of dogs (breed, size, face shape, color etc.) were detected less often, which could be an opportunity to reinforce the concept of bias.

🟡 Click the animation

💬 **Discuss:** How might we mitigate some of the bias that we witnessed? Whole class discussion

💡 **Discussion Goal:** Since this is the Object Detection model, it was trained using the COCOs image dataset. That might seem to suggest that the image dataset is not robust enough to account for the variety of dogs that might need to be identified. Adding more training images of different breeds, sizes, colors, face shapes, etc. could go a long way towards alleviating low confidence scores that certain images received.

> 🎙️ **Say:** Today, we will be sharing the results of our design work thus far and getting feedback from our classmates about it. These checkpoint moments in the process of creating a project are important to learn about how you might continually iterate on your project to make it the best version possible.

☑️ **Do This:** Have students work with their group to complete the “Our Idea Outline” portion of the Design Document. This template will allow classmates (and you, the teacher!) to see an overview of the major strokes of the project at a glance: Who is the community that we are focusing on? What is the problem statement? What is the proposed solution using computer vision? What data might you need to gather to make your solution viable? What potential bias might exist in the data that you seek to collect?

🔁 **Circulate:** Encourage students to use their pre-existing work to fill out this outline.

> 🎙️ **Say:** Please place your “Idea Outline” document out so that other members of the class can circulate around and read it. You will be giving feedback to other groups using sticky notes. Don’t forget to bring something to write on, like a binder, book, or composition notebook.

☑️ **Do This:** Students will circulate around the room and give general feedback as to the high level direction of other groups’ projects. Instruct them to use one sticky note per idea that they share so that it becomes easier to sort and parse through the feedback.

🔁 **Circulate:** As the teacher, it would be helpful to model the process along with your students. Grab a stack of sticky notes and make comments on projects as well.

Teaching Tip: There are going to be two rounds of feedback in this activity. If you have multiple colors of sticky notes available for students, it would be a great idea to color-code the type of feedback that students are providing. For example, students can put things that they notice on yellow sticky notes, while posing their wonders / questions on blue sticky notes. This will help differentiate the types of feedback that different projects are receiving. Halfway through the activity, you can instruct students to pay attention to the predominant type of feedback that projects are receiving and to begin to provide the other type in order to achieve better balance.

A gallery walk is almost always more impactful and interesting if you treat the object of analysis like an actual piece of art in a gallery. This can be as simple as using tape and hanging the Idea Outlines on the wall, so that students can look at them in that fashion. If you have a quiet hallway nearby, you could also consider taking the activity outside of the classroom for more novelty and impact. At that point, it is highly recommended that it become a silent activity– all “talking” is done through the sticky notes!

☑️ **Do This:** Students will make another pass at projects, except this time they will be focusing on identifying possible sources of bias that might exist in student proposals. They can also provide suggestions for how to mitigate that bias.

🔁 **Circulate:** Again, engage with student projects and provide important checkpoint feedback for student groups.

Teaching Tip If you have a third color of sticky notes available, this activity would benefit from being differentiated by color as well. If you only have two colors of sticky notes available, consider just color-coding the feedback by round.

Assessment Opportunity: Formative As you make your way around the room to examine the different Idea Outlines, this would be a good time to see if students recognized the need for diverse and representative sources of data based on what sources they mention need to be collected.

> 🎙️ **Say:** You’ve come up with some impressive brainstorms regarding how you might address the problem statement that your group identified. Now that you have gotten some feedback from members of the class surrounding your design, our next steps will involve making some decisions about what solutions to focus on, and to begin to create a prototype that demonstrates a portion of our solution. That means that we are getting ready to transition from the Ideating phase of the Design Thinking Process into the Prototyping phase.

🎙️ Remarks: In the next class session, please come prepared with any media that you might need to train a sample model for your computer vision application. This can take the form of physical objects, images, video, sounds, music, etc. The more data that you bring, the better the model will likely perform. If the model does not perform as well as you thought it might, there will be opportunities during upcoming project time when you can make adjustments and tweaks to your model.

💬 **Discuss:** What physical objects, images, video, or other artifacts are you going to bring to class next to help train your model?

💡 **Discussion Goal:** This is a good time to make sure that students are clear that they will need to be responsible for bringing training data for their model in the next class period.

For example, if a student is making proposing an application that would help zookeepers know how many bananas a gorilla has eaten on a given day, then they would need to bring in a banana to train their model with– likely one that is undisturbed, and one that has been eaten and just the peel remains. Using this object, students could train a model to recognize both forms of banana, and could then use this model as a part of their application.

🖼️ Display: Lesson Objectives

🖼️ Display: Question of the Day

🖼️ Display: Key vocabulary
