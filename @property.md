[[@property]] = Decorator used to define a method as a property (it can be accessed like an attribute)

Benefit: Add additional logic when read, write, or delete attributes 
Gives you getter, setter, and deleter method

Ex:
 `Class Rectangle:`
	 `def __init__ (self, width, height):`
		 `self.width = width`
		 `self._height = height`
	
	@property`
	`def width(self):`
		`return f"{self._widht:1f}cm"`
	
	`@property`
	`def height(self):`
		`return f"{self._height:1f}cm"`

	`@width.setter`
	`def width(self,nw_width):`
		`if nw_width > 0:`
			`self._width = nw_width`
		`else:`
			`print("width must be greater than zero")`

	`@width.setter`
	`def height(self,nw_width):`
		`if nw_width > 0:`
			`self._height = nw_width`
		`else:`
			`print("height must be greater than zero")`
	
	@width.deleter
	def width(self):
		del self._width
		print("width has been deleted")

	@width.deleter
	def height(self):
		del self._height
		print("height has been deleted")
			
`rectangle = Rectangle(3, 4)`

`*to set/modify the attributes*`
`rectangle.width = 5`
`rectangle.height = 6`

`*to use deleter we use del keyword*`
`del rectangle.width`
`del rectangle.height `

*to get the object from property*
`print(rectangle.width)`
`print(rectangle.height)`
