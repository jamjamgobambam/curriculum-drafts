# Lesson 4: Patterns in the Noise

## Overview (Teacher)

**the question of the day**

In this lesson, students will begin with a case study of a computer vision product: the Roomba. Moving from the Empathizing to the Defining step of the Design Thinking process, students will learn some basic ways to visualize and interpret data, which they will use to define unique issues within the community for which they are designing their computer vision application.

## Overview (Students)

You will learn about another computer vision application in this lesson: the Roomba! Taking the research questions that you developed in the previous lesson, you will learn ways to interpret and visualize data in order to get a better idea about what is important to the members

{% tabs %}
{% tab title="Slides" %}
{% embed url="https://docs.google.com/presentation/d/1MUr8iBpV7m3p1TPpI6vgmGyHU1hWd2KuVsS-NOwHgaI/edit?usp=sharing" %}
{% endtab %}

{% tab title="Standards" %}
* CSTA: 2-DA-08: Collect data using computational tools and transform the data to make it more useful and reliable.
* CSTA: 3B-AP-20: Use project planning techniques to manage work, as a team member and in the development of complex artifacts.
{% endtab %}

{% tab title="Objectives" %}
* Explain ways in which computer vision aids the functionality of a Roomba
* Explore qualitative and quantitative data
* Visualize data using a histogram and scatterplot
* Cluster data to create thematic classifications


{% endtab %}

{% tab title="Preparation" %}
In order to prepare for this lesson, you will need access to the following materials:

* Large posterboard / butcher paper sheets (optional)
* Printed / Digital versions of all the resources below
{% endtab %}

{% tab title="Links" %}
For the teacher

