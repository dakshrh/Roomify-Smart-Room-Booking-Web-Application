🏨 Roomify – Smart Room Booking Web Application

Roomify is a full-stack web application designed to manage room bookings efficiently while preventing date collisions.
It offers dynamic pricing based on optional meal selections and uses Firebase as a real-time backend for data integrity.

This project focuses on real-world booking logic, not just UI — ensuring correctness, consistency, and usability.

🔍 Project Overview

Booking systems often fail due to overlapping reservations, inconsistent pricing, or poor confirmation flows.
Roomify solves these problems by enforcing strict date validation, dynamic cost calculation, and controlled booking confirmation.

Flow:
User selects room → Chooses dates → Adds meals → Price updates → Confirms booking → Data stored in Firebase

🚀 Key Features:
🏨 Three types of rooms available for booking

📅 Collision-free date management
Prevents overlapping bookings for the same room

🍽 Optional meal selection
Breakfast
Lunch
Dinner

💰 Dynamic pricing
Automatically recalculated based on room type, duration, and meals

🔐 Booking confirmation
Prompt-based confirmation before final submission

🔄 Auto-reset & navigation
Returns to home page after successful booking

☁️ Firebase-backed persistence
Real-time database ensures data consistency

🛠 Tech Stack:

Frontend
HTML
CSS
JavaScript / React (if applicable)
Backend / Database
Firebase
Real-time Database / Firestore
Handles booking records and availability checks

📁 Project Structure:

Roomify/
├── src/
│   ├── components/
│   ├── pages/
│   └── styles/
├── firebase/
│   └── config.js
├── public/
└── README.md

🧠 Core Booking Logic
🔒 Date Collision Prevention

Before confirming a booking, the system:
Checks existing bookings for the selected room
Ensures no date range overlaps
Booking is blocked if a collision is detected

💰 Pricing Calculation 
Total Price =
(Room Price × Number of Days)
+ Selected Meals Cost
Prices update in real time as meal options are selected or removed.

🧪 Example Booking Scenario
Input	Value
Room Type	Deluxe
Stay Duration	3 Days
Meals Selected	Breakfast + Dinner
Result	Collision-free booking with updated total price

⚠ Challenges Faced & Solutions
1️⃣ Date Collision Handling

Problem:
Ensuring bookings do not overlap for the same room.

Solution:
Implemented date-range comparison logic before allowing confirmation.

2️⃣ Dynamic Pricing with Meal Options

Problem:
Meal selection changed pricing unpredictably.

Solution:
Recalculated total price on every user interaction with meal checkboxes.

3️⃣ Data Consistency in Firebase

Problem:
Risk of inconsistent booking states.

Solution:
Used Firebase’s real-time updates to validate availability before final submission.

4️⃣ User Experience Flow

Problem:
Users could accidentally submit incomplete bookings.

Solution:
Added confirmation prompts and auto-reset navigation after success.

▶ How to Run Locally
npm install
npm start

Or open directly if using static hosting.

📸 Screenshots:

Login Page:
![image](https://github.com/user-attachments/assets/7b861a78-b33e-4475-b453-7f24c52d807e)
Register Page:
![image](https://github.com/user-attachments/assets/547fd55d-b6ee-4994-a042-b7753b389b8b)
Home Page:
![image](https://github.com/user-attachments/assets/1b4d1daa-d46f-4edb-9ed4-fc86a50a8062)
![image](https://github.com/user-attachments/assets/65d8bd16-28ff-445f-9868-d376c8cfad97)
![image](https://github.com/user-attachments/assets/42ab0412-e941-4bd6-be72-17dc5c868f98)
Rooms Page:
![image](https://github.com/user-attachments/assets/5d4bec8c-008a-46dd-8270-94942e67bfb2)
Feedback:
![image](https://github.com/user-attachments/assets/36a3cba8-a3b4-4c5f-b591-7eb509598445)
Room Booking:
![image](https://github.com/user-attachments/assets/f8f7db17-40bc-4caf-9da2-34ccd6fe0bdb)

🚀 Future Enhancements

User authentication

Admin dashboard for room management

Booking history per user

Payment gateway integration

Mobile-responsive UI improvements

👤 Author

Daksh Rathi
AI & ML Enthusiast | Full-Stack Developer
Focused on building real-world, production-grade applications with clean logic and reliable backend systems.

⭐ If you like this project, feel free to star the repository!

