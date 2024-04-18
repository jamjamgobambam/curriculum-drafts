# Lesson 8

## Warm Up (10 mins)

> 🎙️ **Say:** In the previous lesson, you developed an edge detection algorithm to isolate an object in an image. Once we have objects or other important things isolated within an image, how do we train a computer vision application to understand what these things are?

**Group:** Place students in pairs or small groups of 3.

📄 **Distribute:** Give each pair a set of the Classifying and Grouping Images.

☑️ **Do This:** Have students work with their partner to group, sort, and label a collection of images based on similarities that they see.

🔁 **Circulate:** As students work on finding their ideal groupings, tell them to create labels to organize their thinking. You should also encourage them to revise and reform groupings at any time. Reinforce to them that there is not one answer that you are looking for.

{% hint style="info" %}
**Teaching Tip**

The images were chosen purposefully, so that there are many different ways to group them. Students could group them based on objects that they see, locations, contexts, or even color palette. Often they will find that an image belongs in two of the categories that they created.
{% endhint %}

💬 **Discuss:** _What is the correct way to group the images?_

💡 **Discussion Goal:** Short answer - there is no correct way! It is important to point out that there are many different ways of grouping the images – it could be based on similar objects that are detected in the scene (e.g. cooking utensils), on location (e.g. inside of a school), on attributes (e.g. clean vs. dirty / color palette), or context (e.g. it must be lunch time!). An important takeaway is that while there are many ways to group, sort, and label images, the most important consideration is the purpose behind what you are grouping. If we want a dataset that will help a computer vision application to identify objects in a scene, for instance, then labeling and classifying by object type would be the ideal way to group these images.

Another important conversation thread that could emerge is that it is often difficult (if not impossible!) to sort the images based on a singular object. If you made two categories- books and tables- there are images that contain one or the other, but also images that contain both. Therefore, being able to tag multiple objects within an image becomes important.

> 🎙️ **Say:** Having access to datasets full of thousands or millions of images that are sorted and labelled with information is absolutely essential in being able to train a computer vision system to interpret the world around us.

## Activity (30 mins)

> 🎙️ **Say:** As we just experienced, it can be a lot of work to classify images sometimes. There are lots of different rules and patterns that you can use for how you choose to organize them. However, the act of ordering, sorting, and classifying the objects in images is essential in order to train computer vision applications to learn what they are seeing with their camera. Just like we need to learn to interpret the world around us through repeated use of our five senses, so too must a computer vision application train in order to make sense of what it sees in images.

☑️ **Do This:** Have students navigate to the COCO Dataset website. They should first read the purpose of the dataset, and should then navigate to the Explore section.

> 🎙️ **Say:** Take a few minutes to explore COCO and to see what it outputs when you click the various icons that are available in the Explore section.

☑️ **Do This:** Allow students several minutes to explore COCO. Encourage them to click around through the different icons and toggles and to run searches to see what comes up.

💬 **Discuss:** _What did you notice as you explored COCO?_

💡 **Discussion Goal:** Students will notice that the dataset made it very easy to search for one or more common objects that might be present in images. They might notice that the object(s) are color-coded as a segment within the larger image. They are able to hover over the various icons in the results in order to toggle which object segments they wish to view. Some students might have seen that there is a context toggle that they can select in the result images that will attempt to describe the scene in five different ways. This adds another layer of possibility with what is possible with COCOs and how it might be used to train computer vision applications.

🟡 Click the animation

💬 **Discuss:** _What do you wonder?_

💡 **Discussion Goal:** Student results will vary. They might wonder who made this dataset and how? What applications might it be useful in creating? Are there any other objects that it can detect?

{% hint style="info" %}
**Teaching Tip**

A great takeaway from this discussion might be that while COCO contains a lot of information and data about objects, it is limited to certain objects. This will show up in the next activity that students do, so this important consideration can be stressed at that point in time.
{% endhint %}

☑️ **Do This:** Introduce classes.

💻 **Transition:** Direct students to Level 1. Have students work with a shoulder partner to examine the image in order to see if they can identify classes that COCO would identify in this image.

☑️ **Do This:** Have students select the classes they see on COCO to see if they can find the image.

{% hint style="info" %}
**Teaching Tip**

Students will likely identify that the image contains a truck and people. However, when those terms are entered into COCO, there are 4151 possible images that fit that criteria! That is too much visual data to sort through. We will zoom out from this image to include more classes, which will speed up the process of finding the image.
{% endhint %}

☑️ **Do This:** Have students add in new possible classes that they see– a bench, skateboard, bag, and bowl.

{% hint style="info" %}
**Teaching Tip**

Once they enter in some additional classes, it should be easier to find the image. This highlights the highly indexed and searchable nature of COCOs, which makes it particularly useful for training computer vision models.
{% endhint %}

💬 **Discuss:** _How might an image dataset labeled with classes help a computer vision application?_

