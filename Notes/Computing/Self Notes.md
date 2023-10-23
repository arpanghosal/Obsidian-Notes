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

