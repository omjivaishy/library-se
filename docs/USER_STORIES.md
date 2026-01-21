# User Stories – Library Book Management System

This document describes the user stories for the Library Book Management System developed
using Agile methodology. User stories capture the system requirements from the end user’s
perspective and guide sprint-wise development.

---

## User Story 1: Book Registration

**As a librarian**,  
I want to add new books to the library system using a unique Book ID, title, and author,  
so that books can be stored and managed properly in the library.

### Acceptance Criteria:
- The system must allow adding a book with Book ID, Title, and Author.
- Each Book ID must be unique.
- If a duplicate Book ID is entered, the system must reject it with an error.

This user story was implemented in **Sprint-1**. It forms the foundation of the system
because all other features depend on having books registered first.

---

## User Story 2: Borrow and Return Book

**As a librarian**,  
I want to borrow a book and return a book,  
so that the availability status of books is accurately maintained.

### Acceptance Criteria:
- A book can be borrowed only if it is available.
- Borrowing an already borrowed book must raise an error.
- Returning a book must update its status back to available.

This user story was implemented in **Sprint-2**. It introduces business rules and state
management by tracking whether a book is available or borrowed.

---

## User Story 3: Library Status Report

**As a librarian**,  
I want to generate a report of all books in the library,  
so that I can view book details and their current status.

### Acceptance Criteria:
- The report must include Book ID, Title, Author, and Status.
- The report must contain a header row.
- The report must list all books currently stored in the system.

This user story was implemented in **Sprint-3**. It focuses on reporting and visibility
of system data rather than modifying it.

---

## Summary

These user stories were implemented incrementally across three sprints following Agile
principles. Each story was translated into code, verified using unit tests, and tracked
using Git branches and tags.

