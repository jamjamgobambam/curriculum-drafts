# Lesson 8

## Overview (Teacher)

**How does the quality and quantity of training data impact the performance of computer vision models?**

Students will learn the basics of training a computer vision model– including gathering / creating data, training the model, and evaluating the results. They will be using Teachable Machine to create a model that will be the first addition to the project prototype that they will be creating over the next several class sessions.

## Overview (Students)

You will be learning the basics of training a computer vision model– including gathering / creating data, training the model, and evaluating the results. We will be using Teachable Machine to create a model which will become the first addition to the project prototype that you and your group will be creating over the next several class sessions.



{% tabs %}
{% tab title="Slides" %}
{% embed url="https://docs.google.com/presentation/d/1mk85wn2sT6M5R7STRXHGL7q51bG3CZYW5XR5-N5YjEE/edit?usp=sharing" %}
{% endtab %}

{% tab title="Standards" %}
| CSTA: 3A-AP-16            | Design and iteratively develop computational artifacts for practical intent, personal expression, or to address a societal issue by using events to initiate instructions. |
| ------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| CSTA: 3A-AP-13            | Create prototypes that use algorithms to solve computational problems by leveraging prior student knowledge and personal interests.                                        |
| <p>AI4K12:<br>3-A-iii</p> | Training a model - Use either a supervised or unsupervised learning algorithm to train a model on real world data, then evaluate the results.                              |
{% endtab %}

{% tab title="Objectives" %}
* Explore how visual data is used within a machine learning algorithm to train and create a model
* Train, validate, and test basic AI classification systems in computer vision
* Create and evaluate prototypes that solve problems using computer vision
{% endtab %}

