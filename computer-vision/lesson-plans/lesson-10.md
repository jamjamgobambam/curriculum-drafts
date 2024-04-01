# Lesson 10

## Overview (Teacher)

**the question of the day**

Summary of what is in this lesson (2-3 sentences). How does this fit into the big picture \[optional] (2-3 sentences)?

## Overview (Students)

A student-friendly version of the text above. Speak directly to the students.

{% tabs %}
{% tab title="Slides" %}
(embed the slide deck for the lesson here)
{% endtab %}
{% endtabs %}

🎙️ Remarks: Before we start testing and training our models today, we’re first going to warm up our creative skills and give us a firsthand look at the challenges and considerations involved in training a computer vision model.

🎙️ Remarks: Imagine you are trying to teach a friend to recognize something they’ve never seen before. But, there’s a catch - you can only use images! This is similar to how we can train machine learning models in computer vision.

🟡 Click the animation

🎙️ Remarks: We provide them with examples, or “training data”, to help them learn.

🟡 Click the animation

🎙️ Remarks: As you can see in these images, the same subject can be represented in various ways depending on our viewpoint. Each perspective offers unique information about the subject.

🎙️ Remarks: These drawings range from a frontal view to a side view, and back perspectives. We could have even had a top-down view or a zoomed in view as well. Notice how each view captures different details? Think about why this diversity in data would be crucial for training algorithms to recognize objects.

🎙️ Remarks: It is now your turn to train your classmates! When you get your object card, make sure you do NOT show anyone! Keep this a secret!

☑️ **Do This:** Place students into groups of 3-4.

📄 **Distribute:** Give each student one of the compound object cards.

☑️ **Do This:** Direct students to take out a blank piece of paper and fold the paper into quarters, then separate the paper into four pieces.

☑️ **Do This:** Instruct students to draw their object on their card from the fourth and final perspective. Again, this can be whichever perspective they wish.

🔁 **Circulate:** As you walk around the room, remind students that their goal with each drawing is to try to capture the essence of the object in a way that others can recognize, despite not having it labeled.

Teaching Tip: Timing If the music in the provided timer is too distrracting for your students, you may wish to mute the audio by right clicking on the video and selecting “Format Options”. If you have the time, you can also give students more than 30 seconds, however, to keep the activity progressing, it is suggested not to give them longer than 1 minute for each drawing.

☑️ **Do This:** Instruct students to draw their object on their card from the first perspective. This can be whichever perspective they wish.

🔁 **Circulate:** As you walk around the room, remind students that their goal with each drawing is to try to capture the essence of the object in a way that others can recognize, despite not having it labeled.

Teaching Tip: Timing If the music in the provided timer is too distracting for your students, you may wish to mute the audio by right clicking on the video and selecting “Format Options”. If you have the time, you can also give students more than 30 seconds, however, to keep the activity progressing, it is suggested not to give them longer than 1 minute for each drawing.

☑️ **Do This:** Instruct students to draw their object on their card from the second perspective. Again, this can be whichever perspective they wish.

🔁 **Circulate:** As you walk around the room, remind students that their goal with each drawing is to try to capture the essence of the object in a way that others can recognize, despite not having it labeled.

Teaching Tip: Timing If the music in the provided timer is too distrracting for your students, you may wish to mute the audio by right clicking on the video and selecting “Format Options”. If you have the time, you can also give students more than 30 seconds, however, to keep the activity progressing, it is suggested not to give them longer than 1 minute for each drawing.

☑️ **Do This:** Instruct students to draw their object on their card from the third perspective. Again, this can be whichever perspective they wish.

🔁 **Circulate:** As you walk around the room, remind students that their goal with each drawing is to try to capture the essence of the object in a way that others can recognize, despite not having it labeled.

Teaching Tip: Timing If the music in the provided timer is too distrracting for your students, you may wish to mute the audio by right clicking on the video and selecting “Format Options”. If you have the time, you can also give students more than 30 seconds, however, to keep the activity progressing, it is suggested not to give them longer than 1 minute for each drawing.

☑️ **Do This:** Instruct students to separate their drawings so that each one is on its own piece of paper (if they haven’t done so already).

