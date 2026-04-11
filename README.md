# Quizec

[cite_start]**Quizec** is an interactive quiz application developed with **Kotlin** and **Jetpack Compose**[cite: 9]. [cite_start]It integrates **Firebase** for authentication and real-time data storage, providing a dynamic environment for teachers and students to interact through customized quizzes[cite: 9, 10].

---

## 🚀 Features

* [cite_start]**Secure Authentication**: Integrated with **Firebase Authentication** to manage user registration and login securely[cite: 15].
* [cite_start]**Quiz Creation**: Users can define a title and description for their quizzes[cite: 24].
* [cite_start]**Unique Access Codes**: Every quiz automatically generates a **unique 6-digit random code** that serves as an identifier for participants to join[cite: 11, 25].
* **Custom Question Types**: 
    * [cite_start]**P01 (Yes/No)**: Simple questions where the correct answer is selected via a checkbox[cite: 32].
    * [cite_start]**P02 (Multiple Choice)**: Questions with dynamically added options and a selectable correct answer[cite: 33, 34].
* [cite_start]**Real-time Lobby**: A waiting room where players are added to the quiz in real-time using a `SnapshotListener` to ensure the participant list updates instantly[cite: 38, 41].
* [cite_start]**Cloud Storage**: All quizzes, questions, and player data are stored in **Firebase Firestore**[cite: 26, 35, 40].

---

## 🛠️ Tech Stack

* [cite_start]**Language**: Kotlin [cite: 9]
* [cite_start]**UI Framework**: Jetpack Compose [cite: 9]
* [cite_start]**Backend & Auth**: Firebase (Authentication & Firestore) [cite: 9, 15, 26]

---

## 📖 Application Flow

1.  [cite_start]**Entry**: Users can register by providing an email and password or log in to an existing account[cite: 14, 16, 19].
2.  [cite_start]**Creation**: Once authenticated, a user can create a quiz and set its details[cite: 18, 23].
3.  [cite_start]**Setup**: The host adds questions (Yes/No or Multiple Choice) which are associated with the unique quiz code[cite: 29, 31].
4.  [cite_start]**Interaction**: Participants join the lobby using the 6-digit code, and the host manages the players before starting the quiz[cite: 38, 39].

---
[cite_start]*Developed for the **Arquiteturas Móveis** course at **isec**.* [cite: 1, 2]
