This section will likely be expanded to include other topics.

## MITRE ATT&CK

This section covers notes from [TryHackMe's MITRE](https://tryhackme.com/room/mitre) room. The main terminology used by MITRE and other threat intelligence frameworks revolves around defining what an APT is. An **Advanced Persistent Threat** is any organized threat group or nation-state that is capable of sustained attacks. The main method of identifying the different APTs lies in unwrapping their TTPS. **Tactics, Techniques, and Procedures** are defined as the adversary's goal, how their goal is achieved, and how the technique is executed. 

[MITRE ATT&CK](https://attack.mitre.org/) is a knowledge base of tactics based on their real-world work. It has been updated to include macOS and Linux techniques. There are currently 14 tactics used by adversaries. Each tactic has its own techniques that adversaries use to achieve it. Each technique has sub-techniques, procedure examples, data sources to search for it, mitigations, and detection tips. 

## MITRE CAR

The MITRE Cyber Analytics Repository holds analytics derived from MITRE ATT&CK. CAR provides pseudocode for each "data model" it holds. These pseudocode formats can be in Logpoint, Splunk, or other formats. Overall, CAR helps operators find analytics to detect techniques defined in ATT&CK. 

## MITRE SHIELD

MITRE SHIELD is an active defense knowledge base. It is designed to provides tactics and techniques for engaging with an adversary that is within a network. A common example of this is the honeypot (or honeyfile) that no user would normally visit unless they had malicious intentions. By interacting with that trap, the defenders are now alerted to an adversary within their network. Like how adversaries use TTPs, defenders have Opportunities, Use Cases, and Procedures. 
