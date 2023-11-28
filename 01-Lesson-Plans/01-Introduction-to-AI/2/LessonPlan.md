## 1.2: The Impact of Machine Learning

### Overview

Today’s lesson will begin with a series of activities to delve deeper into AI and machine learning (ML). Students will learn the differences between unsupervised and supervised ML, and will then be introduced to more complex models such as neural networks, deep learning, natural language processing, and transformers. In the AI foundations section of the course (the second half), students will learn about file version control and how to upload files to GitHub, which will be used throughout the course.

### Class Objectives

By the end of today's class, the students will be able to:

* Compare and contrast supervised and unsupervised ML.

* Define complex AI models including neural networks, deep learning, natural language processing, and transformers.

* Download and upload files to GitHub using the git GUI.

* Add, commit, and push code to GitHub from the command line.

---


### Instructor Notes

Begin this lesson with a brief lecture to introduce the differences between supervised and unsupervised ML. Use visual aids to help clarify these concepts and consider using real-world examples. Then move on to the more complex AI models. Break these down into manageable parts and explain each concept in detail. For the practical part of the lesson, provide a step-by-step guide on how to use Git GUI and the command line for GitHub operations. Include time for students to practice these skills under your guidance. Wrap up the lesson by checking students' understanding and answering any questions.

---


### Class Slides