🟡 Click the animation

☑️ **Do This:** Students should then number their drawings with “1” being the least accurate or detailed and “4” being the most accurate or detailed.

☑️ **Do This:** Instruct students to take turns presenting their drawings to the other group members. Ensure students show one drawing at a time, starting with the one they think is the least accurate or detailed. After each drawing is shown, the other group members will make educated guesses about what the drawing is attempting to convey.

Teaching Tip: Extension If you have time, you can have students track guesses using tick marks to represent how many times various objects are guessed for each object model in order to simulate how confidence ratings might work. For example, group members keep track of every time someone guesses “girl” or “ice cream” or “dress” throughout the four different drawings.

💬 **Discuss:** How does this activity relate to how an AI model might be trained?

💡 **Discussion Goal:** Just as diverse perspectives in drawings help students guess the object more accurately, diverse training data helps AI models improve their recognition capabilities across different conditions and contexts. In addition, while this was not an exercise in drawing ability, the quality and the level of accuracy and detail in the drawings potentially affected the guessing process. This is similar to how detailed and accurate data can significantly enhance an AI model's learning accuracy and its ability to make correct identifications or predictions

🟡 Click the animation

💬 **Discuss:** Why might it be important to see objects in multiple contexts? How might this assist with training an AI?

💡 **Discussion Goal:** The goal is to further illuminate the critical need for AI systems to encounter objects in varied contexts for robust recognition and understanding. The question aims to drive home the point that exposing AI to multiple contexts enhances its ability to generalize across different scenarios, making it more effective in real-world applications. In essence, diversity in data is crucial for training algorithms to recognize objects in real-world situations, where conditions and angles can vary greatly.

🎙️ Remarks: By engaging in this warm-up, you stepped into the shoes of a computer vision scientist. You saw firsthand the challenges they face in training models to accurately recognize and understand the world. And guess what? This is now exactly what you'll be doing with Teachable Machine. You'll be training your own computer vision models, applying what you've learned from this activity!

🖼️ Display: Consider having student volunteers read the bulleted objectives

🖼️ Display: Consider having a student volunteer read the Question of the Day

> 🎙️ **Say:** We will be moving from Ideating …

🟡 Click the animation

> 🎙️ **Say:** … to Prototyping today as we work with making models in Teachable Machine.

As you ideated with your group members, you came up with lots of impressive ideas. Prototyping involves taking the most promising of these ideas and making something tangible with it. We will not be creating a whole product, rather we will be creating parts of it so that it can be tested with our users. Prototypes are intended to be quick representations of what our ideas can look like – they are not perfected final versions. The more ideas that we have and which we are able to incorporate into our prototype, the better data our testing will give at the end of the process.

☑️ **Do This:** Have students navigate to the Teachable Machine website. They should click the “Get Started” button.

Teaching Tip: Teachable Machine Link To ease the process of finding the correct website, it might be helpful to provide students with a hyperlink in your LMS.

☑️ **Do This:** Have students choose the “Image Project” option for this first exploration with Teachable Machine.

🎙️ Remarks: Take a few minutes to explore the Teachable Machine. Can you figure out how it works … how to gather samples … how to add classes … how to train a model. Play around with with the interface and options - don’t worry, you can’t break it! Explore!

☑️ **Do This:** Allow students several minutes to explore Teachable machine. Encourage them to click around through the different sample options, create at least two classes, and to run the “Training” to see what happens.

💬 **Discuss:** What did you notice as you explored the Teachable Machine?

💡 **Discussion Goal:** Here are some key things students may notice: The Machine Learns Quickly: Students might notice that Teachable Machine starts recognizing patterns or objects almost immediately after a few examples are shown. Different Results with Small Changes: They may observe that slight changes (like moving the object closer or further, changing angles, or altering lighting) can lead to different recognition results. Needs Examples to Understand: The machine requires examples to learn what an object looks like; it doesn't "know" anything until it's shown examples. Fun and Interactive: Students might find the process of teaching the machine and seeing instant feedback engaging and surprising.

💬 **Discuss:** What do you wonder?

