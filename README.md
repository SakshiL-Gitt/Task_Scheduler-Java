# Task_Scheduler-Java
This Java project implements a Task Scheduler that schedules a set of tasks with given durations, deadlines, and resource constraints while respecting task dependencies. The scheduling algorithm prioritizes tasks based on earliest deadline first and ensures that dependencies are satisfied.
**Features**
•	Uses topological sorting (Kahn's Algorithm) to process tasks in the correct order.
•	Uses a priority queue (earliest deadline first) for scheduling.
•	Allocates resources efficiently to avoid overuse.
•	Ensures that no task exceeds its deadline.
•	Prints the scheduled start time, end time, and resource allocation for each task.
**Prerequisites**
Before running this project, ensure you have:
•	Java JDK (8 or higher) installed → Check using java -version
•	Git installed (if cloning from GitHub)
**Installation & Setup**
🔹 Method 1: Clone the Repository (Recommended)
1.	Open a terminal (Linux/macOS) or Command Prompt (Windows).
2.	Run the following command to clone the repository:
       git clone https://github.com/SakshiL-Gitt/Task_Scheduler-Java
3.	Navigate into the project directory:
      cd Task-Scheduler-Java
🔹 Method 2: Download Files Manually
1.	Go to the GitHub repository.
2.	Click on each .java file, then press the "Download" button.
3.	Save all files in a new local folder (e.g., Java-DSA-Project).
4.	Open Command Prompt/Terminal and navigate to the folder where you saved the files:
      cd path/to/Java-DSA-Project
**How to Run the Project**
🔸 Windows
1.	Open Command Prompt (cmd) and navigate to the project folder:
                       cd path\to\Java-DSA-Project
2.	Compile the Java files:
                     javac *.java
3.	Run the project:
                    java Main
🔸 Linux/macOS
1.	Open a terminal and navigate to the project folder:
                    cd path/to/Java-DSA-Project
2.	Compile:
                     javac *.java
3.	Run:
                     java Main
**Input Format**
The program takes:
1.	A list of tasks with the following attributes:
o	id: Task identifier (e.g., "A", "B").
o	duration: Time required to complete the task.
o	deadline: Maximum allowable time to complete the task.
o	resources: Number of resources needed for the task.
2.	A list of dependencies, specifying which task depends on another.
3.	The total number of available resources.
**📌 Example**
Example Input/Output
**INPUT**
Enter the number of tasks: 4
Enter task details (ID, Duration, Deadline, Resources):
A 4 10 2
B 3 15 1
C 2 8  1
D 5 20 3
Enter the number of dependencies: 2
Enter dependencies in the format A->B:
A->B
C->D
Enter the available resources: 4
**OUTPUT**
Task       StartTime  EndTime    Resources 
C          0          2          1         
A          0          4          2         
B          4          7          1         
D          2          7          3    
**License**
This project is licensed under the MIT License – free to use and modify.

