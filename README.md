# Library Management System

A command-line interface (CLI) application built with Python to manage library operations. This system utilizes Object-Oriented Programming (OOP) principles and file handling to track books, issue them to students, and manage returns.

## Project Overview

The Library Management System (LMS) allows a library administrator to keep records of available books and track circulation. It uses a text file to persist the list of book titles and a Python dictionary to manage the runtime status (Available/Issued) of each book.

## Features

- **Display Books:** Lists all books in the library with their unique ID and current status (Available or Issued).
- **Issue Books:** Allows a user to borrow a book. The system records the borrower's name and the date/time of issuance. It prevents issuing a book that is already borrowed.
- **Add Books:** Enables the administrator to add new book titles to the library. These titles are saved permanently to a text file.
- **Return Books:** Processes book returns and updates the status back to 'Available'.
- **Input Validation:** Checks for valid Book IDs and ensures book titles do not exceed character limits.

## Prerequisites

- Python 3.x

## File Structure

- `main.py`: The main Python script containing the LMS class and application logic.
- `library_catalog.txt`: A text file that stores the names of the books (one title per line).

## Installation and Setup

1. Clone this repository or download the source code.

2. Ensure you have a text file named `library_catalog.txt` in the same directory as the script. You can create this file and add some initial book titles manually (one per line).

   Example `library_catalog.txt`:
   ```text
   Python Programming
   Data Structures
   Algorithms
   Operating Systems
   Run the application:

Usage
Once the application is running, follow the on-screen prompts to navigate the system:

Press D to Display Books.

Press I to Issue a Book.

Press A to Add a Book.

Press R to Return a Book.

Press Q to Quit.

Example Workflow
The user presses A to add a new book titled "Machine Learning".

The user presses D to see the new book listed with a generated ID (e.g., 1005).

The user presses I, enters ID "1005" and their name. The book status changes to "Already Issued".

Limitations
Runtime Status: While book titles are saved to the text file, the borrowing status (who borrowed which book) is stored in a temporary dictionary. Closing the program will reset the status of all books to "Available".