💡 **Discussion Goal:** Student results will vary. Here are some common questions students might have after a short, five minute session with Teachable Machine: Why does it sometimes get it wrong? Students might be curious about why the machine doesn't always recognize objects correctly, even if they've just shown it similar examples. Does it remember what we showed it? They could wonder if the Teachable Machine retains the information from their session for the next time it's used. Can it learn to recognize me? Some students might be intrigued by the possibility of the machine learning to recognize them personally or specific gestures they make. How does it know what it's seeing so fast? The immediate feedback from the Teachable Machine might lead students to question how it processes information quickly. What else can it learn to do? Curiosity about the scope of Teachable Machine's learning capabilities, wondering if it can learn tasks beyond simple object or gesture recognition.

Teaching Tip During the discussion, the teacher should encourage students to reflect on these observations and questions, guiding them to understand the the importance of diverse and extensive training data. This discussion can significantly deepen students' comprehension of how AI models are trained and the complexities involved in creating accurate, fair, and reliable AI systems.

🎙️ Remarks: Let’s take a look at how Teachable Machine works. As you watch this short video, think about what would be important to do when training the model to know the difference between “you” and “your dog”.

💬 **Discuss:** What would be important to do when training the model to recognize “you” vs “your dog”?

💡 **Discussion Goal:** Students should recall their experience with the Training Data Pictionary warm-up activity and be able to recognize that the machine will learn better with more examples that are diverse with varied contexts. Students should understand that exposing AI to multiple contexts enhances its ability to generalize across different scenarios, making it more effective in real-world applications.

🎙️ Remarks: Let’s watch the last part of the video. As you watch section, keep in mind what kinds of data you can use with the machine.

💬 **Discuss:** What kinds of data can you use with the Teachable Machine?

💡 **Discussion Goal:** Students should be able to ascertain from the video that they can use images, video, or audio. Encourage students to start thinking about what kinds of data they will need to work with for their group’s CV application.

☑️ **Do This:** Direct students to discuss what kind of model(s) they want to create with their PBL group. Each student in the group should create their own model.

Teaching Tip There can be different models within the same group if the CV application has more complicated functions. Otherwise, group members can create the same type of model and compare results and experiences.

☑️ **Do This:** Direct students to start a new project by clicking on the “hamburger” icon in the top left corner and then “New Project”

☑️ **Do This:** Have students choose one of the types of projects that would best fit with their group’s CV application.

☑️ **Do This:** Direct students to create their own models using the Teachable Machine. As they create and test, they should fill in the table in their CV Design Document with “Category (class)”, “Testing technique”, “What the model did well”, and “What did not work about the model”.

🔁 **Circulate:** As you move around the room, encourage students to retrain their models to get better results.

☑️ **Do This:** Direct students to save their models into a Google account which will make it easy to share in their project later

💬 **Discuss:** What did you think was the hardest part of creating your model? How did you overcome it? Any surprises about how your model performed?

💡 **Discussion Goal:** This discussion should encourage students to articulate the problem-solving strategies they employed, highlighting the importance of creativity, persistence, and adaptability in the field of AI. It aims to provide students with insight into the iterative process of model development, including the importance of troubleshooting and refining based on performance feedback.

💬 **Discuss:** How do you envision that your model might actually be used?

💡 **Discussion Goal:** The goal here is to inspire students to think creatively about the practical applications of their AI models, fostering a forward-thinking mindset. This encourages students to connect their technical skills with the real-world problem they are trying to solve, envisioning how their work could have a tangible impact.

☑️ **Do This:** Direct students to discuss their experiences with the models they just created and tested. Students can refer to their CV Design Document to see some guiding questions that will help them evaluate their models.

🎙️ Remarks: Your model will be the first component of a larger prototype that you will be designing and building out over the next few class sessions. From here, what you create and how you create it will be the decision of the group. As we build on to our prototypes, we will learn more about some of the options that are available to us, and the various forms that it might take. This Teachable Machine model is a great first step in prototyping!

🖼️ Display: Lesson Objectives

🖼️ Display: Question of the Day

🖼️ Display: Key vocabulary
