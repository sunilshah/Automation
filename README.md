# Automation

## Exploring Human Decision Making

Automation is sometimes seen as replacing humans.  However, in most cases only some elements of tasks performed by humans is replaced.

For example, an autopilot does not replace human pilots in an airplane. It merely makes the task of flying easier for human pilots, still requiring vigilent supervision of potential failure modes of automation. For many more years, this state of partial automation will remain in safety critical tasks.   

Situation is not very different in deremining and adminstering medication to a patient. Whether it is determining insulin dose, or chemotherapy dose,
humans are still involved in the critical decisions, often aided by computers and software.

Therefore, human decision making process under partial automation needs to be examined closely.  In addition, understanding the process of human decision making is important even for human behavior not involving automation per se.  

Here we will explore this topic using Jupyter notebooks and Python for live interaction with the user. I want to systematically explore surprises that occur along the way. In doing so, I want to point out various method pitfalls relating to human decisions. Sometimes, these pitfalls are present in computer automation methods.   

In these examples, I will first describe a problem and the method used commonly. Then I will describe assumptions underlying the method and show that it works as intended when used on a simulation that matches the assumptions. Next I will show what happens when used on a more realitic situation simulated by a more complex model. Granted that reality is always more complex than the simulation, it does show the method problems encountered in practice.    


##  Poor Control Inspite of Perfect Prediction  

It seems logical that if you want to control something, you need to measure it and predict it. 

For example, if you want to achieve a particular health outcome like blood glucose level, measuring it, predicting its response to nutrition, exercise and medication seems sufficient. Once you can predict it well, then achieving your goal of controlling it appears a matter of diligent execution. 

We all know from personal experience, that it is easier said than done. 


Although I describe a dose-response problem, the method pitfalls apply equally well to biological and non-living processes.


