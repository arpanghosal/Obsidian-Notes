
## Obsidian:
cmd + opt + i   - to got to developer mode

cmd + r  and cmd shift r = record and stop
cmd + shift + c = change color from palette below

ctrl + p,o,y,g,c -> highlight
ctrl + r -> remove highlight


## Links:
https://www.inovex.de/de/leistungen/artificial-intelligence/ - for ML related stuffs


[[Tutorials-Things to do]] -> Uproot comes with Scikit-HEP package. Major advantage. - calls compiled vectorized functions to perform very fast calculations on arrays



Start jupyter-notebook from your browser - any folder. 
$ jupyter-notebook
This will open from the same directory in browser. 


## ssh - config setting and key 
 ssh-copy-id aghosal@lxplus.cern.ch

---

## vnc
screen -S vnc

k5reauth -x -f pagsh

aklog

bash

vncserver -geometry 1800x1000 :2 (session=2 is the port where server is running, might be already occupied, use any free. Play with the resolution as you need)

k5reauth -x -f pagsh

aklog

ctr+a and then d to detach from screen.

Then (later) change machine number and session number in your file (i think it is impfiles/vnc.sh (config for mac)) –

In lxplus : cd .vnc; ls and then you can see the pid of the current machine and the channel.

config lxplus713.cern.ch:2.pid lxplus767.cern.ch:2.log

lxplus610.cern.ch:9.log lxplus713.cern.ch:9.log

then you need to change your vnc.sh file. change machine number to 713, and in which screen did you open ? if you have used this "vncserver -geometry 1800x1000 :2" then this :2 means screen 2.

so in vnc.sh file change 5909 to 5902. it will be 5902:localhost:5902

---
## Siegen cluster trex-fitter
setupATLASSi
lsetup root (latest version 6+)
source setup.sh
then do trex-make 


---
vim 
:nohl - to turn off yellow highlighting which comes up with using ^&


## Print on Siegen cluster
For digital form, while printing, use Print to Files option.
A \*.ps  file will be saved. Take care of path.
Convert it to pdf using $ ps2pdf \*.ps \*.pdf 

---

## Computer architecture
As a user you are interested in reducing the response time (also called the
execution time or latency). The computer manager is more interested in
increasing the throughput (also called bandwidth), the number of jobs
done in a certain amount of time.
### clock cycle :
The choice of clock speed depends on the specific requirements of the system and the balance between power efficiency, heat management, and performance. For desktop computers, gaming systems, and high-performance servers, faster clock speeds are often desired to achieve better performance. On the other hand, mobile devices and laptops may prioritize power efficiency and longer battery life, which can be achieved with slower clock speeds.

A cluster is essentially a large computer that is made up of many smaller computers. The smaller computers are called nodes, each node has its own RAM (memory) and a specific number of processors, also called cores. The OMNI cluster has about 450 **compute nodes** for running computations, 4 **login nodes** which are directly accessible to users, and a number of specialized nodes.

---
#obsidian
fn cmd left/right arrow - pg up down


----
## Root.   #root

- sumWeights->Scan("names_mc_generator_weights","","colsize=30")

#### <mark style="background: #FFB8EBA6;">show full:</mark>
root [8] sumWeights->Scan("*","","colsize=30"); // adjust col size

---
### File search

find . -type f -name 'run.sh' 

