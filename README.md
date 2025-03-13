# MarvelmindModularization
**The goal of this project is to create a modular function for all useful Marvelmind testing and querying functions.** Throughout the Spring 2025 semester as part of the Cornell Aerospace Adversary lab, the group has worked on developing an indoor GPS tracking system using the Marvelmind Indoor Navigation System. The system is created out of <ins>Four-Stationary Beacons</ins> that were setup on the walls of the lab, such that they had an accurate view of each other (free of obstructions); <ins>One-Hedgehog Beacon</ins> (a stationary beacon with the hedge-hog mode turned on, such that it is being tracked via ultrasounds from the four stationary beacons); a <ins>modem</ins> (plugged into the port, such that it streams the data from the hedgehog). The stationary beacons were setup on the walls and flahsed (with the IA software) using the documentation from https://www.youtube.com/watch?v=Uj2_BGS1AjI and https://docs.fictionlab.pl/leo-rover/integrations/positioning-systems/marvelmind-rtls. Submaps were created (following the fictionlab documentation) such that the beacons made a rough outline of the testing room. After the beacons were setup, preliminary testing was conducting; there were slight issues with line-of-sight which were fixed with moving the beacons into better "sight" of each other. After the accuracy was improved, the group tried to query positional data using ROS 2 following https://marvelmind.com/downloads/marvelmind_ROS2.pdf, however, there were technical difficulties and the group switched to querying using Marvelmind's own class: https://github.com/MarvelmindRobotics/marvelmind.py. 

**Next Steps:**
The next steps of this project are to further test the accuracy of the system (intending to converge towards an accuracy of +/- 2cm) and then implement manuevers. After the accuracy is adequate and the group feels confident with how well the system is tracking the positional data, the goal is to implement anti-adversarial cybersecurity manuevers, such that previously developed (state-of-the-art) software can be tested in vitro, rather than relying on satellite simulations or expensive real-world satellites.