The slides for this lesson can be viewed on Google Drive here: [Lesson 1.2 Slides](https://docs.google.com/presentation/d/1T7aty6abx7MO3xoPMSoEKFaVBqC4GJjC42txFFm_gSM/edit#slide=id.g21f2d3f9243_0_462).

To add the slides to the student-facing repository, download the slides as a PDF by navigating to File, selecting "Download as," and then choosing "PDF document." Then, add the PDF file to your class repository along with other necessary files. You can view instructions for this [here](https://docs.google.com/document/d/1XM90c4s9XjwZHjdUlwEMcv2iXcO_yRGx5p2iLZ3BGNI/edit).

> **Note** Editing access is not available for this document. If you wish to modify the slides, create a copy by navigating to File and selecting "Make a copy...".

---


### Time Tracker

| Start Time | Number | Activity                                           | Duration |
| ---------- | ------ | -------------------------------------------------- | -------- |
| 6:30 PM | 1 | Instructor Do: Introduction to Class | 0:05 |
| 6:35 PM | 2 | Instructor Do: Demystifying Machine Learning | 0:15 |
| 6:50 PM | 3 | Instructor Do: Advanced Technologies | 0:15 |
| 7:05 PM | 4 | Instructor Do: Machine Learning is Awesome | 0:15 |
| 7:20 PM | 5 | Instructor Do: AI Foundations | 0:05 |
| 7:25 PM | 6 | Instructor Do: Intro to Git | 0:25 |
| 7:50 PM | 7 | BREAK | 0:15 |
| 8:05 PM | 8 | Student Do: Create a Repository | 0:15 |
| 8:20 PM | 9 | Instructor Review: Create a Repository | 0:05 |
| 8:25 PM | 10 | Instructor Do: Pull Requests and Code Review | 0:05 |
| 8:30 PM | 11 | Student Do: Protect Main Branch | 0:15 |
| 8:45 PM | 12 | Instructor Do: Branching | 0:15 |
| 9:00 PM | 13 | Student Do: Git Branching, Pushing | 0:15 |
| 9:15 PM | 14 | Everyone Do: Git Practice | 0:10 |
| 9:25 PM | 15 | Instructor do: Wrap up class | 0:05 |
| 9:30 PM |        | END                                                |          |

---
### 1. Instructor Do: Introduction to Class (5 min)

Welcome students to the second day of class and the next lesson in Module 1.

Take some time to introduce the topics that will be covered in this lesson: the differences between supervised and unsupervised learning, an exploration of neural networks, deep learning, natural language processing, and transformers, as well as the technical skills related to working with GitHub. This lesson will continue introducing students to the skills and knowledge required to gain a deeper understanding of AI engineering.

Use the slideshow to review the objectives for today's class.

Cover the following points:

* Today, students will begin to learn about different learning strategies and AI models in a theoretical capacity. Later units and activities will delve into hands-on experiences with advanced tools, techniques, and technical concepts.

* Students will continue their introduction to working with fundamental developer tools, which started last lesson with the command line. By the end of today they will be familiar with the processes involved with working collaboratively using the git version control system.

Encourage students and get them excited for the lesson. Reiterate that today will be a crash course in both hard and soft skills: students will learn technical skills and contextual knowledge to aid them in their future careers in AI.

---


### 2. Instructor Do: Demystifying Machine Learning (15 minutes)


Open the slideshow and continue through, covering the following talking points:

* ML is a subset of AI.

* ML is the use of algorithms and statistical models to make decisions or predictions about data.

* Today, ML is changing the world at an unprecedented pace. These changes are driven by automation, which enables quick and efficient decision-making.

Next, send out the link (Source: [Twilio blog](https://www.twilio.com/blog/ultimate-guide-openai-gpt-3-language-model)) while explaining the following example of how ML can be useful in the field of finance:

Imagine that you work as a fraud analyst in a bank and want to identify fraudulent transactions. One option is to create a 5,000-line if-else decision structure that evaluates every price range and product category to determine if a transaction counts as fraudulent. Or you can use ML algorithms to review all the transactions that an account owner has made, and then have the model group the transactions and predict whether the most recent transaction counts as fraudulent.

**Types of ML**

Ask the students for some examples of ML models they have heard of before. If no one volunteers, provide some examples, such as regression, clustering, classification, and deep learning.

Use the graphic on the slide to explain that we can group all these models into two main buckets:

* **Unsupervised learning:** The algorithm tries to make sense of an unlabeled dataset by extracting features and patterns on its own.

* **Supervised learning:** The algorithm learns on a labeled dataset where each example in the dataset is tagged with the answer. This provides an answer key that can be used to evaluate the accuracy of the training data.

Tell the students that in later lessons, they will get hands-on experience using both unsupervised and supervised ML models in different applications.

Move onto the next slide to compare and contrast supervised and unsupervised ML.

Move onto the next slide to go into detail on **unsupervised learning**.

Explain that unsupervised learning uses unlabeled data, which represents raw information, to find patterns or to group data.

Use the graphic on the slide to explain the following steps in unsupervised learning:

1. Interpret unlabeled data.

2. Use an algorithm to process the data.

3. Create the output of groups by characteristic.

Mention a few applications where unsupervised learning is particularly useful:

* Exploratory data analysis

* Cross-selling tactics

* Consumer segmentation

* Pattern recognition (since it can identify similarities and differences in large volumes of information)

Move onto the next slide to explain **supervised learning**.

Explain that, in contrast to unsupervised learning, programmers “supervise” the algorithm’s learning by feeding it carefully selected data with known outcomes, which the model can then use to make the most accurate predictions possible.

Explain the supervised learning training cycle:

1. Provide the algorithm with categories.

2. Feed additional data into the training cycle, guiding it towards better results.

3. Assess model performance and make adjustments to optimize results.

After supplying the algorithm with data and expected outcomes, the model can learn how to make predictions for new pieces of data that have similar features.

Introduce a practical example of ML. Feel free to use one of your own or the one provided below:

Assume that you have a dataset of high-risk versus low-risk loans, and the factors that led to those results. You can use that information to improve the model's predictive capability. After that initial data is fed into the algorithm, you can identify the algorithm’s mistakes and make adjustments to improve its performance on future datasets. Once it’s trained, a supervised learning model can then learn from its own “mistakes,” and continue to improve predictions on new pieces of data, such as a new consumer loan.

Before wrapping up, explain that even though algorithms learn from data in supervised learning, there are still limitations, and complex problems require complex systems to solve them. Much of the current research in AI is in building upon our current technology of supervised and unsupervised learning to create even more complex algorithms that solve increasingly complex problems.

Answer any questions before moving on.

---


### 3. Instructor Do: Advanced Technologies (15 minutes)


In this section, students will be introduced to further, more complex ML concepts, including neural networks and deep learning.

Continue navigating through the slides as you cover the following points:

**Neural networks**, also known as artificial neural networks (ANN), are a set of algorithms that are modeled after the human brain. Neural networks are designed to mimic the way our brains function, with artificial neutrons serving the same purpose as our biological neurons.

Use the graphic on the slide to illustrate how a neural network functions at a high level.

Use the table on the slide to explain some advantages of neural networks over traditional statistical or machine learning models:

Advantages:

* Neural networks can effectively detect complex relationships in data, such as predicting future shopping behavior based on credit card transactions, or a loan applicant's likelihood of defaulting on a loan based on their application.

* Neural networks have greater tolerance for messy data. They can learn to ignore noisy characteristics within a large dataset.

Disadvantages:

* The neural network algorithms can be too complex for humans to dissect and understand (creating a black box problem).

* Neural networks are prone to overfitting (characterizing the training data so well that the model does not effectively generalize to test data).

Call out that model designs and optimization techniques introduced later in this course can help account for, and mitigate both of these disadvantages.

Ask if there are any questions about neural networks so far, then move onto the next slide.

Explain that **deep learning** is a type of neural network that consists of three or more layers. These additional layers help make the algorithm even more efficient and accurate than a traditional neural network.

Use the graphic on the slide to explain how deep learning functions at a high level.

Call out that what makes a neural network model considered deep learning is the number of hidden/additional layers.

> **Note** Precise definitions vary by source. In this course, we’ll classify any neural network with more than one hidden layer as “deep.”

Explain that the advantage of deep learning is that, unlike most other ML algorithms, these models can discover nonlinear relationships among data.

Each additional layer of neurons makes it possible to model more complex relationships and concepts.

An example could be a neural network designed to classify whether a picture contains a cat, which will follow these steps:

1. The model checks whether any animals exist in the picture.

2. Drilling deeper, the model checks for the presence of paws, pointed ears, or other “cat” features.

3. The model will continue breaking down the challenge in this way until it reaches raw input&mdash;the picture’s individual pixels.

Explain that by specifying the problem correctly, a user enables the model to process each of these conceptual steps on a different neuron layer.

Transition to natural language processing by explaining that it is one of the main applications of neural networks.

Introduce **natural language processing (NLP)** by explaining the inherent challenges of language processing:

* Computers don’t naturally understand and process data the way humans do. Instead, they store data as zeros and ones, known as **binary code**. They’re able to interpret this data as instructions on how to display text, sound, images, or video.

* To communicate with and/or instruct computer systems more simply or naturalistically, we must combine various AI technologies and ML algorithms to enable computers to understand written text and spoken words similarly to humans.

Using the next slide as a guide, define NLP as the following:

NLP combines the rules of human linguistics with ML algorithms not only to translate text into a format that a computer can understand, but to essentially understand the meaning behind the words, including the writer or speaker’s intent and sentiment.

Move onto the next slide to explain that “a **large language model** is a type of deep learning algorithm that can recognize, summarize, translate, predict, and generate text and other content based on knowledge gained from massive datasets” (Lee, 2023).

Moving onto the next slide, explain that, “A transformer model is a neural network that learns context and thus meaning by tracking relationships in sequential data like the words in this sentence” (Merrit, 2022).

At a high level, explain how transformer models work using the slide as a guide:

1. Text or spoken words are fed into the algorithm, which extracts the data and breaks each element into individual words or phrases through a process called **tokenization**.

2. The algorithm classifies and labels each element.

3. Using statistical training, the algorithm proposes the *most likely* meaning of the data.

Explain that NLP algorithms are becoming increasingly popular, in part, due to the availability of pre-trained models which help reduce computational costs and enable advanced models.

Some applications include:

* Distinguishing spam from legitimate emails

* Translating from one language to another

* Social media sentiment analysis

* Chatbots and virtual agents

Ask for and answer any questions students may have before moving on.

---


### 4. Instructor Do: Machine Learning is Awesome (15 minutes)


This section uses a demo made by the [Teachable Machine project from Google](https://teachablemachine.withgoogle.com/v1/) to show the students how ML works and to build excitement about the ML curriculum.

Highlight an up-and-coming area of ML called **neural networks** in the following demonstration:

* Open your web browser and navigate to [the Teachable Machine website](https://teachablemachine.withgoogle.com/v1/). This web application shows the fundamental mechanism of a neural network by training a model that recognizes gestures from your webcam to predict one of three classes.

Once you open the Teachable Machine website, follow the next steps to conduct the demo:

* Click the “skip the tutorial” option to start the demo.

![A screenshot shows the Teachable Machine website and the option to start the demo.](https://static.bc-edx.com/ai/ail-v-1-0/m1/lesson_2/img/intro_nns_1.png)

* Allow the web application to use your webcam and microphone.

![A screenshot shows the Teachable Machine website and the option to allow webcam and microphone access.](https://static.bc-edx.com/ai/ail-v-1-0/m1/lesson_2/img/intro_nns_2.png)

Explain to the students that now you are going to train the neural network model by doing the following:

1. Raise your left hand and press the TRAIN GREEN button for a few seconds. Your current image is the input data for the neural network. It's learning that these visual patterns correspond to a cute kitten.

![An animation of the “train green” button being clicked, resulting in a video of a kitten in the output box.](https://static.bc-edx.com/ai/ail-v-1-0/m1/lesson_2/img/intro_nns_3.gif)

2. Continue to train the purple class by posing seriously for the camera. Press the TRAIN PURPLE button for a few seconds. Now the neural network is learning that your poker face corresponds to a furry dog.

![An animation of the “train purple” button being clicked, resulting in an image of a dog in the output box.](https://static.bc-edx.com/ai/ail-v-1-0/m1/lesson_2/img/intro_nns_4.gif)

3. Finally, train the orange class by making a funny face and pressing the TRAIN ORANGE button for a few seconds. You are telling the neural network that this funny pose corresponds to a little bunny.

![An animation of the “train orange” button being clicked, resulting in an image of a bunny in the output box.](https://static.bc-edx.com/ai/ail-v-1-0/m1/lesson_2/img/intro_nns_5.gif)

Now that you have trained the model, play around by making several poses and faces for the camera:

* Raise your right hand. Although the neural network was trained to recognize your left hand raised, these kinds of models are continuously learning and capable of recognizing and learning new patterns.

* Make a tricky test by partially raising your left hand. The neural network gets confused but is still learning, as can be seen on the confidence bars; finally, the model can decide on your partially raised hand.

![A video of a person raising their hand.](https://static.bc-edx.com/ai/ail-v-1-0/m1/lesson_2/img/intro_nns_6.gif)

Explain to the students that this funny experiment is just an example of the power of ML, but instead of matching gestures with silly pets, you can use this kind of technology for AI applications.

With their excitement about ML at a peak, let the students know that they will be developing their own ML algorithms later in the course.

---


### 5. Instructor do: AI Foundations (5 minutes)


Today’s AI foundations section will cover GitHub, the industry-standard collaboration tool.

Students will use it to store their code, collaborate with their peers on projects, and submit assignments.

Tell students that their first Challenge assignment will be creating a repo with GitHub, so learning these skills is very timely.

Getting comfortable with Git and GitHub will be critical for their success in the boot camp, and post-graduation, so they should invest the time now to get to know it very well. Ask questions early if they are struggling.

---


### 6. Instructor Do: Intro to Git (25 minutes)

Today, we will delve into Git and how to use it through the Terminal to interact with GitHub.

In this section, you will discuss the importance of version control in the process of software development.

Start by asking students questions about their own experiences with version control:

* How did you collaborate with others?

* How did you manage changes to your work?

Then transition to talking about Git and GitHub. Ask students the following questions:

* Did you use GitHub before beginning this boot camp?

* If so, how has your usage changed? If not, how has your experience with it been so far?

> **Note** If teaching with VS Code, consider using the [Git History](https://marketplace.visualstudio.com/items?itemName=donjayamanne.githistory) extension to demonstrate this section's concepts.

Continue the slideshow to facilitate discussion of the next topic.

* Explain that Git is essentially a way for us to keep track of our work over time. Whenever we get another piece of a project working, we can save the change with Git.

* Note that this "save" is called a **commit**. It represents a checkpoint for our project where we save and describe our work.

Emphasize that if we break something while working on our code, this system allows us to restore working code from earlier.

Note that since Git remembers these checkpoints, we can work on several different concerns all at once.

Provide the following example:

* Suppose we need to analyze Uber ride data for a project.

* Explain that we might decide to analyze the average age of riders. Git essentially allows us to write this code and save it with the name `age analysis`.

Emphasize that this code is *different* from the code we started with and that it lives separately from it.

* Explain that in this scenario, we have a version of the code called `main`, which is the main version of our code. We also have a version called `age analysis` that contains updates.

Note that each version of the code lives on a different **branch**.

* Explain that a **branch** is essentially a history of changes.

* Note that in this case, we say that the `age analysis` branch **diverged** from the `main` branch.

* Take a moment to demonstrate the difference between the files on the `age_analysis` and `main` branches.

Explain that saving the age analysis code in a different branch gives our teammates a chance to review it for errors and offer suggestions.

After the proposed change has been reviewed, we can update the `main` branch to include the changes in `age analysis` by doing a **merge**.

Explain that **merging** two branches combines them into one branch.

Explain that this is how we can work on new features or bug fixes without making changes to working code.

* Note that this also makes working with teammates easier, as people can avoid stepping on each others' toes by working on different branches.

Review the popular Git commands with the class:

* `git clone`: Clones a git repository onto the local file system.

* `git add`: Adds changed files to the queue of tracked files ready to be committed.

    * Adding a period after `git add .` adds all the files to the queue.
    * Or, you can add a file(s) or folder name to add specific file, files, or folders.

* `git commit`: Adds tracked files as a bulk checkpoint ready to be pushed to the remote git repository.

* `git push`: Uploads changed files from the local git repository to the remote git repository and updates the remote files.

* `git pull`: Downloads changed files from the remote git repository to the local git repository and updates the local files.


Finally, review Git's **snapshot model**. Slack out the link to *Pro Git* (a book of GitHub documentation) where this is discussed: [“Getting Started - What is Git?”](https://git-scm.com/book/en/v2/Getting-Started-What-is-Git%3F).

* A commit in GitHub is like a snapshot of what your project or file looks like at a particular moment in time.

* If a file doesn’t contain any changes, the file is not stored again; instead, Git provides a link to the identical file that it previously stored.

* According to the documentation, “Git thinks about its data more like a stream of snapshots.” (Chacon & Straub, 2023)

* Highlight the images (available at the previous link) that capture the Git snapshot model, which differentiate between changed and unchanged files.

---

### 7. BREAK (15 minutes)

---


### 8. Student Do: Create a GitHub Repository (15 min)


**Files**

[README.md](Activities/01-Stu_Create_Github_Repo/README.md)

In this activity, students will get some additional practice creating a repository via the terminal. Tell students they will do the following:

* Create a repository for the AI application, including a `README.md` file that follows the [template](Activities/01-Stu_Create_Github_Repo/README.md) provided in the activity files.

Reiterate that students should create their repos using Terminal:

* Use only Terminal commands in order to do this; don’t use the GUI or VS Code.

**Instructions:**

1. Create the repository

    * Create a GitHub repository with a name that describes your AI application.

    * Initialize your repository with a `README.md` file.

    * Once your repository is created, click the green "Code" button and copy the https clone link.

2. Clone the repository

    * Open a Terminal window and use `cd` commands to navigate to the directory where you would like to save your repository.

    * Use the `git clone` command and the link you copied previously to clone the repository in the location you selected.

3. Add and edit files

    * Copy the files for your AI application into this folder.

    * Edit your `README.md` file so that the headers match the [README template](Activities/01-Stu_Create_Github_Repo/README.md).

    * Fill in the sections of the `README.md` file with brief descriptions.

4. Stage and commit changes

    * Use the `git status` and `git add` commands to review the changes you have made and track your new files.

    * Once you have tracked your files using `git add`, commit these changes with a message using `git commit -m` followed by a short but descriptive summary of what you changed.

5. Push local changes to remote repository

    * Use the `git push` command to copy your local changes to the GitHub remote repository.

    * Go to your Github repository to see your changes.

---


### 9. Instructor Review: Create a Repository (5 minutes)


At this point, instructional staff checks in with each student to ensure their repo was created correctly.

---


### 10. Instructor Do: Pull Requests and Code Review (5 minutes)


Explain that when working with others on the same repo, it's important to make sure that all of the new code gets reviewed by at least one other team member before getting merged into the main branch.

Assure the class that we'll go into further detail about how this is done, but ask the class: "Why would we want to get code reviewed before merging it into the main?"

Reviewing new code decreases the chances that broken code will accidentally be introduced into the main branch. Code review helps group members who didn't write the code understand how it works.

Explain that the next step of setting up our project repos for group collaboration is to protect the main branch.

Protecting the main branch means we will configure the repo to prohibit any team members from pushing code up into the main directly, or merging it in without another team member's review.

---


### 11. Student Do: Protect Main Branch (10 minutes)


**Corresponding activity** [02-Stu_Protect_Main_Branch](Activities/02-Stu_Protect_Main_Branch/)

In this activity, groups will protect their main branches.

Slack out the [README.md](Activities/02-Stu_Protect_Main_Branch/README.md) file to the class and have students complete this activity with their groups.

---


### 12. Instructor Do: Branching (15 minutes)


> **Note** For now, we just want to give students a high-level conceptual understanding of branching.

Continuing with the slides, explain the following points about branching:

* Every Git repo starts off with a main branch, which is there to hold the production version of the repo's code. But when we want to work on the code, we start by creating a new feature branch off the main.

* If we create a new branch from the main, we essentially create a self-contained copy of all of the main branch's code for us to work in.

* When we're satisfied with our work in the new feature branch, we submit a pull request from the feature branch to the main branch.

* A pull request is a request to merge the **diffs** or changes from the source branch (the feature branch) to the target branch (main).

* With the way our repos are set up now, another group member must look at and approve the pull request before its changes can be merged into the main.

* Once a feature branch has been merged into the main, we delete it and then check back out to the main branch. From there, we'd check back out to a new feature branch, and repeat the process for each feature we add.

Take a moment to answer any questions, but avoid going too in depth. Students will utilize branches in the next activity.

---


### 13. Student Do: Git Branching and Pushing (15 minutes)

**Corresponding activity** [03-Stu-Git_Branching_Pushing](Activities/03-Stu-Git_Branching_Pushing/)

In this activity, students will create branches, submit pull requests, and perform code reviews before merging.

Slack out the [README.md](Activities/03-Stu-Git_Branching_Pushing/README.md) file to the class and have students complete this activity with their groups.

Instructional staff should be walking around the class making themselves available for assistance, and ensuring students understand the instructions.

---


### 14. Everyone Do: Git Practice (10 minutes)


Ask the class for any questions, and take a few minutes to review any commands that weren't clear. Offer to help students throughout the day and during office hours.

Explain to students that this will be the new, primary way of submitting homework to GitHub (no more manual uploads!).

Reassure them that it's okay if it takes them time to get comfortable with Git. By the end of the course, they will be Git pros!

Draw on your own personal experience to discuss common errors or pitfalls beginners encounter when using Git, and how to resolve them.

Encourage students to continue adding and committing today’s activities into a repo for additional practice.

---


### 15. Instructor do: Wrap-up Class (5 minutes)


Use the last few minutes of class to allow the students to digest and decompress from this lesson.

First, congratulate students for completing this class! They should be proud, as the pace of today's class was much quicker than the previous class.

Recap today's objectives. Students are now able to:

* Compare and contrast supervised and unsupervised ML.

* Define complex AI models including neural networks, deep learning, natural language processing, and transformers.

* Download and upload files to GitHub using the Git GUI.

* Add, commit, and push code to GitHub from the command line.

Ask students if they have any questions about the homework.

Tell students that in the next class they will learn about AI interactions, impacts, and foundations, as well as learning more about using the Terminal, README.md files, Anaconda, and virtual environments.

Ask if students have any remaining questions before ending the class. If needed, TAs will host office hours after class.

End Class
---


### References

Lee. A. 2023. *What are large language models used for?* Available: [https://blogs.nvidia.com/blog/2023/01/26/what-are-large-language-models-used-for/](https://blogs.nvidia.com/blog/2023/01/26/what-are-large-language-models-used-for/) [2023, April 6].

Merritt. R. 2022. *What is a transformer model?* Available: [https://blogs.nvidia.com/blog/2022/03/25/what-is-a-transformer-model/](https://blogs.nvidia.com/blog/2022/03/25/what-is-a-transformer-model/) [2023, April 5].

Chacon, S. & Straub, B. 2023. *Pro Git.* Mountain View, USA: Apress. Available: [https://git-scm.com/book/en/v2](https://git-scm.com/book/en/v2) [2023, June 13].

---

© 2023 edX Boot Camps LLC. Confidential and Proprietary. All Rights Reserved.