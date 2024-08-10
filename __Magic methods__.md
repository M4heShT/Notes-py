[[__Magic methods__]]= Dünder methods (double underscore) __init__, __str__, __eq__ 
They are automatically called by many of Python's built-in operations. 
They allow developers to define or customize the behavior of objects

Ex:

`class Book: 
	`def __init__(self, title, author): <--- constructor which automatically called` `
		`self.title = title`               `to allocate memory when  new object/instance 
		`self.author = author`                                            `created`
		
	`def __str__(self) :`         <----returns object when called directly 
		`return f"'{self.title}' by {self.author}"`
		
	`def __eq__(self,other):`      <----checks the equal or not
		`return self.title == other.title and self.author == other.author`
		
	`def __lt__(self,other):`  <------checks less than func.
		`return self.num_pages < other.num_pages`
		
	`def __gt__(self,other):`   <------checks greater than func.
		`return self.num_pages > other.num_pages`

	`def __add__(self,other):`   <------adds total no. pages.
		`return f"{self.num_pages + other.num_pages`} pages"

	def __contains__(self,keyword):
		return keyword in self.title or keyword in self.author

	def __getitem__(self,key):
		if key == "title":
			return self.title
		elif key == "author";
			return self.author
		elif key == "num_pages";
			return self.num_pages
		else:
			return f"key :{key} not found"
			
`book1 = Book("Harry Potter...", "J.K. Rowling")` 
`book2 = Book("The Hobbit", "J. R. R. Tolkein")` 
`book3 = Book("The Colour of Magic", "Terry Pratchett") 

`print(book1)`
`print(book1 < book2)`
`print(book1 > book2)`
`print(book1 + book 2)`
`print("Colour" in book3)`
`print(book['title'])`