----
HTTPs error codes :
- **100s**: Informational status codes that indicate continuing requests.
- **200s**: Success codes for well-functioning requests.
- **300s**: Redirection messages explaining a [redirect](https://kinsta.com/docs/redirect-rules/) to another resource.
- **400s**: Error codes for client-side problems.
- **500s**: Error codes for server-side issues.
---

[[project - js to html]]   - WIP



## Notes for obsidian:

[[obsidian]]

----

## Rucio -> request for files on tape :
1. Go to https://rucio-ui.cern.ch/r2d2/request 
2. Create request by chosing container and some proper scratchdisk (whatever is suggested).
3. Sample numbers can also be constrained.
4. You get a new DID from where you can download (in a few hrs) :

![[Pasted image 20231024145639.png]]

$ rucio download --nrandom=2 user.aghosal.mc16_13TeV.504554.aMCPy8EG_tty_yprod.merge.EVNT.e8261_e7400_der1698137653

----


## Bash commands : #bash #shell

$ open -a <app_name> \*.pdf
### epub to pdf

To convert book types, ahve calibre installed first.
$ ebook-convert \*.epub  \*.pdf 


### bash command to 'NOT' ls a filetype
ls -l | grep -v '\.log$'

---

## How to research:

What you're experiencing is a common issue known as "information overload" or "analysis paralysis," where the vast amount of available information can become overwhelming and distracting. Here are some strategies to manage this issue better:

1. **Define Your Objective:**
   - Clearly define what you want to learn or decide before you start researching. Write down a specific question or thesis you are trying to answer.

2. **Set Limits:**
   - Give yourself a time limit for the initial research phase.
   - Limit the number of sources you consult.

3. **Stay Organized:**
   - Keep notes of your research process, including where you've looked and what you've found.
   - Use digital tools like Evernote, OneNote, or a simple document to organize your thoughts.

4. **Summarize Regularly:**
   - After each article or source, summarize the key points and how it relates to your main question.
   - This helps cement the information and maintain focus on your objective.

5. **Create an Outline:**
   - Make an outline of the topics and subtopics you need to cover.
   - Stick to the outline and resist the urge to go off on tangents.

6. **Implement the "Five Sentence Rule":**
   - When you read an article or paper, try to summarize it in five sentences or less to focus on the main points.

7. **Use the Pomodoro Technique:**
   - Work for 25 minutes, then take a 5-minute break.
   - This can help you stay focused on one thing at a time.

8. **Learn to Recognize When You're Satisfied:**
   - Accept that there will always be more to learn, and you don’t need to read every single source to get a good understanding of a topic.
   - Decide in advance what constitutes "enough" information.

9. **Reflect on Information Value:**
   - Not all information has the same value. Ask yourself how important the details are to your main objective.
   - This will help you decide whether to dig deeper or move on.

10. **Use Distraction Blocking Tools:**
    - Consider using website blockers to keep you from straying off into unrelated topics.

11. **Practice Mindful Research:**
    - Be present with your research. When you notice your attention drifting, gently bring yourself back to your main objective.

12. **Allocate Time for Exploration:**
    - Set aside separate time for open-ended exploration, which can be satisfying and creatively stimulating, but keep it distinct from focused research time.

13. **Review and Adjust Your Approach:**
    - Periodically step back and review the information you've gathered. Adjust your approach if you find yourself deviating from your main objective.

Remember, research is an iterative process. It's often necessary to go through several rounds of refining your focus based on what you learn along the way. But with practice and discipline, you can train yourself to stay on task and manage the wealth of information available to you more effectively.


## In a nutshell:
> try to set clear goals 
> try to set limits on what you read. Literary research is important.
> try to stay organized with notes and everything.
> > >Probably mention in your notability app - analysis or whatever note you're writing during first read. include references etc. as well. 
> > >In second read, mention stuffs in obsidian as well. highlight stuffs if you read on zotero. Add comments on notes themselves in real time so you don't forget them.
> create outline while you work. 
> write summary in < 5 sentences to squeeze everything you learnt - can be article wise (obsidian or notion daily tasks), can be topic wise (digital notes on notability probably best place to do so), codes - try to archive to git.
> reflect on the information value.
> set apart time for open ended research - excluding it from actual research you do during work time.
> keep timely reviews of things and projects.


So here are things you should take care of:
1. obsidian self notes - for yourself . Like this one [[Self Notes]]
2. obsidian has pages for science stuffs, non science stuffs, analysis and computing etc.
3. notion - try to take down everyday summaries of what you did and what you learnt, just to keep track. 
4. notion - make plans in to do pages.
5. notability - trivia notes for trivial mapping of ideas
6. notability -  Streamlined notes in "Mind map - Analysis and more". Here put stuffs from work and productive life.
7. Zotero - there are int notes, papers, interesting books, presentations, etc. to be read. Both academic and non academic.
8. Make use of chatgpt and youtube to learn more.
9. Work on expanding github repo base with more projects and skills, that would be beneficial.

<span style="color:#0ff549">
Take Notes, //
use softwares, //
have Patience, //
Get in the mindset - broadest possible search engine  - google trends, Wikipedia, Google Scholar, scientific peer review, Journals ; //
Find review paper check primary source, //
How to read research effectively  - abstract, intro, figures, results and then methods if you must.
When to stop why are you actually doing this. Start writing. </span>

----

## How to make a good presentation ?
 - have a clear message - keep it clear and terse
 - don't overdo, don't overload slides.
 - interact with audience.
 - message should be clear - why are you doing what you do? do you know well what you are attempting? do you know the consequences? if you change something a little bit, how much would it impact other things? what's the overview? what's the nutshell message from these slides or routines?
 - practice a lot 
 - be engaging toward your audience. Know your audience well. Don't waste their time by showing things they don't care about or probably won't understand.
 - End with a strong call for action. 
 - Elevate your slides with ample visuals and visual hints such as if there are too many things crammed in a single slide, simplify it for audience. Give visual cues. you don't want to lose your audience. Use bullets, highlighting, main takeaway messages, minor and major points, images and charts etc. in case you have an informatively loaded slide.


----

## Sending travel reimbursement request:
Use Adobe on your laptop to fill the form (otherwise xx while printing or monetary values put to 0,00). Then save it on computer, send it to markus if cern, and while sending to abrechnung@siege.... , forward the approval mail.


----

## D-ticket:
https://www.ots-nrw.de/product/213/show?active_path=ticket%7Cproduct_category_24%7Cproduct_subcategory_28%7Cproduct_213

----

## Asking chatgpt:
Keep all expressions, mathematical equations, special and greek and other characters within $ and $, so as to be easily readable in obsidian. 

---

## SSH node creation and jupyter for plots:
$  sshlxplus7 -L8869:localhost:8869 (any port number)
### set env:
[aghosal@lxplus784 fitting_tests]$ source /cvmfs/sft.cern.ch/lcg/views/LCG_105/x86_64-centos7-gcc12-opt/setup.sh

[aghosal@lxplus784 fitting_tests]$ jupyter-notebook --port=8869 --no-browser

Then click on the links

-----

## Getting Samples from Tape (LHC ATLAS)
#lhc #rucio #ATLAS 

- If you need an EVNT file that's most likely been transferred to the tape, the first thing to try is to check if the EVNT is still available.
  $  rucio download --nrandom 1 mc16_13TeV.504554.aMCPy8EG_tty_yprod.merge.EVNT.e8261_e7400
If this fails, means they are not available right now.
- How to request them?
    $  rucio add-rule mc16_13TeV.504554.aMCPy8EG_tty_yprod.merge.EVNT.e8261_e7400 1 CERN-PROD_SCRATCHDISK
    This will start adding the EVNT (all) files from tape back to disk (here CERN Prod disk)

- You can check the progress with list-rules:
  $  rucio list-rules mc16_13TeV.504554.aMCPy8EG_tty_yprod.merge.EVNT.e8261_e7400
<small><small>
ID                                ACCOUNT    SCOPE:NAME                                                              STATE[OK/REPL/STUCK]    RSE_EXPRESSION         COPIES    SIZE    EXPIRES (UTC)        CREATED (UTC)
--------------------------------  ---------  ----------------------------------------------------------------------  ----------------------  ---------------------  --------  ------  -------------------  -------------------
7054626926414c86b6c3c28ebee9307d  aghosal    mc16_13TeV:mc16_13TeV.504554.aMCPy8EG_tty_yprod.merge.EVNT.e8261_e7400  REPLICATING[0/2043/0]   CERN-PROD_SCRATCHDISK  1         N/A     2024-03-15 09:37:38  2024-03-01 09:37:39
</small></small>

7054626926414c86b6c3c28ebee9307d is the job id 

- Delete replication rule using delete-rule and ID.

---

## Lima: #todo





----
## Organizing files and folders:
Taken from a zapier blog.
- Create a clear hierarchy of folders.
- Use consistent naming convention:
  keywords, 
  pascal case, 
  add date at beginning(yymmdd_), 
  include version if working on project,
  keep filenames concise
- Add tags:
  Red - important, analysis related
  Orange - mildly relevant, official etc.
  Blue - Self study, papers etc.
  Green - Self development, codes etc.
- Archive and delete unnecessary files
- File as you go
- Name as WIP, final, archived etc.
-

----

#todo 
# Career Contemplation: 
#todo 
Transitioning into a role as a Data Analyst, Data Scientist, or Data Engineer requires a blend of technical, analytical, and soft skills. Given your background in physics, computing, and statistical skills, you're already on a strong footing. Here’s a breakdown of specific skills and resources that could help, along with advice on building a relevant portfolio:

### Technical Skills

1. **Advanced Programming**: Proficiency in Python is essential, as it's widely used for data analysis, machine learning, and data engineering tasks. R is also beneficial, especially for statistical analysis and visualizations.

2. **Machine Learning/AI**: Understanding of machine learning algorithms, principles, and their application. This includes supervised and unsupervised learning, neural networks, and deep learning.

3. **Data Manipulation and Analysis**: Skills in using libraries like Pandas, NumPy for Python. Ability to clean, manipulate, and analyze large datasets to derive meaningful insights.

4. **Database Management**: Knowledge of SQL for querying databases is crucial. Familiarity with NoSQL databases (MongoDB, Cassandra) is also beneficial for Data Engineer roles.

5. **Big Data Technologies**: For Data Engineering positions, skills in Hadoop, Spark, and Kafka are highly sought after. These technologies help in processing and analyzing large data sets beyond the capacity of traditional databases.

6. **Data Visualization**: Proficiency in visualization tools and libraries such as Matplotlib, Seaborn (Python), and interactive tools like Tableau or Power BI to communicate data insights effectively.

7. **Statistical Analysis**: Your background in particle physics and statistical skills will be invaluable. A deep understanding of statistical testing, regression analysis, and probability theory is essential.

### Soft Skills

1. **Problem-Solving**: Ability to approach complex problems logically and creatively.
2. **Communication**: Clear communication of complex data insights to non-technical stakeholders.
3. **Project Management**: Organizing, planning, and executing projects efficiently.

### Resources for Learning

1. **Online Courses**: Platforms like Coursera, edX, and Udacity offer specialized courses in data science, machine learning, and data engineering from top universities and companies.
   
2. **Books**: There are many excellent books on data science and machine learning. Some recommendations include "Python for Data Analysis" by Wes McKinney, "Data Science from Scratch" by Joel Grus, and "The Data Warehouse Toolkit" by Ralph Kimball for data engineering concepts.

3. **Competitions and Projects**: Participate in Kaggle competitions to practice your skills on real-world data sets. GitHub is also a great platform to collaborate on projects and contribute to open-source.

### Building a Portfolio

1. **Showcase Projects**: Include projects that demonstrate your ability to extract insights from data, apply machine learning models, and use data visualization effectively. Projects related to your PhD research, where you've applied data analysis or machine learning, can be very compelling.

2. **Blog Posts**: Writing about your projects or explaining complex data science concepts in simple terms can showcase your expertise and communication skills.

3. **GitHub Repository**: Maintain a clean, well-documented GitHub repository for your projects. Include clear README files that explain the projects, the techniques used, and the results obtained.

4. **Kaggle Profile**: Participating in Kaggle competitions and sharing your kernels (code notebooks) can also be part of your portfolio.

Start with focusing on a few key areas where you feel most interested or where your skills are strongest, and gradually expand your expertise from there. Balancing technical skills development with real-world applications through projects will make your transition into data science roles smoother and more successful.


"""
### 2. Data Analyst/Data Scientist in Tech or Research

- **Pros**: Your skills in C++, Python, machine learning, data analysis, and statistics are highly valued in these roles. There's a strong demand for data professionals across many sectors, offering good career growth and opportunities to work on varied projects.
- **Cons**: May require continual learning and upskilling to stay abreast of new technologies and methodologies in data science."
"""

## Expertise skills:
Transitioning to an industry job in Python and machine learning within a few months is ambitious, but with focused effort and strategic learning, it's certainly achievable. Here’s a roadmap with key areas to concentrate on, aimed at building a strong foundation in Python programming and machine learning, along with skills that are highly valued in the industry.

### 1. Strengthen Python Skills
- **Core Python**: Become proficient in Python syntax, data types, control flow (if statements, loops), functions, and error handling.
- **Advanced Topics**: Understand more complex topics like list comprehensions, lambda functions, decorators, generators, and context managers.
- **Object-Oriented Programming**: Grasp the principles of object-oriented programming in Python, including classes, inheritance, and polymorphism.

### 2. Learn Key Python Libraries
- **NumPy**: For numerical computations and understanding array manipulations.
- **Pandas**: For data manipulation and analysis, especially with tabular data.
- **Matplotlib** and **Seaborn**: For data visualization. Being able to visually explore and present data is crucial.
- **Scikit-learn**: For implementing machine learning algorithms. Understand how to preprocess data, train models, evaluate model performance, and fine-tune parameters.

### 3. Dive into Machine Learning
- **Foundational Concepts**: Understand types of machine learning (supervised, unsupervised, reinforcement learning) and key concepts like bias-variance tradeoff, overfitting, underfitting, and cross-validation.
- **Algorithms**: Get familiar with common algorithms for classification, regression, clustering, and dimensionality reduction. Know how and when to use algorithms like linear regression, logistic regression, decision trees, random forests, SVMs, k-means, and PCA.
- **Model Evaluation**: Learn how to evaluate models using metrics like accuracy, precision, recall, F1 score, ROC-AUC for classification, and MSE, RMSE for regression.

### 4. Get Hands-on with Projects
- **Practical Experience**: Apply what you’ve learned in projects. Start with simple projects and gradually increase complexity. Projects could involve data analysis, predictive modeling, or even implementing machine learning algorithms from scratch.
- **Portfolio Development**: Document your projects in a portfolio. GitHub is a great platform for this. Include a mix of your own projects and contributions to open-source.

### 5. Study Deep Learning (Optional but Recommended)
- **Frameworks**: Learn a deep learning framework such as TensorFlow or PyTorch. Start with basic neural network concepts and then explore more complex architectures like CNNs (Convolutional Neural Networks) and RNNs (Recurrent Neural Networks).
- **Online Courses and Tutorials**: Leverage online resources, courses (e.g., Coursera, edX, Udacity), and tutorials to understand the intricacies of deep learning models and their applications.

### 6. Soft Skills and Industry Knowledge
- **Problem-Solving**: Sharpen your problem-solving skills. Practice with coding challenges on platforms like LeetCode, HackerRank, or CodeSignal.
- **Version Control**: Become proficient with Git. Understand how to use branches, merges, pull requests, and how to collaborate on projects with others.
- **Stay Informed**: Follow industry trends, read relevant blogs, join Python and machine learning communities, attend webinars, and participate in forums.

### 7. Preparation for Job Applications
- **Resume and LinkedIn**: Update your resume and LinkedIn profile to highlight your Python and machine learning skills, projects, and any relevant courses or certifications.
- **Interview Preparation**: Prepare for technical interviews by reviewing machine learning concepts, practicing coding problems, and preparing to discuss your projects in detail.

This roadmap is a guide to help you focus your learning efforts. The key to making a successful transition is consistency, practical application, and the continuous expansion of your knowledge and skills. Remember, the field of machine learning is vast and constantly evolving, so be prepared for lifelong learning.

----


# Recipe for functional pgm:

To become knowledgeable in #functional programming (FP) without aiming for expert-level depth is a great way to broaden your programming skills and enhance your understanding of various programming paradigms. Here’s a structured recipe to help you get more acquainted with functional programming, including suggested resources, platforms for practice, and key concepts that are particularly beneficial in industry settings. #functionalprogramming
   #career.  #skills
### Step 1: Understand the Core Concepts

Start by familiarizing yourself with the core principles of functional programming:
- **Immutability**: Data objects are not allowed to be modified after they are created.
- **First-Class and Higher-Order Functions**: Functions are treated as first-class citizens, meaning they can be assigned to variables, passed as arguments, and returned from other functions.
- **Pure Functions**: Functions that have no side effects (i.e., do not alter any state outside their scope) and return the same output for the same input.
- **Recursion**: Many functional languages rely on recursion as the primary mechanism for repetition, instead of traditional looping techniques.
- **Functional Data Structures**: Understanding persistent and immutable data structures.

### Step 2: Learn Through Online Courses

There are many free and paid online courses that can provide a structured and comprehensive introduction to functional programming:

- **Coursera**: Offers courses like "Functional Programming Principles in Scala" by École Polytechnique Fédérale de Lausanne. While it uses Scala, the principles are applicable across all functional languages.
- **edX**: Look for "Introduction to Functional Programming" which historically has been offered by institutions like Delft University of Technology and covers functional programming in Haskell.

### Step 3: Read Books and Articles

Several books can provide in-depth knowledge and are often recommended within the functional programming community:
- **"Structure and Interpretation of Computer Programs"** by Harold Abelson and Gerald Jay Sussman (uses Scheme, a dialect of Lisp, and is available online for free).
- **"Learn You a Haskell for Great Good!"** by Miran Lipovača (a beginner-friendly introduction to Haskell, available for free online).
- **"Real World Haskell"** by Bryan O'Sullivan, Don Stewart, and John Goerzen.

Additionally, reading blogs and articles can keep you updated on the latest trends and discussions in the FP community.

### Step 4: Practice Coding

To solidify your knowledge, practice is crucial. Here are a few platforms where you can practice functional programming:
- **Exercism**: Offers mentoring and practice exercises in many languages, including functional languages like Haskell and Elixir.
- **HackerRank and LeetCode**: While these platforms are not specific to functional programming, they offer problems that can be solved using functional approaches in languages like Python.
- **Codewars**: Provides many exercises that can be approached from a functional programming perspective.

### Step 5: Apply FP Concepts in Industry-Relevant Projects

Look for opportunities to apply functional programming concepts in your work or personal projects. Even in languages that are not purely functional like Python or JavaScript, you can apply functional programming principles to write cleaner, more robust code. For example:
- Use Python’s `map`, `filter`, `reduce`, and lambda functions to process data functionally.
- Explore libraries and frameworks in your language of choice that encourage functional programming, like Lodash for JavaScript.

### Step 6: Join Communities

Engage with the functional programming community:
- **Online forums**: Such as the Functional Programming subreddit or Haskell and Scala communities.
- **Meetups and Conferences**: Like LambdaConf in the USA and Functional Conf in Asia.

### Conclusion

By following this structured approach—starting with foundational concepts, progressing through structured learning via courses, deepening knowledge with books, practicing coding problems, applying FP principles in real-world scenarios, and engaging with the community—you’ll gain a solid understanding of functional programming that distinguishes you from the general public. This will not only improve your coding skills but also expand your approach to problem-solving in programming.

-----

# ssh-keygen:
[aghosal@lxplus714 ~]$ ssh-keygen
Generating public/private rsa key pair.
Enter file in which to save the key (/afs/cern.ch/user/a/aghosal/.ssh/id_rsa):
/afs/cern.ch/user/a/aghosal/.ssh/id_rsa already exists.
Overwrite (y/n)? y
Enter passphrase (empty for no passphrase):
Enter same passphrase again:
Your identification has been saved in /afs/cern.ch/user/a/aghosal/.ssh/id_rsa.
Your public key has been saved in /afs/cern.ch/user/a/aghosal/.ssh/id_rsa.pub.
The key fingerprint is:
SHA256:2uxnVjVMFfndX9BPP43xZwFcRNDUodMYZHgWiL2hv6o aghosal@lxplus714.cern.ch
The key's randomart image is:
+---[RSA 2048]----+
|          o =BXX*|
|         . =.+O++|
|          . =* BO|
|         . .  *.%|
|        S .  . o=|
|       +   ..   .|
|      . o  ..    |
|       .  +.     |
|       Eo=.      |
+----[SHA256]-----+
[aghosal@lxplus714 ~]$ cat .ssh/id_rsa
id_rsa      id_rsa.pub
[aghosal@lxplus714 ~]$ cat .ssh/id_rsa.pub
ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQC7SgsQYnJ6yr/Vs75wg9SDjT6Y78fotUxpNuKb4UibyT3uNYGsAP6bY0q6ERCyrXnV22X9LkHuhCjP/czfSUFlV4wxJlisvhgVxMclDJ2XYqY9LRusJdUChHihVctyIl+GAapT4wt2FBUYqS7RAJAzll9P9S/3NG730YUdpFSzHDFfkAjCz/TrBgQ0v5XTc3dP1B4OYN4DzplAQS0jB24QRQkhunhqLNCCGqpqLuOa8+OHF0JK1dUP/dxxHxdAA+jXfSYLTVmmYD1O55NMy+qPMgKAOsh+ZyfqBXzABk5VM42DDqBA34ZuqvD1Sg0GMeiPvu81bEaUbBXR4xjG6ws3 aghosal@lxplus714.cern.ch
[aghosal@lxplus714 ~]$ logout
Connection to lxplus7.cern.ch closed.
>
>
then add it to gitlab or wherever.
>
>
-----