{% tab title="Preparation" %}
* Blank white paper will be needed for the warm-up. You can cut it into quarters in advance.
* Students should have the items needed to train their model (webcam / images / video / microphone, etc.)
* Verify that students have access to the [Teachable Machine website](http://teachablemachine.withgoogle.com) in order to train their models.
{% endtab %}

{% tab title="Links" %}
For the teachers

* [Model-Making Machine](https://docs.google.com/presentation/d/1mk85wn2sT6M5R7STRXHGL7q51bG3CZYW5XR5-N5YjEE/edit?usp=sharing)- Slides
* [Teachable Machine 2.0](https://youtu.be/T2qQGqZxkD0?feature=shared)- Video
* [Object Cards](https://docs.google.com/presentation/d/1vq99wxIkEBMhOt9h3QzDF35A6WWson3U3s7\_suZXoFQ/edit?usp=sharing) - Resources

For the students

* [Teachable Machine 2.0](https://youtu.be/T2qQGqZxkD0?feature=shared)- Video
* [Teachable Machine](http://teachablemachine.withgoogle.com) - Website
{% endtab %}

{% tab title="Vocabulary" %}
model - programs that detect specific patterns using a collection of data sets
{% endtab %}
{% endtabs %}



🎙Remarks In the previous class, you developed an algorithm that helps a computer vision application be able to isolate an object in an image through the use of an edge detection algorithm. Once we have objects or other important things isolated within an image, how do we train a computer vision application to understand what these things are?

✅ **Do This:** With a partner, students will group, sort, and label a collection of images based on similarities that you see.

📄 **Distribute:** Physical - sticky notes for making labels and a copy of the images to cut out. Digital - a Google Slide that contains the images, shapes for labels, and blank slides for workspaces

🔁 **Circulate:** As students work on finding their ideal groupings, tell them to create labels to organize their thinking. You should also encourage them to revise and reform groupings at any time. Reinforce to them that there is not one answer that you are looking for.

Teaching Tip The images were chosen purposefully, so that there are many different ways to group them. Students could group them based on objects that they see, locations, contexts, or even color palette. Often they will find that an image belongs in two of the categories that they created. In the digital version of this warm-up, students might simply copy-paste an image into multiple categories; however, those with a physical version would have to make a determination as to which category something belongs in. This should lead to some interesting and enlightening conversations at the tail end of this warm-up.

💬 **Discuss:** What is the correct way to group the images together?

**Discussion Goal:** Short answer - there is no correct way! It is important to point out that there are many different ways of grouping the images – it could be based on similar objects that are detected in the scene (e.g. cooking utensils), on location (e.g. inside of a school), on attributes (e.g. clean vs. dirty / color palette), or context (e.g. it must be lunch time!). An important takeaway is that while there are many ways to group, sort, and label images, the most important consideration is the purpose behind what you are grouping. If we want a dataset that will help a computer vision application to identify objects in a scene, for instance, then labeling and classifying by object type would be the ideal way to group these images.

Another important conversation thread that could emerge is that it is often difficult (if not impossible!) to sort the images based on a singular object. If you made two categories- books and tables- there are images that contain one or the other, but also images that contain both. Therefore, being able to tag multiple objects within an image becomes important.

🎙Remarks Having access to datasets full of thousands or millions of images that are sorted and labelled with information is absolutely essential in being able to train a computer vision system to interpret the world around us.

🖼️ Display: Lesson Objectives

🖼️ Display: Question of the Day - How can datasets of images help a computer vision application to interpret what it sees?

🎙Remarks As we just experienced, it can be a lot of work to classify images sometimes. There are lots of different rules and patterns that you can use for how you choose to organize them. However, the act of ordering, sorting, and classifying the objects in images is essential in order to train computer vision applications to learn what they are seeing with their camera. Just like we need to learn to interpret the world around us through repeated use of our five senses, so too must a computer vision application train in order to make sense of what it sees in images.

✅ **Do This:** Have students navigate to the COCOs Dataset website. They should first read the purpose of the dataset, and should then navigate to the Explore section.

🎙Remarks Take a few minutes to explore COCOs and to see what it outputs when you click the various icons that are available in the Explore section.

✅ **Do This:** Allow students several minutes to explore COCOs. Encourage them to click around through the different icons / toggles and to run searches to see what materializes.

💬 **Discuss:** What did you notice as you explored COCOs?

**Discussion Goal:** Students will notice that the dataset made it very easy to search for one or more common objects that might be present in images. They might notice that the object(s) are color-coded as a segment within the larger image. They are able to hover over the various icons in the results in order to toggle which object segments they wish to view. Some students might have seen that there is a context toggle that they can select in the result images that will attempt to describe the scene in five different ways. This adds another layer of possibility with what is possible with COCOs and how it might be used to train computer vision applications.

💬 **Discuss:** What do you wonder?

**Discussion Goal:** Student results will vary. They might wonder who made this dataset and how? What applications might it be useful in creating? Are there any other objects that it can detect?

Teaching Tip A great takeaway from this discussion might be that while COCOs contains a lot of information and data about objects, it is limited to certain objects. This will show up in the next activity that students do, so this important consideration can be stressed at that point in time.

🖼️ Display & Read: COCOs allows the user to search images based on 91 pre-identified classes, or output categories.

✏️ **Vocabulary:** Class: The output category of one’s data

Teaching Tip The vocabulary word class will be used in a later lesson involving Teachable Machine. You might tell students that this term will come up again shortly. A mnemonic device that could be used to help them remember the term might be to equate class with classification – i.e. classes are based on a classification of an object.

🎙Remarks Let’s see if we can deconstruct how COCOs might view an image. Take a look at the image here and discuss with a shoulder partner what classes COCOs might identify. Then, head to the dataset, enter those classes, and see if you can find the image.

✅ **Do This:** Have students work with a shoulder partner to examine the image in order to see if they can identify classes that COCOs would identify in this image.

✅ **Do This:** Have students select the classes they see on COCOs in order to see if they can find the image

(HOST image on a level)

Teaching Tip Students will likely identify that the image contains a truck and people. However, when those terms are entered into COCOs, there are 4151 possible images that fit that criteria! That is too much visual data to sort through. We will zoom out from this image to include more classes, which will speed up the process of finding the image.

🎙Remarks More of the image has been revealed now. Can you identify more classes and does that help with being able to find the image on COCOs?

✅ **Do This:** Have students add in new possible classes that they see– a bench, skateboard, bag, and bowl.

Teaching Tip Once they enter in some additional classes, it should be easier to find the image. This highlights the highly indexed and searchable nature of COCOs, which makes it particularly useful for training computer vision models.

💬 **Discuss:** How might an image dataset with classes identified help a computer vision application?

**Discussion Goal:** Having a well-labeled dataset is crucial in being abled to train computer vision models to accurately identify and classify the objects that it sees. However, as seen here with COCOs, the classes that it is able to recognize are limited in scope. Oftentimes, there is a need to create and classify one’s own dataset for more niche computer vision applications and tasks.

🎙Remarks Let’s take a look at a real-world model that was actually trained using information gathered from the COCOs dataset.

✅ **Do This:** Have students select the MediaPipe Object Detection choice level.

🔁 **Circulate:** Encourage them to play around with the model. They will need to upload a sample image in order to have the model run and to detect possible objects. While they are exploring, suggest that they change the various options that are available within the model. However, have them focus on score threshold. Challenge them to infer what it might be doing to the image.

(Create choice level with links to landing pages for the MediaPipe demos)

💬 **Discuss:** What did you notice as you played with the model? What do you wonder?

**Discussion Goal:** Answers will vary. However, a few important items to discuss include: The purpose of the score threshold. Students might figure out that it acts as a filter, and seems to get rid of results that are below a certain percentage. They will learn next that the percentage represents a confidence rating that the model has with its own guess. The higher the number, the higher its confidence that it is correct in inferring the object. The max results toggle. This allows the model to put more predictions on the screen at once. It will display the highest confidence objects first, and will include less confident responses as the slider value increases.

🖼️ Display: When a computer model makes a prediction, it also provides a measure of the confidence it has in that prediction, usually reported as a percentage. This percentage is often called a confidence score.

Teaching Tip Being able to judge and rate its own performance at object detection is an important skill that computer vision models rely on to make important decisions. You can encourage students to consider confidence scores as part of their design for the computer vision application that they are developing. How might their application respond differently when there is different confidence scores? You might even frame it as an If-Else If-Else conditional statement.

🖼️ Display: We saw in the sample Lotus Blossom brainstorm that one problem that gardeners often deal with is pests. The designers behind this brainstorm want to know if this model would work well for an Auto-Pest Detection application.

Teaching Tip This Lotus Blossom brainstorming sample was first seen in the PBL section of Lesson 6’s slide deck. The community of focus was “gardeners”. The problem statement identified was “Gardeners always mention a lack of time, and wish for a smart solution to know how to best tend to their crop”. \[LINK]

🎙Remarks We will now test the Object Detection model that was created using COCOs on a variety of different images of common garden pests. This model is a proof of concept that their solution might be a good one to pursue.

📄 **Distribute:** Have students download the garden\_images.zip file and unzip the contents. Possibility two

🎙Remarks You do not need to upload and test all of the images. Select a few of them and run them through the model. Make sure to try different settings in order to see if you can maximize your results.

✅ **Do This:** Have students select 2 to 3 images to upload to the tool. They can adjust the inference delegate, the model selection, the max results, and the score threshold attributes to see if they can have the model identify the insects.

💬 **Discuss:** What were your results?

**Discussion Goal:** The student groups should have come to the sad conclusion that the object detection model was not successful in identifying the insects.

💬 **Discuss:** Was this the outcome that you expected? Why or why not?

**Discussion Goal:** Some students may have recognized that amongst the 91 different classes that COCOs is able to identify, insects are not among them. As such, since this model was trained using COCOs, it will not be able to be used for an Auto-Pest Detection application. Emphasize the importance of having a dataset that is attuned to the purpose of the application in which you want to use it. A computer vision application is only as good as the data on which it is trained!

🎙Remarks Let’s try a different model – Image Classification. As before, you do not need to upload and test all of the images. Select a few of them and run them through the model. Make sure to try different settings in order to see if you can maximize your results.

✅ **Do This:** Go to MediaPipe’s Image Classification model demo, and upload a few of the insect image files using this model

💬 **Discuss:** How did the results differ?

**Discussion Goal:** This model will have much higher success rates. That is because it is not trained using COCOs. Point out that under the description of the Image Classification model that is says it is trained using ImageNet. This dataset has access to 1000 classes – a much greater amount of possibilities to train a computer vision model with!

💬 **Discuss:** Were there any unexpected results or patterns that you indentified?

**Discussion Goal:** Students notice that some of the insects are still misidentified (e.g. the caterpillar and the aphids). They might notice that the confidence scores that are displayed at the bottom are not near 100% even when the prediction is correct.

Teaching Tip Underscore the importance of choosing data that can support the type of model that you want to create. Encourage students to think about where this data comes from. If there is no existing dataset available, how does one train a unique and novel computer vision application?

🎙Remarks We are continuing our work from yesterday with the Ideate Stage from the Design Thinking Process. As you brainstorm today, discuss if which of the models that you explored today might be a good choice to use in your proposed application. There are also several other models that are available on MediaPipe that you can explore through the choice levels.

📄 Resource: The Lotus Blossom brainstorming document. Students can also work on it digitally, or create their own version of it on a blank sheet of paper.

Teaching Tip This is day 3 of 3 for the Ideate Phase of the PBL work days. Students should aim to finish up their brainstorming, to add specific details to their proposed solutions by linking it to a model, and to decide which of the possible solutions that they might want to pursue as they transition from the Ideate phase to the Prototype phase of the Design Thinking Process.

🖼️ Display: Learning Objectives

🖼️ Display: Question of the Day

🖼️ Display: Key Vocabulary
