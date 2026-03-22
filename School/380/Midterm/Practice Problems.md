> [!fit] Title
> [[Study Guide|Study Guide]]

---

# 1.
## a) Develop a complete use case (text)
> Develop a complete use case (text) for “I as a borrower should be able to borrow a book from the CSUN library via online library management”. You must present your solution in the exact format of the use case template discussed in class. Note that this problem does not ask you to draw the UML use case diagram. Only give use case (text).

- Use case name: BorrowBookOnline
- Primary actor: Borrower
- Goal in context: Borrow book
- Preconditions: There are books listed, borrower has internet & access to system site
- Trigger: Borrower clicks button to borrow book
- Scenario (briefly explain)
	1. Borrower clicks button to checkout book
	2. Login to account if not logged in
	3. Specify how long to checkout (optional)
- Exceptions (briefly explain)
	1. Book not available: System displays message when available next, borrower checks box to be notified when available if desired 
	2. Borrower has no account: Sign up or register student account
	3. Library database unavailable: Display error and prompt borrower to try again later
	4. Borrower reached checkout limit: Display error, prompt to return books
- Priority: Very high, essential for schools
- When available: First increment
- Frequency of use: Many times per hour
- Channel to actor: Website portal
- Secondary actors: Librarian
- Channel to secondary actors: Website admin panel, physical database server
- Open issues (if any):
	1. Student graduates with checked out books
	2. Checkout limit reached

## b) Consider a simple Library Management System described below:
-  The library system must keep track of when books are borrowed and returned.
-  The system must support librarian work - keeping track of book borrowing and return.
-  The library is open to university staff and students.
-  University staff can borrow books.
-  Students can borrow books.
Design a UML use case diagram, identify all actors. Show all actors (stick figures), the system, use cases or services that the system knows how to perform, and interaction/ relationship between elements. Add sub-diagrams as necessary to show more details.

![[C380TestPractice1.png]]