💡 **Discussion Goal:** Having a well-labeled dataset is crucial in being able to train computer vision models to accurately identify and classify the objects that it sees. However, as seen here with COCO, the classes that it is able to recognize are limited in scope. Oftentimes, there is a need to create and classify one’s own dataset for more niche computer vision applications and tasks.

☑️ **Do This:** Direct students to Level 2 to access MediaPipe's Object Detection model demo. Have students play around with the model by uploading a sample image.

🔁 **Circulate:** Encourage them to play around with the model. They will need to upload a sample image in order to have the model run and to detect possible objects. While they are exploring, suggest that they change the various options that are available within the model. However, have them focus on the score threshold. Challenge them to infer what it might be doing to the image.

💬 **Discuss:** _What did you notice as you played with the model? What do you wonder?_

💡 **Discussion Goal:** Answers will vary. However, a few important items to discuss include: The purpose of the score threshold. Students might figure out that it acts as a filter, and seems to get rid of results that are below a certain percentage. They will learn next that the percentage represents a confidence rating that the model has with its own guess. The higher the number, the higher its confidence that it is correct in inferring the object. The max results toggle. This allows the model to put more predictions on the screen at once. It will display the highest confidence objects first, and will include less confident responses as the slider value increases.

☑️ **Do This:** Explain the role of the confidence score.

{% hint style="info" %}
**Teaching Tip**

Being able to judge and rate its own performance at object detection is an important skill that computer vision models rely on to make important decisions. You can encourage students to consider confidence scores as part of their design for the computer vision application that they are developing. How might their application respond differently when there is different confidence scores? You might even frame it as an If-Else If-Else conditional statement.
{% endhint %}

> 🎙️ **Say:** We saw in the sample Lotus Blossom brainstorm that one problem that gardeners often deal with is pests. The designers behind this brainstorm want to know if this model would work well for an Auto-Pest Detection application.

> 🎙️ **Say:** We will now test the Object Detection model that was created using COCO on a variety of different images of common garden pests. This model is a proof of concept that their solution might be a good one to pursue.

☑️ **Do This:** Direct students to Level 3 to download the image files.

☑️ **Do This:** Have students select 2 to 3 images to upload to the tool. They can adjust the inference delegate, the model selection, the max results, and the score threshold attributes to see if they can have the model identify the insects.

💬 **Discuss:** _What were your results?_

💡 **Discussion Goal:** The student groups should have come to the sad conclusion that the object detection model was not successful in identifying the insects.

🟡 Click the animation

💬 **Discuss:** _Was this the outcome that you expected? Why or why not?_

💡 **Discussion Goal:** Some students may have recognized that amongst the 91 different classes that COCO is able to identify, insects are not among them. As such, since this model was trained using COCO, it will not be able to be used for an Auto-Pest Detection application. Emphasize the importance of having a dataset that is attuned to the purpose of the application in which you want to use it. A computer vision application is only as good as the data on which it is trained!

> 🎙️ **Say:** Let’s try a different model – Image Classification. As before, you do not need to upload and test all of the images. Select a few of them and run them through the model. Make sure to try different settings in order to see if you can maximize your results.

☑️ **Do This:** Direct students to Level 4 to access MediaPipe’s Image Classification model demo. Have students upload a few of the insect image files using this model.

💬 **Discuss:** _How did the results differ?_

💡 **Discussion Goal:** This model will have much higher success rates. That is because it is not trained using COCO. Point out that under the description of the Image Classification model that is says it is trained using ImageNet. This dataset has access to 1000 classes – a much greater amount of possibilities to train a computer vision model with!

💬 **Discuss:** _Were there any unexpected results or patterns?_

💡 **Discussion Goal:** Students notice that some of the insects are still misidentified (e.g. the caterpillar and the aphids). They might notice that the confidence scores that are displayed at the bottom are not near 100% even when the prediction is correct.

{% hint style="info" %}
**Teaching Tip**

Underscore the importance of choosing data that can support the type of model that you want to create. Encourage students to think about where this data comes from. If there is no existing dataset available, how does one train a unique and novel computer vision application?
{% endhint %}

☑️ **Do This:** Direct students to continue brainstorming ideas for their project.

## Wrap Up (5 mins)

💻 **Transition:** Direct student to Level 5 to complete their reflection questions on Levels 5, 6, and 7.

* _Can you explain how datasets like COCO and ImageNet are used in training computer vision models?_
* _What is a confidence score, and why is it important in the output of a computer vision model?_
* _Reflecting on today’s lesson, how do the suitability and characteristics of different datasets influence the design of computer vision applications?_

💡 **Reflection Goals:** Students should discuss the role of large image datasets in providing the labeled data necessary for training computer vision models to recognize and classify objects within images This question assesses students’ understanding of confidence scores as a measure of how certain a computer vision model is about its predictions, emphasizing its importance in determining the reliability of these predictions. To synthesize learning by having students articulate the critical role of selecting appropriate datasets in designing computer vision applications that can accurately perceive and interpret images.

{% hint style="success" %}
**Assessment Opportunity**

The responses in the levels can be used to formatively assess how well students have met the objectives of the lesson.
{% endhint %}
