[[Aggregation]] = Represents a relationship where one object (the whole) contains references to one or more INDEPENDENT objects (the parts)

Aggregation = A relationship where one object contains references to other INDEPENDENT objects "has-a" relationship

ex: library has-a relationship with book

`class Library:   <------ independent class`
	`def __init__(self, name):` 
		`self.name = name` 
		`self.books = []`
	`def add_book(self, book):      <------ we add(refernce) book in library`  
		`self.books.append(book)` 
	`def list_books(self):` 
	`return [f"{book.title} by {book.author}" for book in self.books]` 
	
`class Book: <------ independent class`
	`def __init__(self, title, author):` 
		`self.title = title` 
		`self.author = author` 

`library = Library("New York Public Library")`
`book1 = Book("Harry Potter...", "J.K. Rowling")` 
`book2 = Book("The Hobbit", "J. R. R. Tolkein")` 
`book3 = Book("The Colour of Magic", "Terry Pratchett") 

`library.add_book(book1)` 
`library.add_book(book2)` 
`library.add_book(book3)` 

`print(library.name)` 
`for book in library.list_books():`
	`print(book)`