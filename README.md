# CS-320
Created for the CS-320 Software Test, Automation QA class

OVERVIEW
This artifact comes from CS-320. It includes the Contact, Task and Appointment services with full JUnit 5 test suites, along with my Summary and Reflections report. Together these show practical skills in requirement driven design, unit testing, and test automation. The code enforces clear constraints for each domain object, the services manage add, update, and delete operations, and the test classes validate both happy paths and failure cases.

WHY THIS ARTIFACT MATTERS
THis work shows that I can turn written requirements into code and tests that protect data quality. I used boundary checks, null and length validation, and clear exception messages to make failures obvious. I wrote tests first for several parts, then filled in the implementation, which kept me focused on behavior. I measured coverage and added missing tests when I noticed gaps around edge cases and update guards. The end result is code that is simple to read and easy to change because the tests give fast feedback.

WHAT I IMPROVED FOR THE PORTFOLIO
I cleaned up comments, made exception messages consistent, and added a few missing negative tests for invalid updates. I did not change the design in a way that would hide course intent. I kept the structure familiar so another developer can open the project and run the tests quickly. 

HOW TO BUILD AND RUN THE TESTS  
You can run the tests with Maven or with an IDE. Requirements are Java and Maven if you choose the command line route.

MAVEN
From the project folder run mvn test

IDE 
Import as a Maven project in Eclipse or IntelliJ. Run the test suites from the test package using the JUnit runner.

WHAT THIS DEMONSTRATES
Requirement alignment
Each constraint from the assignment is enforced in the constructors and setters. Tests confirm maximum lengths, non null rules, and that immutable fields do not change after creation.

QUALITY THROUGH AUTOMATION
The test suites cover valid creation, invalid inputs, and service level operations. I used focused test methods with clear names so failures point straight to the problem. I also grouped tests by behavior, which makes it easy to find and extend them.

IMPACT ON MY PROCESS
Writing tests early exposed unclear spots in my assumptions. It pushed me to keep methods small and to return clear errors. I also learned to isolate responsibilities so each class stays simple, which made tests faster and more reliable.

TRANSFER TO OTHER WORK
These practices carry to any project that needs reliable updates. I can stand up a small service, write tests around the edges, and keep making changes with confidence. The same approach fits API endpoints, data validation in forms, or background jobs that touch customer records.

INCLUDED FILES
The src folder contains the Contact, Task, and Appointment services and their tests. The docs folder contains the Summary and Reflections PDF. This README explains the artifact and how to run it.
