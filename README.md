# CS300_Analysis-and-Design
Portfolio repository for CS300 from SNHU

**What was the problem you were solving in the projects for this course?**

The problem I was solving was how to design and implement an efficient advising assistance program that allows academic advisors at ABCU to load course data from a CSV file, validate prerequisite relationships, search for individual courses, and display all courses in alphanumeric order. The key challenge was selecting and implementing an appropriate data structure that could support fast searching, scalable validation of prerequisites, and ordered output as the dataset grows. In Project One, the focus was on analyzing multiple data structures (vector, hash table, and binary search tree) to determine which best met the advisor’s requirements. In Project Two, the goal was to translate that design decision into a fully functioning C++ program that advisors could realistically use.


**How did you approach the problem? Consider why data structures are important to understand.**

I approached the problem by first breaking down the functional requirements of the advising system: loading course data, validating prerequisites, searching for a specific course, and printing all courses in alphanumeric order. From there, I evaluated how different data structures would perform when handling these tasks. Understanding data structures was critical because each structure directly impacts runtime efficiency, scalability, and code complexity. In Project One, I implemented pseudocode and runtime analyses for vectors, hash tables, and binary search trees. This comparison showed that while vectors are simple, they scale poorly due to linear searches, and hash tables—while fast for lookup—do not naturally support ordered output without additional logic. The binary search tree, however, naturally maintains order and supports efficient searching through traversal. Based on this analysis, I selected a binary search tree as the most appropriate structure and used it as the foundation for the final implementation in Project Two.


**How did you overcome any roadblocks you encountered while going through the activities or project?**

One major roadblock was ensuring that prerequisite validation and course searching were both efficient and reliable. Early designs using vectors required repeated linear searches, which quickly became inefficient as the number of courses increased. This was resolved by switching to more appropriate data structures and carefully analyzing their runtime behavior. Another challenge was translating pseudocode logic into working C++ code while managing memory correctly. Implementing a binary search tree required careful handling of pointers, node insertion, traversal, and cleanup through destructors. I overcame this by breaking the implementation into smaller, well-defined methods (such as insert, Search, and inOrder) and thoroughly testing each component independently before integrating them into the menu-driven program. Input validation and file handling also presented challenges, which I addressed by adding error checking, user prompts, and defensive programming techniques.


**How has your work on this project expanded your approach to designing software and developing programs?**

This project significantly expanded my approach to software design by reinforcing the importance of planning before coding. By analyzing data structures and runtimes in Project One, I was able to make informed design decisions that directly improved the quality of the final program in Project Two. I also gained a deeper appreciation for separating concerns such as keeping data storage logic, file parsing, traversal, and user interaction distinct. This made the program easier to debug, extend, and reason about. Additionally, designing the software with a real user (academic advisors) in mind helped me focus on usability, clear output, and predictable behavior rather than just technical correctness.


**How has your work on this project evolved the way you write programs that are maintainable, readable, and adaptable?**

Working on this project has improved how I write maintainable and readable code by encouraging consistent naming conventions, clear function responsibilities, and meaningful comments. In Project Two, the use of a dedicated BinarySearchTree class allowed the core data structure logic to remain isolated from the menu and user interface code, making future changes easier. The program is also adaptable because the binary search tree naturally supports scalable growth in the number of courses without requiring major changes to the logic. Additional features—such as removing courses, adding new traversal methods, or expanding validation—could be implemented with minimal disruption to the existing code. Overall, this project reinforced the value of thoughtful data structure selection, modular design, and writing code that can evolve as requirements change. It demonstrated how strong foundational planning can lead to cleaner, more efficient, and more professional software.
