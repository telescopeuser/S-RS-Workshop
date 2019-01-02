<img align="right" src='http://www.aisp.sg/images/APP/ISS.jpg' width=25%>

## Reasoning Systems Workshops & References

**This [Reasoning Systems (RS)](https://www.iss.nus.edu.sg/executive-education/course/detail/reasoning-systems "Reasoning Systems") course is part of the Analytics and Intelligent Systems and Graduate Certificate in [Intelligent Reasoning Systems (IRS)](https://www.iss.nus.edu.sg/stackable-certificate-programmes/intelligent-systems "Intelligent Reasoning Systems") series offered by [NUS-ISS](https://www.iss.nus.edu.sg "Institute of Systems Science, National University of Singapore").**

**Lecturer: [GU Zhan (Sam)](https://www.iss.nus.edu.sg/about-us/staff/detail/201/GU%20Zhan "GU Zhan (Sam)")**

[![alt text](https://www.iss.nus.edu.sg/images/default-source/About-Us/7.6.1-teaching-staff/sam-website.tmb-.png "Let's check Sam' profile page")](https://www.iss.nus.edu.sg/about-us/staff/detail/201/GU%20Zhan)

**zhan.gu@nus.edu.sg**

---
### Open and refer to file: [S-RS Workshop Guide.pdf](https://github.com/IRS-RS/S-RS-Workshop/blob/master/S-RS%20Workshop%20Guide.pdf)
---

Institute of Systems Science

National University of Singapore

GRADUATE CERTIFICATE

INTELLIGENT REASONING SYSTEMS

Workshop Project (Continuous Assessment) Guide

Subject: Reasoning Systems

• Source impactful real life business scenario for workshop project. 

• Conduct comprehensive research and reference reading.

• Make your own reasonable assumptions where necessary.
 

### Workshop 1 Guide


### Workshop 1.1 [ Individual ] 

### Workshop 1.2 [ Individual ] 

Design and draft robot navigation search representation here:


Write down DFS search order:
Write down BFS search order:
Construct reasonable heuristics, then design heuristic search strategy to enhance above DFS/BFS brute force search:


### Workshop 1.3 [ Group ] 

Form groups: 4-6 learners per group.


Design and draft VRP search representation here:
Strategy to avoid looping (revisiting same customer):


### Workshop 1.4 [ Individual ] 

KIE OptaPlanner Tutorial: Installation; KIE Workbench; IDE plug-in; Case Study

Above: OptaPlanner Installation
https://www.optaplanner.org/

Above: Install Eclipse IDE
https://www.eclipse.org/downloads/packages/
 
Above: Install Maven in Eclipse
https://stackoverflow.com/questions/8620127/maven-in-eclipse-step-by-step-installation
 
Above: Install KIE plug-in for Eclipse
https://www.drools.org/download/download.html

Above: Download OptaPlanner source code and example cases
https://github.com/kiegroup/optaplanner

Above: Import OptaPlanner example cases as Maven project in Eclipse

Above: Standalone OptaPlanner

https://www.optaplanner.org/
 
VRP Reference 

• http://www.optaplanner.org/learn/useCases/vehicleRoutingProblem.html

• http://www.optaplanner.org/learn/slides/optaplanner-presentation/index.html#/2

• https://www.optaplanner.org/blog/2015/03/10/VisualizingVehicleRoutingWithLeafletAndGoogleMaps.html
 

### Workshop 2 Guide

Above: Search Algorithms in Action


### Workshop 2.1 [ Individual ] 

Analyze and execute cloud computer balancing system using both Eclipse and KIE Workbench.


Solver in Java / Eclipse


Solver in Java / Eclipse (Web Application on KIE Server)

Above: example web applications

Above: example solution enquiry via RESTful API

Above: example KIE server interaction via RESTful API

Above: example server end point

Reference 

• https://github.com/kiegroup/optaplanner/tree/master/optaplanner-webexamples

• https://docs.optaplanner.org/latest/optaplanner-docs/html_single/index.html#quickStart


Solver in KIE Workbench & Server
 
Above: domain objects based on class diagram
 
Above: constraints using Drools guided rule

Above: constraints using Drools guided rule

Above: solver configuration

Above: solver configuration (xml)

Reference 

• http://www.optaplanner.org/learn/useCases/cloudOptimization.html

• http://www.optaplanner.org/learn/slides/optaplanner-presentation/training.html#/4/26

• https://docs.jboss.org/optaplanner/release/latestFinal/optaplanner-wb-es-docs/html_single/
 

### Workshop 2.2 [ Individual ] 

Choose one use case; propose relevant enhancements; then import, analyze, adapt, enhance, and solve/execute. 

Enhancement example 1: 
Enhance the Cloud Balancing system by introducing a comprehensive user interface for end user to 

1. [ Input ] Key in problem configuration:

a. Computer instances with: cpuPower, memory, networkBandwidth, cost.

b. Process instances with: requiredCpuPower, requiredMemory, and requiredNetworkBandwidth.

2. [ Output ] Display graphical final solution of cloud computer assignments:

a. Hint: reusable Java code from https://github.com/kiegroup/optaplanner/tree/master/optaplanner-examples/src/main/java/org/optaplanner/examples/cloudbalancing

Enhancement example 2: 
Enrich the Cloud Balancing domain model and add extra constraints such as these:

• Each Process belongs to a Service. A computer might crash, so processes running the same service must be assigned to different computers.

• Each Computer is located in a Building. A building might burn down, so processes of the same services should (or must) be assigned to computers in different buildings.

Reference https://docs.optaplanner.org/latest/optaplanner-docs/html_single/index.html#cloudBalancingBeyondThisTutorial

Enhancement example 3: 
Propose and implement/enhance your own relevant business use case.


### Workshop 3 Guide

Refer to workshop by co-lecturer
 

### Workshop 4 Guide

Refer to workshop by co-lecturer


### Workshop 5 Guide


### Workshop 5.1 [ EEP Individual / MTech Group ] 

Identify a relevant business scenario/problem. Propose and create a hybrid reasoning system.
The proposed group workshop project must develop, integrate, and demonstrate at least two out of following three technique groups: 

1. Business rule OR Business process based reasoning techniques 

2. Business resource optimization techniques: Heuristic search OR Constraint satisfaction OR Evolutional computing 

3. Knowledge Discovery OR Data Mining techniques 

The submitted runnable system should have a graphical user interface for end user to input or update data to execute different business scenarios, e.g. to enable initial planning and frequent re-planning/re-optimization. And to display system output results in a user friendly manner. (Input/output using xml file or console log is not considered as user friendly.)
Candidate/Example Project: 

ANNEX 1 WORKSHOP PROJECT CANDIDATE
Project Submission Guideline: 

ANNEX 2 PROJECT CODE EXPORT & IMPORT USING KIE WORKBENCH

ANNEX 3 WORKSHOP PROJECT SUBMISSION

Domain Modelling Reference 

• https://docs.optaplanner.org/latest/optaplanner-docs/html_single/index.html#designPatterns

 

### ANNEX 1 WORKSHOP PROJECT CANDIDATE

### Workshop Project Candidate One

Hybrid Airport Gate Assignment System (HAGAS)

The Airport Gate Assignment Problem: Scheduling Algorithms and Simulation Approach

Ahmed Thanyan AL-Sultan

The rapid development of airlines has made airports busier and more complicated. The assignment of schedule to available gates is a major issue for daily airline operations. We consider the over-constrained airport gate assignment problem (AGAP) where the number of flights exceeds the number of available gates, and where the objectives are to minimize the number of ungated flights and the total walking distance or connection times. The procedures used in this project are to create a mathematical model formulation to identify decision variables to identify, constraints and objective functions. In addition, we will consider in the AGAP the size of each gate in the terminal and also the towing process for the aircraft. We will use a greedy algorithm and a Tabu search meta-heuristic to solve the problem and compare it with other scheduling methods. Actual and forecasted data will be simulated in the experiment. The greedy algorithm minimizes ungated flights while providing initial feasible solutions that allow flexibility in seeking good solutions, especially in case when flight schedules are dense in time. Experiments conducts give good results. The distance a passenger has to walk in any airport to reach various key areas, including departure gates, baggage belts and connecting flights provide for an important performance measure for the quality of any airport. While certain walking distances are fixed, others are dynamic. In particular, the distances traversed by passengers from check-in counters to gates and from gate to gate, in the case of transfer or connecting passengers, change according to how scheduled flights are assigned to gates. This allows for the ground handling agents and airlines, together with airport authorities, to dynamically assign airport gates to scheduled flights so as to minimize walking distances while, consequently, minimizing connection times. Which flight to gate assignment policy to be used so as to achieve such minimum times can be derived at the start of such planning day based on published flights schedules and booked passenger loads. The airport gate assignment problem (AGAP) seeks to find feasible flight to gate assignments so that total passenger connection times and walking distances is minimized. Distances that are taken into account are those from check-in to gates in the case of embarking or originating passengers, from gates to baggage claim areas (check-out) in the case of disembarking or destination passengers and from gate to gate in the case of transfer or connecting passengers. In the over-constrained case, where the number of aircraft exceeds the number of available gates, we include the distance from the apron or tarmac area to the terminal for aircraft assigned to these areas. 
…

Reference

The Airport Gate Assignment Problem: Scheduling Algorithms and Simulation Approach, Ahmed Thanyan AL-Sultan, Graduate School of environmental science, March 2012

http://ousar.lib.okayama-u.ac.jp/files/public/4/48534/20160528091554614463/K0004584_honbun.pdf
 

### Workshop Project Candidate Two

OptaPlanner Application Implementation in KIE Workbench & Server

Objective:

Construct a useful business reasoning system using KIE product suite, incorporating an OptaPlanner solver as an embedded optimization engine/task for automated machine reasoning.
Choose one OptaPlanner example application from below ONLY:

• Cloud balancing

• Course timetabling

• Vehicle routing with time windows

• Project job scheduling

• Exam timetabling

• Nurse rostering

• Cheap time scheduling

• Flight crew scheduling

System Requirements:

• Make use of KIE BRMS (Drools) & BPMS (jBPM) capability;

• Define at least one practical business enhancement/requirement based on OptaPlanner example;

• Convert/migrate original Maven/Eclipse OptaPlanner project with enhancements into KIE (jBPM) Workbench project;

• Develop a (web-based) User Interface;

• Deploy the developed system onto KIE Server for use;


### ANNEX 2 PROJECT CODE EXPORT & IMPORT USING KIE WORKBENCH
Example: export KIE project Mortgage_Process_ISS_MR from work space MySpace
Review project settings to obtain project URL


Export project from KIE Workbench

1. Select a folder for exporting, example here uses /home/iss-user/iss-vm-program/is-intelligent-reasoning-systems/jboss/project-io

2. Start a Terminal there, key in command git clone ssh://wbadmin@localhost:8001/MySpace/Mortgage_Process_ISS_MR

3. Key in password ‘wbadmin’ for user wbadmin


Import project into KIE Workbench

1. In KIE workbench, select/create a project Space, example here uses ISS-MR

2. Click menu function ‘Import Project’

3. For Repository URL, key in file:///home/iss-user/iss-vm-program/is-intelligent-reasoning-systems/jboss/project-io/Mortgage_Process_ISS_MR

Reference

• https://developer.jboss.org/thread/269991

• https://developer.jboss.org/thread/237411

• https://developer.jboss.org/thread/252588


### ANNEX 3 WORKSHOP PROJECT SUBMISSION

Submission due by 23:59 on last lecture date (+ 14)
One delayed day = 10 marks deduction

1. [MTech & EEP] Create Github repository for project submission
2. [MTech] Download Github repository as a ZIP file, then upload to NUS LumiNUS / IVLE

Reference https://github.com/IRS-PM/Workshop-Project-Submission-Template


### ANNEX 4 KIE OptaPlanner Examples

Reference

• https://docs.optaplanner.org/latest/optaplanner-docs/html_single/index.html#useCasesAndExamples

Link https://www.guidedchoice.com/video/dr-harry-markowitz-father-of-modern-portfolio-theory/


### The End of Workshop Project Guide
