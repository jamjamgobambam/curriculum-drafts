# Lesson 4

## Overview (Teacher)

**How can datasets of images help a computer vision application to interpret what it sees?**

In this lesson, students will move from learning how an image is extracted from an image to how computer vision systems are then able to take that information and process it. They will be introduced to the COCOs and ImageNet image datasets which are used to train computer vision applications. Students will experiment with sample models built from both datasets in order to learn about confidence scores and how they play an important role in determining the accuracy of a model.

## Overview (Students)

In this lesson, you will explore how computer vision applications learn to perceive the objects that are extracted from images through algorithms like edge detection. You will explore various image datasets which are used to train computer vision applications. Experimenting with sample models built from image datasets, you will learn about confidence scores and how they play an important role in determining the accuracy of what a computer vision system perceives.



{% tabs %}
{% tab title="Slides" %}
{% embed url="https://docs.google.com/presentation/d/1p3n3e1nxMxby7TVJeD4tvCUtIwr67lt3bH7kPH7Spag/edit#slide=id.g26b38d373c3_0_94" %}
{% endtab %}

{% tab title="Standards" %}
| CSTA: 3A-AP-16                   | Design and iteratively develop computational artifacts for practical intent, personal expression, or to address a societal issue by using events to initiate instructions |
| -------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <p>AI4K12 </p><p>3-C-i.9-12 </p> | Compare two real world datasets in terms of the features they comprise and how those features are encoded.                                                                |
| AI4K12 3-A-iii.3-5               | Train a classification model using machine learning, and then examine the accuracy of the model on new inputs                                                             |
{% endtab %}

{% tab title="Objectives" %}
Students will be able to:

* Evaluate the suitability and characteristics of different datasets
* Explain the importance of using confidence ratings
* Explore how databases of processed images might be used within your project designs
{% endtab %}

