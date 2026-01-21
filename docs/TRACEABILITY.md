# Traceability Matrix – Library Book Management System

This document provides traceability between user stories, implementation code,
unit tests, and Git releases. Traceability ensures that every requirement is
implemented, tested, and delivered in a controlled and verifiable manner.

---

## Why Traceability is Important

Traceability links user requirements to code and tests. It helps ensure that:
- All user stories are implemented.
- Every feature is tested.
- Each sprint deliverable can be verified using Git tags.
- No requirement is missed or partially implemented.

---

## Traceability Table

| User Story ID | User Story Description              | Sprint   | Code Component        | Test Case Name                | Git Tag |
|---------------|-------------------------------------|----------|-----------------------|-------------------------------|---------|
| US-01         | Register new books                  | Sprint-1 | add_book()            | test_add_book_success         | v0.1    |
| US-01         | Prevent duplicate Book ID           | Sprint-1 | add_book()            | test_duplicate_book           | v0.1    |
| US-02         | Borrow an available book            | Sprint-2 | borrow_book()         | test_borrow_book              | v0.2    |
| US-02         | Prevent borrowing borrowed book     | Sprint-2 | borrow_book()         | test_borrow_unavailable       | v0.2    |
| US-02         | Return a borrowed book              | Sprint-2 | return_book()         | test_return_book              | v0.2    |
| US-03         | Generate library status report      | Sprint-3 | generate_report()     | test_report_header            | v0.3    |
| US-03         | Report contains book entries        | Sprint-3 | generate_report()     | test_report_contains_book     | v0.3    |

---

## Explanation

Each user story is mapped to:
- **Sprint** in which it was implemented
- **Code component** responsible for the functionality
- **Unit test** that verifies correct behavior
- **Git tag** that marks the completed sprint release

This traceability matrix demonstrates disciplined Agile development, proper use
of Git branching and tagging, and test-driven verification of requirements.

