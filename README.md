🏥 Hospital Emergency Queue Management System (Doubly Linked List)
📘 Project Overview

This project models a Hospital Emergency Room (ER) Queue System using a Doubly Linked List in C++.
It manages patients according to their treatment priority, giving preference to critical cases while allowing normal patients to wait in sequence.
The system supports quick insertion and deletion of patients at the beginning, end, or at any specific position in the queue, ensuring smooth and efficient hospital operations.

🎯 Features / Operations
Function	Description
🩺 InsertAtBeginning(patientID)	Adds a critical patient to the front of the queue for immediate treatment.
🚶 InsertAtEnd(patientID)	Adds a regular patient to the end of the list who can wait for their turn.
⚖️ InsertAtPosition(patientID, position)	Inserts a patient at a specific priority-based position within the list.
🏁 DeleteFromBeginning()	Removes the first patient after successful treatment.
⚙️ Data Structure Used

The system is implemented using a Doubly Linked List, where each node contains:

🔢 patientID — Unique ID assigned to each patient

⬅️ prev — Pointer to the previous patient

➡️ next — Pointer to the next patient

This structure enables two-way traversal and allows the system to update the queue efficiently as patients are added or removed.

🧩 Dry Run / Step-by-Step Example

Starting with an empty emergency list, the following operations are performed step by step:

1️⃣ InsertAtEnd(101)
2️⃣ InsertAtEnd(102)
3️⃣ InsertAtBeginning(200) (Critical patient)
4️⃣ InsertAtPosition(150, 2)
5️⃣ DeleteFromBeginning()
6️⃣ InsertAtEnd(300)

✅ Final Output
Property	Value
Head	150
Tail	300
Forward Traversal	150 → 101 → 102 → 300
Backward Traversal	300 → 102 → 101 → 150
🧠 Working Methodology

Initialize an empty queue for ER patients.

Add patients according to their urgency level (critical or normal).

Continuously update head, tail, prev, and next pointers after each modification.

Once treated, remove the patient at the front of the queue.

Maintain proper linkage to avoid broken connections between nodes.

Keep processing dynamically as new patients arrive or are discharged.

💻 Technologies Used
Component	Description
💬 Language	C++
🧱 Data Structure	Doubly Linked List
📚 Conclusion

This project showcases the practical use of a Doubly Linked List for managing an emergency room queue system.
It ensures priority-based treatment, supports real-time updates, and maintains an organized and efficient patient flow — making it suitable for real-world hospital management systems.

👩‍💻 Author

Name: Areeba