{% tab title="Preparation" %}
* Print the Classifying and Grouping Images document ahead of time if you will be using the physical version. Students will need access to scissors to cut out the images.
* Preview the MediaPipe models presented (Object Detection /&#x20;
* Make sure that students are able to download / unzip the images for the main activity.
{% endtab %}

{% tab title="Links" %}
For the teachers

* [From Pixels to Perception](https://docs.google.com/presentation/d/1p3n3e1nxMxby7TVJeD4tvCUtIwr67lt3bH7kPH7Spag/edit#slide=id.g26b38d373c3\_0\_94)- Slides
* [Classifying and Grouping Images](https://docs.google.com/presentation/d/1kpCbq5itHPSJILXZYqexTeeA4vYQjj\_fZ4L1YwJzLEA/edit#slide=id.p) - Physical Activity&#x20;
* [garden\_images.zip](https://drive.google.com/file/d/1ScSCuXN75ltGUZzMKze1\_LTR5PMrM-Ax/view?usp=drive\_link) - Resource

For the students

* [Classifying and Grouping Images](https://docs.google.com/presentation/d/1kpCbq5itHPSJILXZYqexTeeA4vYQjj\_fZ4L1YwJzLEA/edit#slide=id.p) - Physical Activity&#x20;
* [Classifying and Grouping Images](https://docs.google.com/presentation/d/1n3dBJJI0T26X-56bSOBlL3hjvWTxbxYDYPUsj5Bdb-s/edit#slide=id.p) - Digital Activity
* [garden\_images.zip](https://drive.google.com/file/d/1ScSCuXN75ltGUZzMKze1\_LTR5PMrM-Ax/view?usp=drive\_link) - Resource
* Lotus Blossum Brainstorm ([Digital](https://docs.google.com/presentation/d/1PqPXAGgH6sgDSVK9B-Haj2aiprI3FOhag9M1ARfLtv8/edit?usp=sharing) / [Physical](https://drive.google.com/file/d/1gI4dvD77yQL2gr7SAvTIT81BJeN0O-WB/view))- Resource
{% endtab %}

{% tab title="Vocabulary" %}
* Class - the output category of one’s data
* Confidence score - A percentage that represents a measure of the confidence that a model has in its prediction
{% endtab %}
{% endtabs %}

> 🎙️ **Say:** Today, we’ll begin by examining a case study of computer vision in action by looking at “smart” robo-vacuum cleaners. Let’s start by examining the unique design challenges their designers had to overcome to make create these robotic cleaning technologies. We’ll also examine how data might be used to make informed decisions about possible solutions.

☑️ **Do This:** Read the slide / Get a volunteer to read

> 🎙️ **Say:** When we evaluate computer vision technologies, we can ask ourselves these four important questions in order to analyze the technology’s impact.

Today, let’s focus in on the following question: What are a robo-vacuum’s features and functions?

Teaching Tip: Our Case Study Analysis Framework For every computer vision case study (such as with robo-vacuums), we will highlight on one of four analysis questions, which when put together, provide a consistent framework for engaging with and exploring computer vision technologies and applications. Each of the warm-up activities during Week One of this module will focus on a different analysis question.

By being able to look at a product or technology using this framework, we are helping train students to be critical consumers of technology, rather than passive adopters.

☑️ **Do This:** Read the slide / Get a volunteer to read

💬 **Discuss:** What insight does this graph offer about robo-vacuum users?

💡 **Discussion Goal:** The histogram clearly shows that a majority of robo-vacuum users are very concerned that their expensive cleaning product will tumble down the stairs. Gathering and visualizing data in this way can very quickly point out important areas of focus when designing products. There is an opportunity to make an inference about the second largest bar in the graph which indicates folks that are not concerned about it. You might want to prompt students and ask why people might not be worried (they live in an apartment with one floor, for instance). This will connect to the idea of creating User Personas which will be the focus of the next lesson.

🟡 Click the animation

💬 **Discuss:** What feature / function might help address this need?

💡 **Discussion Goal:** Here students can speculate as to how robo-vacuums might overcome this challenge. A main point is that there needs to be a camera or other sensor built into the machine that can identify and avoid areas where there is a sudden drop. Ideally, this should be something that the robot can determine on its own, rather than having to have users erect barriers or use other means to discourage the robot from tipping over the edge.

> 🎙️ **Say:** We have already identified that falling down the stairs might be a danger both for the robot and for the owner’s wallet. Let’s take a moment to empathize with the robo-vacuum itself– what challenges and dangers does it have to overcome on a daily basis in order to do its job well?

☑️ **Do This:** Have students work together with a partner to quickly brainstorm some obvious dangers or challenges that a robo-vacuum might face as it attempts to clean.

🔁 **Circulate:** Help students ideate if they appear stuck. Possible responses to help prompt groups might include:

Obstacle navigation Avoiding damaging household items Stairs and drops Overzealous (and playful) pets Different types of surfaces Battery life Getting entangled / jammed Not leaving behind dirty “blind spots”

> 🎙️ **Say:** Choose one of the challenges or dangers that you identified. Now, with your partner, brainstorm what features or functions can be added to the robo-vacuum in order to overcome this problem.

☑️ **Do This:** Have students select one of the dangers/challenges that they identified. Have them brainstorm a possible solution. Mention to the groups that it is not necessary to come up with a detailed / technical solution– being able to describe what a general solution might look like ideal.

💬 **Discuss:** Have willing groups share one of their problem / solution combinations.

> 🎙️ **Say:** Just like you did with your groups today, the designers of robo-vacuums had to examine as many challenges and dangers to the product as possible so that they could design a product that was able to meet and overcome them. Gathering data from users and from testing was essential to know how to create the best possible product.

☑️ **Do This:** Read lesson objectives with class

☑️ **Do This:** Read Question of the Day with class

> 🎙️ **Say:** We are on our way to designing a prototype for our very own computer vision application using the Design Thinking Process! Today marks the end of the first step, Empathizing. In that step, we chose a community that is important to us and brainstormed possible issues that affect them.

🟡 Click the animation

> 🎙️ **Say:** Now we are moving onto Defining. In this step, we are going to see if we can use data to help define what problem or issue is the most important to solve.

The focus of today’s lesson will be to explore how you might take data and represent it visually. Many times, visualizing data is necessary in order to see patterns that might not be obvious otherwise. From these visualizations and patterns, solid decisions can be made that keep a user’s needs in focus.

📄 **Distribute:** Students should have access to the Lesson 4 Sample Dataset, available under the Links category within the lesson. They should also have a digital copy of the Our Data Visualizations activity guide.

> 🎙️ **Say:** As you access the sample dataset and activity guide to be used in our first activity, select File > Make a Copy so that you have access to the material in your own account.

🔁 **Circulate:** Assist any students who might need help creating a copy of the dataset and/or Our Data Visualizations activity guide.

Teaching Tip: Title It might be useful to “deputize” several students to assist with the task of making a copy of the data / activity guide in case there are large numbers of students who need assistance with the task.

> 🎙️ **Say:** Today will be an exploration of what is possible using Google Sheets to help us create data visualizations. You and your partner are encouraged to experiment with different ways to visualize some of the data that is represented in the sample dataset.

There are two resource links that are available that can help explain some of the basic ways to visualize data. Use them as a resource if you desire, or simply experiment with the data on your own.

🟡 Click the animation

> 🎙️ **Say:** The Graphs and Charts page provides explanations and examples of charts and graphs that you can use in Google Sheets. The “from Data to Viz” website explains what types of visualizations work best with the type of data that you have. Feel free to use them as possible resources, or explore on your own.

> 🎙️ **Say:** Go ahead and let’s see what you can create. Try as many combinations as you can in the time that we have. The first step to creating a visualization will be to click the Insert menu and select Chart.

Use your “Our Data Visualizations” activity guide in order to document your exploration. Feel free to include visualizations that you like and those that you do not like. There is space to reflect on what worked and what didn’t seem to work within the activity guide.

☑️ **Do This:** Have students work through creating visualizations using the sample data provided within Google Sheets. Document the visualizations using activity guide.

🔁 **Circulate:** As you move through the classroom helping students, use the following tips to assist students in need: Select the data cells that you want to visualize by mousing over them with the left mouse button down. Histograms and line graphs are often the easiest visualizations to create for students. Introduce the Customize menu in the Chart Editor – this allows them to have better control over the labels, looks, and presentation of their data. Encourage the students to try different chart types within the Editor, seeing which one best fits their data. Creating visualizations for qualitative data in Sheets is difficult! Ways that students could overcome this challenge would be to look at the most important words in the data and to keep track of the frequency with which these words appear. With the data presented in that fashion, a histogram could be created that would highlight the most used terms, and thus, indicate what might be most important to users. \[Advanced] Formulas such as =SUM() and =AVERAGE() can be used to aggregate data.

Teaching Tip: Sharing is Caring As you find interesting visualizations while circulating, it might be helpful to take a moment to highlight a few students’ work to share with the class what have created and the kinds of conclusions/insights/inferences that have drawn.

Teaching Tip: The Inquiry Method The inquiry method is a way of learning by asking questions to explore and understand topics deeply. When students use this method to analyze data visualizations, they start might by asking: what patterns do we see? What story does the data tell? This approach encourages curiosity, leads to meaningful discoveries, and helps students use their visualizations to reveal insightful answers, or even new questions to ask!

.

> 🎙️ **Say:** Now that you’ve created your visualizations and did an initial analysis of the visualization, let’s compare with another group.

☑️ **Do This:** Have each student group join one other group. They should walk through one of the visualizations that they created and documented in their activity guide. They should use the conversation with their peers as an opportunity to revise their work, add detail, or formulate new questions that arise.

🔁 **Circulate:** As the groups work together, use this as an opportunity to get a quick pulse check on common issues and successes that the groups encountered. These can be useful to prime conversation in the whole class discussion that will be held at the end of this activity.

💬 **Discuss:** What types of visualizations worked best for the data we explored? Why?

💡 **Discussion Goal:** Students likely found that histograms, bar charts, pie charts and line charts were the best types of visualizations to use when just looking at the data for one question. These visualizations showed clear peaks and valleys which can then be used when a group is making a observation/question/inference. For examining multiple columns of data, a scatter plot might have been the most appropriate. Students will see that there are clusters of points that appear on the scatter plot that might indicate different types of users and needs.

🟡 Click the animation

💬 **Discuss:** What data was most difficult to visualize? Were you able to find a way to overcome that challenge?

💡 **Discussion Goal:** Using Google Sheets, visualizing the qualitative data would most likely be the most difficult. If students use scatter plots, they may also find the way that the data is presented to be difficult to work with. Underscore the importance of productive struggle here – emphasizing that not everything that we do will yield results. It is through the process of exploration and experimentation that we, over time, can refine our visualizations.

Enrichment: Pose a series of data visualization challenges that come directly from your students’ struggles with visualizing difficult-to-graph data.

> 🎙️ **Say:** Now that we have had some experience with creating basic data visualizations, let’s turn our attention to our own data that we gathered in our surveys. Let’s use the techniques that we experimented with in Google Sheets in order to create a visualization that offers an insight about what is important target community/audience.

☑️ **Do This:** With their group partner(s), students should analyze the data that they gathered from their target community. Students should create at least one data visualization to aid in understanding their audience’s needs better.

🔁 **Circulate:** Assist students with formatting their data into columns, if necessary. If the students used Google Forms, they can export their results as a spreadsheet with columns directly into Google Sheets. Encourage them to experiment with different types of visualizations in order to create a visualization that they can then use to make an observation, ask a question, or draw an inference.

Teaching Tip: Types of Visualizations The easiest graphs to work with inside of Google Sheets for the type of data that students have likely gathered includes: Bar Graphs / Histograms Line Graphs / Area Charts Pie Charts Scatter Plots

> 🎙️ **Say:** Now that you’ve created a visualization of your data, let’s analyze our visualization by writing out one observation, question, or inference that you can make about the data

☑️ **Do This:** Have students navigate to Lesson 4, Level 1 and write their answer in the Free-Response box available there.

Assessment Opportunity: Formative Assessment Review the different analyses that students performed on their data in order to know which groups might need more assistance at the next stage of project development, in which they will be taking this observation / question / inference and turning it into a user persona that attempts to define the type of user that might use their product, and what problem they have that might be potentially solved with a computer vision application.

> 🎙️ **Say:** We will be using the visualization(s) that you created today in order to create user personas that will help describe the greatest needs of members of our target community.

> 🎙️ **Say:** Review Lesson Objectives

> 🎙️ **Say:** Review Question of the Day

> 🎙️ **Say:** Review key vocabulary
