## Links:
https://www.inovex.de/de/leistungen/artificial-intelligence/ - for ML related stuffs


[[tutorials]] -> Uproot comes with Scikit-HEP package. Major advantage. - calls compiled vectorized functions to perform very fast calculations on arrays



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

To convert book types, ahve calibre installed first.
$ ebook-convert \*.epub  \*.pdf 

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