* [Slides](https://docs.google.com/presentation/d/1MUr8iBpV7m3p1TPpI6vgmGyHU1hWd2KuVsS-NOwHgaI/edit?usp=sharing)

For the students

* Graphing Guide
  * [Printed](https://docs.google.com/document/d/1mMU60Mb3Jq7xe16lBohx0aAq4LXTBkTBfxpltreEhgU/edit#heading=h.ir5xxe6n135a)
  * [Digital](https://jamboard.google.com/d/1AczqRC5MvpUYcuYCtddF8JjhjpdqYBWlecMhXLC8CCw/viewer?f=0)
* Sample Dataset
  * [Printed - Quantitative](https://docs.google.com/document/d/1r8POugUCcp0-eN-1kLuHC8ImYOSZA2-uy6MVbYx3IpM/edit?usp=sharing)
  * [Printed - Qualitative](https://docs.google.com/document/d/1VSdat0oMExctnfJun\_dZlznqsV1n\_z2CHTX\_Z5oJF8o)&#x20;
  * [Digital](https://docs.google.com/spreadsheets/d/1yMLeTKjwj6\_TmLK\_amHL-RhAQ-rZGq6CGTWyB9e0QBs/edit?usp=sharing)
{% endtab %}

{% tab title="Vocabulary" %}
* **Qualitative Data**- A type of information that describes things using words rather than numbers.
* **Quantitative Data**- Information that you can count or measure with numbers
{% endtab %}
{% endtabs %}

## Warm Up (10 mins)

> :microphone2: _**Remarks**_
>
> Today, we’ll begin by examining a case study of computer vision in action by looking at the world’s smartest vacuum cleaner: the Roomba. Let’s start by examining what it is, what it does, and what unique design challenges its maker, iRobot, had to overcome to make the Roomba the forefront of robotic cleaning technologies.

🖼️ **Display:**  "Computer Vision Case Study - Roomba" slide

🖼️ **Display:**  "Computer Vision Case Study - Analysis" slide

💬 **Discuss:** _What might be some of the Roomba's **features** and **functions**?_

{% hint style="info" %}
**Teaching Tip**

For every computer vision case study (such as with Roombas), we will highlight on one of four analysis questions, which, when put together, provide a consistent framework for engaging with and exploring computer vision technologies and applications. Each of the warm-up activities during Week One of this module will focus on a different question.

\
By being able to look at a product or technology using this framework, we are helping train students to be critical consumers of technology, rather than passive adopters.
{% endhint %}

**Discussion Goal:** Some possible responses to these questions might be as follows:

* It vacuums dirt and debris; it can avoid obstacles and falls; it maps a house and uses computer vision to know where it is; it can return itself to the power station to charge; it can detect dirt.

🖼️ **Display:**  "Computer Vision Case Study - Empathize" slide

✅ **Do This:**  (2 _min_)  In a group of 3-4 students, ask the students to empathize with the daily dangers and challenges that might come with being a Roomba. Have them compile a list of these dangers and challenges and to be ready to share. Have them look at this through the lens of understanding, not necessarily solving the problems that they come up with. &#x20;

💬 **Discuss:** _What are some dangers or challenges that a Roomba might encounter as it tries to do its job?_

**Discussion Goal**: &#x20;

Students should come up with various dangers and challenges a Roomba might face. Examples include:&#x20;

* Obstacle navigation
* Avoiding damaging household items
* Stairs and drops
* Overzealous (and playful) pets
* Different types of surfaces
* Battery life
* Getting entangled / jammed
* Not leaving behind dirty “blind spots”

🖼️ **Display:** "Computer Vision Case Study - Our Solutions" slide

✅ **Do This:**  (2 _min_)  Have students return to their groups and select one of the dangers/challenges that they identified. Have the group brainstorm a possible solution. Mention to the groups that it is not necessary to come up with a detailed / technical solution– being able to describe what a solution might look generally like is ideal.

💬 **Discuss:** _What are some of the possible solutions that you came up with for your unique challenge?_

> :microphone2: _**Remarks**_
>
> Just like you did with your groups today, the designers at iRobot had to examine as many challenges and dangers to the Roomba as possible so that they could design a product that was able to meet and overcome them. Designing a product that can go into an uncertain situation and perform successfully is no easy task! There is a lot to consider.
>
> Let’s take a quick look at some of the technologies that the Roomba uses behind the scenes to overcome three very basic challenges.

✅ **Do This:** (1 min / slide) Go through the "Computer Vision Case Study - Lightning Knowledge 1-3" slides. The three slides detail a specific challenge that Roombas must overcome and its computer vision solution.&#x20;



## Activity (25 mins)

### Visualizing Quantitative Data (15 mins)

🖼️ **Display:** "The Design Thinking Process" slide

> :microphone2: _**Remarks**_
>
> We are on our way to designing a prototype for our very own computer vision application using the Design Thinking Process! Today marks the transition from the first step, Empathizing, to the second step, Defining. We have chosen a community that is important to us and brainstormed possible issues that might occur in that community. Now we are going to see if we can use data to help define what problem or issue is the most important to solve.\
>
>
> When we design, we must keep our users in mind. When using the Design Thinking Process, we avoid coming up with a cool idea first. In the real world, designing like this often means that even if a solution is good, that there might not be people who adopt the idea / buy the product since it is not ranked highly on their list of needs to be addressed.&#x20;
>
> \
> With Design Thinking, we will gather data in order to interrogate our potential users and to find out what is important to them. What issues exist that we might not know about? What actions do they frequently do that we might be able to make easier for them? What is important to them? Using data, we will help to define our users and seek to answer these questions so we can design a computer vision application that will have the greatest impact for them.

🖼️ **Display:** "Lesson Objectives" and "Question of the Day" slides

🖼️ **Display:** "What is Quantitative Data?" slide

✏️ **Vocabulary:**  _Quantitative Data_- Information that you can count or measure with numbers

🖼️ **Display:** "What are some Examples" slide

> :microphone2: _**Remarks**_
>
> Let's take a look at some specific ways that we can convert quantitative data into useful visualizations that can help our data to tell a story.

### Histograms

🖼️ **Display:** "Histograms" and "Histogram Discussion" slides

💬 **Discuss:** _Where might you have used histograms before? What kinds of data are especially useful when displayed in this manner?_

🖼️ **Display:** "Creating a Histogram" slides. &#x20;

{% hint style="info" %}
**Teaching Tip**

There are several animated slides that visually represent how to create different data visualizations throughout this lesson. Students might need to see the visualization a few times in order to understand. It might be useful to take questions and to clear any confusion while displaying these animations.
{% endhint %}

🖼️ **Display:** "Histogram Group Work" slide

✅ **Do This:** Put students in groups of 3-4 for the following activity:

Using the **sample dataset** and **graphing guide**, students will create an exemplar histogram. In the sample dataset there are three questions that have data. Have the students focus on question one for this exercise:&#x20;

* How do you feel about the overall cleanliness and maintenance of our school?

{% hint style="info" %}
**Teaching Tip**

There are two different ways to have students tackle this assignment– physical and digital– and there are resources for each to support your approach.



**Physical**: Print out the Sample Quantitative Responses dataset and the Graphing Guide. Have groups use the dataset to make marks on page 2 in the graphing guide using markers, pens, crayons, stamps, etc.

An alternative method might be to have students recreate the axes themselves on a large piece of poster / butcher paper as a means of having a larger artifact from this exercise that might hang in the classroom for students to refer to later as a resource.

\
**Digital**: There is a spreadsheet that contains all of the data for this exercise, as well as a link to a sample Google Jamboard that you might duplicate (other platforms which might work include Figma, Google Slides / Docs, etc.). Have students copy / paste the rectangles into the requisite columns to represent the data that is shown in the dataset.
{% endhint %}

🖼️ **Display:** "Histogram Group Work Analysis"&#x20;

✅ **Do This:**  Have students circle any data pattern that they see. They should annotate their graph by writing what they think this pattern represents.

🖼️ **Display:** "Histogram Peaks Discussion"&#x20;

💬 **Discuss:** _What do these two two peaks in the histogram potentially represent? Why might the data be clustered this way?_

**Discussion Goal:** Students will note that there are two distinct “peaks” in the data, centered around 1/2 and 8. They should note that it is not easy to see these patterns emerge until the data is graphed. It should be noted that since this data is so split that strong feelings exist on this topic which seem to run counter to one another. There is no clear consensus– such a finding could invite more research or further exploration.

### Scatterplots

🖼️ **Display:** "Scatterplot" and "Scatterplot Discussion" slides

💬 **Discuss:** _Where might you have used scatterplots before? What do the two axes represent in this case? How is this different than a histogram?_

**Discussion Goal:** Students should identify places they have seen these graphs– sports statistics, weather data, health and nutrition charts, for example. The two axes represent different the data from two unique questions. They are different from a histogram because they don’t measure value/frequency along the y-axis, but rather the value of another set of data.

🖼️ **Display:** "Creating a Scatterplot" slides  (_Talk through these steps and repeat if necessary_)

🖼️ **Display:** "Scatterplot Group Work" slide

✅ **Do This:**  Using the same sample dataset and graphing guide, students will create an exemplar scatterplot. In the sample dataset there are three questions that have data. Have the students focus on questions 1 and 2 for this exercise:&#x20;

* **X Axis**: How do you feel about the overall cleanliness and maintenance of our school?&#x20;
* **Y-Axis**: How likely are you to play a sport in school?

{% hint style="info" %}
**Teaching Tip**

As with above, there are two different ways to have students tackle this assignment– physical and digital.



**Physical**: Groups should use questions 1 and 2 from the Sample Quantitative Responses dataset and the Graphing Guide. Have groups use the dataset to make marks on page 3 of the graphing guide using markers, pens, crayons, stamps, etc.\
\
An alternative method might be to have students recreate the axes themselves on a large piece of poster / butcher paper as a means of having a larger artifact from this exercise that might hang in the classroom for students to refer to later as a resource.

\
**Digital**: There is a spreadsheet that contains all of the data for this exercise, as well as a link to a sample Google Jamboard that you might duplicate (other platforms which might work include Figma, Google Slides / Docs, etc.). Have students copy / paste the diamonds into the requisite rows/columns to represent the data that is shown in the dataset.
{% endhint %}

🖼️ **Display:** "Scatterplot Group Work Analysis" slide

✅ **Do This:** Have students circle any clusters of data points that emerged. Have them write on their graph what this circled cluster might represent.

🖼️ **Display:** "Scatterplot Cluster Discussion" slide

💬 **Discuss:** _Who / what might the three clusters potentially represent? Why might the data be clustered this way?_

**Discussion Goal:** There are three main clusters that emerge from the data. Those that are not active in school sports tend to have a polarizing view as to the cleanliness / maintenance of the school. However, there is greater polarization amongst students who are not as active in sports with distinct clusters falling on both sides of the spectrum. Why might students athletes have one opinion while those that don’t use the athletic facilities have two different points of view?

> :microphone2: _**Remarks**_
>
> We’ve now seen two different ways that we can take simple quantitative data and to visualize it to tell a story for us. Sometimes we’ve seen that the data leads to more questions than answers– and that can be a positive thing. It shows that we are getting to a core belief and understanding about the community that we are studying and may be on the cusp of an interesting finding that can help us to brainstorm and create a fantastic computer vision application for them!

### Visualizing Qualitative Data (10 mins)

> :microphone2: _**Remarks**_
>
> How do you graph words and thoughts? While not as neat and tidy as numbers can often be, text that we receive as answers to our research questions can also be organized and visualized so that we can extract meaning from them.

🖼️ **Display:** "What is Qualitative Data?" slide

✏️ **Vocabulary:**  _Qualitative Data_- a type of information that describes things using words rather than numbers

### Classification

🖼️ **Display:** "Classification" slide.

🖼️ **Display:** "What is Classification?" slide.  (_Talk through these steps and repeat if necessary_)

🖼️ **Display:** "Classification Group Work" slide.

✅ **Do This:**  Using your sample dataset, have students classify the data that they have received from question three:

* Describe one technology that helps you learn better.

{% hint style="info" %}
**Teaching Tip**

Again, there are two different ways to approach this task – both digital and physical.



**Physical**: Students can either use sticky notes or can cut out the pre-written data strips from the [Printed - Qualitative](https://docs.google.com/document/d/1VSdat0oMExctnfJun\_dZlznqsV1n\_z2CHTX\_Z5oJF8o) dataset available in the resources above. Using these manipulatives, students should create clusters of similar ideas, using a scrap piece of paper for writing out the descriptive titles of each cluster

\
**Digital**: Students can use a copy of the the pre-populated Jamboard to arrange their digital stickies into clusters. Use the text tool to give a descriptive title for each cluster.
{% endhint %}

🖼️ **Display:** "Classification Discussion" slide.

💬 **Discuss:** _What clusters developed from your analysis? Are these popular forms of learning technology that are already in use in schools?_

**Discussion Goal:** There will be two main clusters that should emerge from this exercise – learning facilitated by cellphone, and learning facilitated by social platforms (TikTok, FB, Discord, etc.) There will be other random groupings that might occur. Time permitting, allow groups to share some of their findings to see if anything novel emerges!

> :microphone2: _**Remarks**_
>
> Now we know a method for classifying and organizing data that involves words so that we might also find interesting patterns that might emerge from our audience. Now that we have this knowledge, we are ready to turn our attention from these examples to our own projects and put our knowledge to work by constructing a data visualization developed from our data.

## Project-Based Learning Time (10  mins)

### Visualizing Our Data

🖼️ **Display:** "PBL Group Work" slide

✅ **Do This:** With their group partner(s), students should analyze the data that they have gathered from your target  community. Students should create _**one**_ data visualization: histogram, scatterplot, or classification to aid in understanding their audience.

> :microphone2: _**Remarks**_
>
> Based on your learning experiences today with visualizing quantitative and qualitative data, it is time to turn our computer vision project. Today, you are going to take the data that you gathered from your own research questions and you will create one type of visualization-- a histogram, scatterplot, or classification.&#x20;

{% hint style="info" %}
**Teaching Tip**

If students have been unable to gather data for this assignment, there are several available datasets grouped by community that you can provide for them. Each one contains more data than should be analyzed. Have the groups focus on 2-3 quantitative and 1-2 qualitative sets of data.\
\
\*\* RESOURCE THAT NEEDS TO BE CREATED \*\*


{% endhint %}

🖼️ **Display:** "Three Ws" slide

💬 **Discuss:** _The Three Ws - What did we learn today? So what? Now what?_

🖼️ **Display:** "Revisit the Objectives" & "Revisit the Vocabulary" slide\
