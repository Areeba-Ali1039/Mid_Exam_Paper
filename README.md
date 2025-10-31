🏥 Hospital Emergency Queue Management System (Doubly Linked List)

📘 Project Overview
This project represents a Hospital Emergency Queue Management System developed in C++, utilizing a Doubly Linked List.
It manages patients in the emergency room by their priority level, ensuring that critical patients receive treatment before regular ones.
The program efficiently performs insertions and deletions from any point in the queue, maintaining an organized and real-time patient flow.

🎯 Features / Operations

Function	Description
🩺 insertAtBeginning(patientID)	Adds a critical patient to the start of the list.
🚶 insertAtEnd(patientID)	Adds a regular patient to the end of the list.
⚖️ insertAtPosition(patientID, position)	Inserts a patient at a specific position based on urgency.
🏁 deleteFromBeginning()	Removes the first patient after successful treatment.

⚙️ Data Structure Used
The system is built on a Doubly Linked List, where every node consists of:

🔢 patientID – Unique identification number for each patient.

⬅️ prev – Points to the previous patient in the list.

➡️ next – Points to the next patient in the list.

This allows two-way traversal and makes the process of adding or removing patients smooth and efficient.

🧩 Dry Run / Step-by-Step Example

Operations performed from an empty list:

1️⃣ insertAtEnd(101)
2️⃣ insertAtEnd(102)
3️⃣ insertAtBeginning(200) (Critical patient)
4️⃣ insertAtPosition(150, 2)
5️⃣ deleteFromBeginning()
6️⃣ insertAtEnd(300)

✅ Final Output:

Property	Value
Head	150
Tail	300
Forward Traversal	150 → 101 → 102 → 300
Backward Traversal	300 → 102 → 101 → 150

🧠 Working Methodology

Start with an empty list.

Add patients depending on their priority level (critical or normal).

Continuously update head, tail, prev, and next pointers with every insertion or deletion.

Remove patients from the beginning after treatment.

Maintain a properly linked structure to avoid data loss or corruption.

The process continues dynamically as new patients arrive in the ER.

💻 Technologies Used

Component	Description
💬 Programming Language	C++
🧱 Core Concept	Doubly Linked List

📚 Conclusion
This project highlights how Doubly Linked Lists can be applied to manage real-life hospital emergency queues.
It ensures a priority-based, fair, and systematic treatment process while maintaining efficiency in patient flow management.

👩‍💻 Author
Name: Areeba
