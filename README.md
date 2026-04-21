# Quizec

**Quizec** is an interactive quiz application developed with **Kotlin** and **Jetpack Compose**. It integrates **Firebase** for authentication and real-time data storage, providing a dynamic environment for teachers and students to interact through customized quizzes

---

## 🚀 Features

* **Secure Authentication**: Integrated with **Firebase Authentication** to manage user registration and login securely.
* **Quiz Creation**: Users can define a title and description for their quizzes.
* **Unique Access Codes**: Every quiz automatically generates a **unique 6-digit random code** that serves as an identifier for participants to join.
* **Custom Question Types**: 
    * **P01 (Yes/No)**: Simple questions where the correct answer is selected via a checkbox.
    * **P02 (Multiple Choice)**: Questions with dynamically added options and a selectable correct answer.
* **Real-time Lobby**: A waiting room where players are added to the quiz in real-time using a `SnapshotListener` to ensure the participant list updates instantly.
* **Cloud Storage**: All quizzes, questions, and player data are stored in **Firebase Firestore**.

---

## 🛠️ Tech Stack

* **Language**: Kotlin 
* **UI Framework**: Jetpack Compose 
* **Backend & Auth**: Firebase (Authentication & Firestore) 

---

## 📖 Application Flow

1.  **Entry**: Users can register by providing an email and password or log in to an existing account.
2.  **Creation**: Once authenticated, a user can create a quiz and set its details.
3.  **Setup**: The host adds questions (Yes/No or Multiple Choice) which are associated with the unique quiz code.
4.  **Interaction**: Participants join the lobby using the 6-digit code, and the host manages the players before starting the quiz.

---
*Developed for the **Arquiteturas Móveis** course at **isec**.
