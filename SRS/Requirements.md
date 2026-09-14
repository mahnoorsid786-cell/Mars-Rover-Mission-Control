Mars Rover Mission Control-Requirements

# Functional Requirements 

 FR-01 (Listen & Move): The rover must obey valid movement orders sent from Earth, such as driving forward, turning, or stopping.
 FR-02 (Report Martian Conditions): The rover must send regular telemetry updates showing where it is, how much battery remains, its current temperature, and whether its antenna link is active.
 FR-03 (Block Faulty Messages): The software must check every incoming packet and reject commands that are corrupted, unreadable, or sent without permission.
 FR-04 (Enter Safe Mode on Crisis): If internal heat rises too high or power drops below critical levels, the rover must instantly shut down non-essential systems to protect itself.
 FR-05 (Acknowledge Actions): After trying an assigned task, the rover must transmit a return receipt confirming whether the task succeeded or failed.
 FR-06 (Track Operator History): The system must save a permanent mission log recording every instruction issued, every critical error, the responsible user ID, and the exact timestamp.

# Non-functional Requirements 

 NFR-01 (Reaction Speed): The rover must parse and begin processing any received command within 5 seconds of arrival on Mars.
 NFR-02 (Access Control): Only recognized, logged-in mission operators with proper clearance may transmit instructions to the rover.
 NFR-03 (Connection Resilience): The rover must remain stable, retain stored data, and run background essentials even if the radio link drops out for hours.
 NFR-04 (Multi-Rover Capacity): Mission Control servers must easily manage communication lines and health streams for up to 20 rovers at once.
