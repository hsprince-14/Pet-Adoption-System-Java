# Pet Adoption System in Java

This repository contains the project files for a simple, console-based Pet Adoption System developed in Java.

## About the Project

This project was created to demonstrate a fundamental understanding of Object-Oriented Programming (OOP) concepts through a practical application. It simulates a real-world pet adoption process where users can log in, browse available pets, and apply for adoption, while an admin manages the listings and applications. The system is designed to promote efficient pet placement and animal welfare.

## Features

The system provides two distinct roles with different permissions, accessible via a secure login.

### Admin (Staff) Role
* **Secure Login:** Access with username `Admin` and password `Admin123`.
* **Add Pets:** Add new dogs or cats to the system. The `addPet` method is overloaded, allowing pets to be added with or without a special note.
* **Manage Applications:** Approve or decline adoption applications submitted by users.
* **View Listings:** View all pets currently in the system and their adoption status.
* **View Applications:** See a list of all submitted adoption applications.

### Customer (Adopter) Role
* **Secure Login:** Access with username `Customer` and password `pet123`.
* **Browse Pets:** View a list of all pets available for adoption.
* **Apply for Adoption:** Submit an application for a specific pet.
* **View Personal Applications:** Check the status of their own submitted applications.

## OOP Concepts Implemented

This project is a practical demonstration of the core principles of OOP:

* **Encapsulation:** User data such as `name` and `password` are kept `private` within the `User` class, with access controlled through public methods. This protects the data and ensures secure login procedures.
* **Inheritance:** The `Adopter` and `Staff` classes are built as subclasses that `extend` the base `User` class, inheriting its properties and methods. Similarly, the `Dog` and `Cat` classes inherit from the abstract `Pet` class.
* **Polymorphism & Overriding:**
    * The abstract method `showInfo()` in the `Pet` class is implemented differently by the `Dog` and `Cat` subclasses to display unique information for each type of pet.
    * The `menu()` method is defined in the abstract `User` class and is overridden by both the `Adopter` and `Staff` classes to display a role-specific menu.
* **Method Overloading:** The `addPet()` method within the `Staff` class is overloaded. One version accepts just the pet's name and type, while another accepts an additional "note".

## Getting Started

Since the source code is provided as a PDF in this repository, you will need to copy the code into a `.java` file to compile and run the application.

### Prerequisites
* Java Development Kit (JDK) installed on your machine.

### How to Run
1.  Open the source code PDF file from this repository.
2.  Copy the entire Java code.
3.  Paste the code into a new file and save it as `PetAdoption.java`.
4.  Open a terminal or command prompt and navigate to the directory where you saved the file.
5.  Compile the code using the Java compiler:
    ```sh
    javac PetAdoption.java
    ```
6.  Run the compiled application:
    ```sh
    java PetAdoption
    ```
7.  The program will start, and you can log in using the credentials below.

### Login Credentials
* **Admin Login:**
    * Name: `Admin`
    * Password: `Admin123`
* **Customer Login:**
    * Name: `Customer`
    * Password: `pet123`
