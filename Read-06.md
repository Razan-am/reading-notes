# **JAVASCRIPT**

### ***Chapter 3: “Object Literals”***

- WHAT IS AN OBJECT? 

  - So object is a set of variables and functions that are been grouping together to create a model of a something you would recognize from the real world. 
  - If `a variable is part of an object`, it is called a `property`. Properties tell us about the object, such as the name of a hotel or the number of rooms it has.
  - If `a function is part of an object`, it is called a `method`. Methods represent tasks that are associated with the object. 

>Example:
- This object represents a hotel. It has five properties and one method.The object is in curly braces. It is stored in a variable called hotel .

`var hotel = {`

//PROPERTIES

 These are variables

`name :  'Quay';`

`room : 40;`

`booked : 25; `

`gym : true;`

`roomTypes : ['twin' , 'double' , 'suite'];`

//METHOD

This is a function 

`checkAvailability : function (){`

 ` return this.room - this.booked ;` 
  `}`

`};`

>The example above shows how to creat an object by letiral notation (There is a several ways to creat an object)

- `To access the properties` for an object by using the `dot notation . ` and also by using the `[ ] sequar brackets`.

  - To access a property or method of an object by using the name of the object following with a period, then the name of the property or the method you want to access.

  - The `preiod is known as the member operator`. The property or the method on its right is a member of the object on its left. 

>To access the property from the example above:

`var hotelName = hotel.name;`

//or

`var hotelName = hotel ['name'] ;`

//hotel is the object

// name is the property


>To access the method from the example above:

`var roomsFree = hotel.checkAvailability ();`

>Example:

`var hotel = {`

`name: 'Park',`

`rooms: 120,`

`booked : 77,`

`checkAvailabi lity: function() {`

`return this.rooms - this.booked;`
`}`

`} ;` 

`var elName = hotel .name ;` 

`var el Rooms = hote 1 . checkAvai l abi lity();` 

-------------------------------------------------------

### ***Chapter 5: “Document Object Model”***







 