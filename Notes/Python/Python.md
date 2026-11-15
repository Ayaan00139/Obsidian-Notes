# Install Any Package-> ~/.my_env/bin/pip install cowsay
*this is specially for arch cause pip tends to break the os*

# Run Python files with Packages-> ~/.my_env/bin/python say.py Ayaan
*this is specially for arch cause pip tends to break the os*


![[Pasted image 20261106004329.png]]
1. We can edit print function in many ways, check python document for more ways you can edit
2. .strip() removes spaces in a string
3. print(f"{z:,}") is to print with commas like 1,000 like `:,` is used to do it 
4. print(f"{z:.2f}") to round the digits i want to print
5. def is used to create function- "define"

	 6.- This Is How We Make Functions:
	 
	def main():
	name = input("Whats Your Name? ")
	hello(name)
	
	def hello(to="world"):
	print("hello,", to)
	  
	main()


	7.- x=float(input("Whats x? "))
	y=float(input("Whats y? "))
	z=x/y
	print(f"{z:.2f}")
	

8.  We can use literal "Or" for || in if statements

	![[Pasted image 20261105023257.png]]
9. We can use Literal "AND" for && in if


10.- 
These 2 are the same thing and only python allows this and can chain them together

![[Pasted image 20261105023626.png]]          ![[Pasted image 20261105023634.png]]


11.
![[Pasted image 20261105025445.png]]

12.

![[Pasted image 20261105025558.png]]                      ![[Pasted image 20261105030152.png]]

this and this is the same thing just using match

13.
Loops:
	![[Pasted image 20261106005023.png]]     Name the variable "_" so cause its a global name which specifies that we care about this variable this and is only for the loop


14.   ![[Pasted image 20261106005205.png]]  we can also use thissssss, and its pythonic and is only available in python

15. ![[Pasted image 20261106011226.png]]



16. ![[Pasted image 20261106011328.png]]



17. ![[Pasted image 20261106011648.png]]

18. Range Basically Creates a list of the number passed as argument in that so if we do range(4) itll create list of 4 things

![[Pasted image 20261106012018.png]]


19. Dictionaries:Here just because this student will print the keys of the dictionary, it is possible to extract value using students, for context, see point 20

	![[Pasted image 20261106013149.png]]          ![[Pasted image 20261106013722.png]]          ![[Pasted image 20261106013734.png]]                            


20. when we print a position of a dictionary, we get its keys

	   ![[Pasted image 20261106013454.png]]                               ![[Pasted image 20261106013508.png]]


21. If in dictionary there are multiple things but not only key value pair, we'll set it like multiple dictionary in lists like this, so for hermione, it'll be a list which has 3 dictionary for name, house and patronus, just like the image

	![[Pasted image 20261106014633.png|986]]

	and to print all, we use 
		![[Pasted image 20261106020136.png|636]]

22. Square:
	![[Pasted image 20261106021711.png|425]]

23.- 
Here is have gotten an error sayign ValueError cat cant be passed in int cause it is not an integer, so we'll use try except in this case and write "ValueError" in except so it only executes when the error is related to the ValueError, but yeah if we only do except: it'll catch everything but it'll also hide bugs in the codes so its a bad practice dont use it....

![[Pasted image 20261106030757.png|577]]       ![[Pasted image 20261106030828.png|389]]

24. In python its a good and recommended practice to keep only the lines which can generate a error in try except and no extra line should be there
		![[Pasted image 20261106031559.png|313]]
		
	but now in this case there is a name error cause when we input string and it goes to int function , i does not return anything hence x does not get defined hence its name error and becuase there is no else except cant simply do nthg and will just print x is not an integer and cause print is in a common place (c termalogy) it will still get executed so a name error

	   ![[Pasted image 20261106031705.png|558]]

	so to solve this we use try except else like in the image, python will tey to execute line 2, if something goes wrong it will run line 3,4 and if everything is right itll run line 6 
	             ![[Pasted image 20261106031859.png|492]]

	same thing in a loop
	                  ![[Pasted image 20261106033417.png|503]]

25. with try except we also have pass, it is used to just ignore the error and retry the try or eg. ie. there is no error msg but just try repeatedly till there is no error

	   ![[Pasted image 20261106034353.png|446]]

26. Random Library:

	   ![[Pasted image 20261106175548.png|554]]


27. **Command Line Argument**
		Here sys.argv return a list which consist of all the words i typed after "python" in the terminal to run it
	   ![[Pasted image 20261107000258.png|456]]

28. Index error:

	![[Pasted image 20261107000719.png|717]]          ![[Pasted image 20261107001649.png|406]]

29. We Use Sys.exit imported from sys to exit a conditional and not run the common place argument

# IMP!!! ->

29. So this "1:" will give me a slice of the list containing every element of list except the first one in this case, the name.py one, ==🔴**IMP!!**== and we can also use it like in other image, with [:-1] we can slice the last element
	   ![[Pasted image 20261107003601.png|485]]    ![[Pasted image 20261107003813.png|496]]


30. Requests is a package manager that allows us to connect to some apis and acts as a browser, it means that we can connect to apis like a browser and act as a browser and download or access those get and post requests. 


### Here we got a json document which has info about Artic Monkey artist which we get from itunes website by hitting the api, if we hit in browser, we get the same result and a txt doc is automatically downloaded. We got a dictionary in which we have a list which has another dictionary. 

   ![[Pasted image 20261107012040.png|1003]]

### we can use another lib named Json which will pretty print this data in a formated way
   
   ![[Pasted image 20261107012529.png|696]]
   
#   This will give me every song of the artist we type in after the name of the file in command line

   ![[Pasted image 20261107014429.png|677]]



31. To import functions created by us we have to use from, import like in the image //"Hello Is a function in savings.py". IMP!! but when running and import we cant leave functions in the file we imported running cause when imported whole file comes to memory and if in this case sayings.py has main() which is executing hello and goodbye, while import these 2 will run automatically

	   ![[Pasted image 20261107015154.png]]                          ![[Pasted image 20261107020150.png|285]]              ![[Pasted image 20261107015450.png]]                    


to fix this, we add this condition near main. and it works cause it is a special feature by python which will set `__name__` to `__main__` when and only when the file is executed and not imported

![[Pasted image 20261107015721.png|398]]     ->   ![[Pasted image 20261107020110.png|331]]   ->   ![[Pasted image 20261107020119.png]]                                 


32.  We use assert keyword to assert/claim something and it will pass with no error if it is try but if it is false, itll give assertion error

   ![[Pasted image 20261107024110.png]]

33.  we can also use raises which will pass if the terminal gives exact error which is obtained then in this case square("cat") is executed...
				![[Pasted image 20261107031549.png]]

34. we can use a package by pip called pytest to check our functions, it basically checks all functions in a file and gives you a report 

	   ![[Pasted image 20261107032908.png|1146]]


35. ### Write File-> We can write files with open like shown in image, we can use with so we dont have to close file everytime, and if we dont close everytime our file may corrupt

	   ![[Pasted image 20261107061142.png|746]]       ![[Pasted image 20261107061447.png]]

36. ### Read File-> when we open a file, we dont have to write "r" to read cause its default

   ![[Pasted image 20261107062044.png|603]]         ![[Pasted image 20261107062124.png|658]]

37. To store multiple info about one thing we use .csv instead of txt, also if there is 2 words after end of the comma, itll be considered a single string and would be complied normally

	![[Pasted image 20261107063217.png]]      ![[Pasted image 20261107063900.png|535]]

38. Ok so in sorted function we can pass a function as a key which will further sort on the basis of the value of the key like in the image it sorts on the basis of every name 

	   ![[Pasted image 20261107065514.png]]

#    To make our life easier, we have a csv lib which take care of everything, sample in image, also here lambda is a one liner function describing what student is... `lambda` is just a concise way to build a throwaway helper function right inside the line of code where you need it.

   ![[Pasted image 20261107072112.png]]

   like csv reader we have csv DictReader which will first check the first row of csv to check the format of data and then format the data accordingly 

   ![[Pasted image 20261107072808.png]]


#    Similarly to write with csv we do like the image suggests ->

   ![[Pasted image 20261107073616.png]]                 -> -> ->              ![[Pasted image 20261107073644.png]]

like csv writer we have csv DictWriter which will write the data as dictionaries and we also have a second argument to pass besides fields

![[Pasted image 20261107074247.png]]    ->->->   ![[Pasted image 20261107074306.png]]


# we can create a gif like this ->

![[Pasted image 20261107080831.png]]


# Using RE-> re.search( pattern, string, flags=0 )

# 39. 

## To Tend To Check Or Validate Something like A email   -> 

   ![[Pasted image 20261107230803.png|330]]  
###### like in this image, it checks for the basics but first we wrote this much lines of code for something rather simple and second it doesnt event cover all the narrow cases, so to fix/improve this we tend to use a library of python- "RE" as in regular expressions

we can create our own regex by this chart and then move forward like this image

![[Pasted image 20261107232121.png|493]]  -> -> -> ->  ![[Pasted image 20261107234410.png]]

![[Pasted image 20261108001150.png|409]]    -> -> -> ->   ![[Pasted image 20261108000223.png|837]]      
complementing the set means that the string passed cannot match the re of which comes under the set... also in a re, if we group soemthing with the brackets, the content in the brackets will be returned from the function

40.  #### \w-> word character means -> [a-zA-Z0-9_]
		![[Pasted image 20261108003224.png|970]]  -> ![[Pasted image 20261108001026.png|295]]

here we can see we have another argument in this case re.IGNORECASE which is a flag and we can pass these among them->
	![[Pasted image 20261108003402.png|381]]

41. here the question mark means that after @ we can have another subdomain but again thats we "can" means it's optional so both ayaan@pahuja.com and ayaan@pahuja.abc.com are valid

![[Pasted image 20261108004312.png|1456]]

# 42.
# also in a re, if we group soemthing with the brackets, the content in the brackets will be returned from the function

![[Pasted image 20261108013804.png]]--> ![[Pasted image 20261108014304.png]]--> here space is optional in name 

# := allows you to asign a value and at the same time check for a boolean in if condition like the image:

![[Pasted image 20261108014458.png|672]] short for ---> ![[Pasted image 20261108014519.png|655]]


43. We use remove prefix here cause if a user gives whole paragraph it will come with the username so we use remove prefix

![[Pasted image 20261108021240.png|781]]---> ![[Pasted image 20261108021326.png|624]]

# but this is still not the fix so we use re.search

![[Pasted image 20261108025601.png|1105]]


# WE can also use re.sub to solve the issue here:
![[Pasted image 20261108021708.png|494]]--->--->![[Pasted image 20261108023635.png|615]]


# ---------------------------------------------------OOPS---------------------------------------------------

## Tuple

44. here in this image, get_student function is returning 2 values separated by comas but these are not 2 values its one value and its type is tuple, whenevr we return 2 or more values it makes a tuple, diff b/w tuple and list is that it is immutable which means we cant change values in a tuple...... and when we get the value from the function we can either unpack it or can make a tuple with the values. Tuple is just like a list so we can access values inside it with indexing, also if you dont want to return 2 values as a tuple use square brackets to return as list..
  ![[Pasted image 20261108034005.png|585]]   ![[Pasted image 20261108033916.png|584]]   ![[Pasted image 20261108034210.png|238]]


45. Objectively better then tuple is returning dict cause we dont need to access it using indexing but we can just pass key and we'll get the value

	![[Pasted image 20261108035910.png|871]]

## -----------------------------------------------------------CLASSES----------------------------------------------------------------

- ... is a placeholder saying that "i'll come and add everything later" and it gives no error
			![[Pasted image 20261108040910.png]]


46. You can create a class with methods/functions  inside them using class keyword and anytime you use a class you create a object which have attributes as in instance variables (name) inside that. So here ==🔴student is a object== and ==🔴Student is a class== . 
	![[Pasted image 20261108041615.png|645]]

### IMPPPPPPPPP!!!! Every function in class takes atleast one argument
46. In a class which is just a template/mold if you want to initialize the contents of an object from a class, it is done in a `def __init__ (self)` function. 
		![[Pasted image 20261108042945.png|566]]                        ==🔴THE CONSTRUCTORS IN C/C++ IS INIT METHOD IN PYTHON==

==🔵How this works?->==   So first, the constructor call will construct a student object, how? it is going to use the student class as a mold/template and create the object and because we passed the arguments in the constructor call, we can customize the object it is about to create. and the constructor call will always call the `def __init__ (self)` function so this means whenever we call Student() which is a class, it will always call `def __init__ (self)` function. Ok so now what's self? Because without self we can not put the values passed anywhere else cause we dont have a variable in that, we use self so it means self gives you access of the current object create with the constructor call to store the values of arguments... name, house here
So in summary a object is created, with a class which is called and arguments are passed to create instance variable of the objects which was empty before call in this case- student...

47. We can raise a error in python just like in the image if something is not going right which will give the error and stop the whole program too
		![[Pasted image 20261108051105.png|576]]


### IMPPPPPPPPP!!!!
   
   ![[Pasted image 20261108054122.png|475]]             ==🔴To Fix This Print Issue that we cant print student directly->->==

48. turns out there is another special method (`__str__`) for class which will automatically call whenever a functions wants to read the object in this case student in string type. for eg->
	![[Pasted image 20261108054451.png|473]]                            


49. We can also create our own method and can also call it outside the function
	![[Pasted image 20261108060317.png|474]]  -------> ----------> ---------->  ![[Pasted image 20261108060339.png]]


### ----------------------------------------------------------DECORATES--------------------------------------------------------------


50. This is how we create getter and setter in python, but why do we do so? we do so so the code cant access the instance variable without the function and if it try so like in the image, it'll automatically run the function you made for the setter but only if a function is made as a setter and to get the value, we can only get through the getter function, also the self.house in init will the call the setter function to set the value, so basically what we manually did in c/c++ is being automatically done in python...THE SETTER WILL GET CALLED EVERYTIME WE SET THE HOUSE VALUE. also we cant keep same name of the method and the instance variable so we tend to keep the name of instance variable in this eg `self._house` also we can see that wwe hvae not put `_` in init function on self.house cause that creates fine line which allows us to just create the validation on the setter cause if its self.house it'll call the setter to set and will be validated automatically
	![[Pasted image 20261108061603.png|429]]   -->---> ---> ---> ![[Pasted image 20261108063439.png|345]]  --> ---> ---> ---> ![[Pasted image 20261108065627.png|407]]

51. but yeah its quite sensible that if you cant change .house youll just change `self._house` cause its the new instance name and yeah it will work and we cant fix it cause there is no public private or protected system like C/C++ in python so its just an honor system that if a instance variable is starting with a `_` you should not touch it... 
				![[Pasted image 20261108070516.png|607]]


### int, list, str are all classes, even the strip,lower,title are instance method that comes with str class

## ---------------------------------------------------------CLASS METHODS---------------------------------------------------------

# 52. 
 So if we want to use a function of class or make class a container for functions we use class methods cause we can access class methods without having a object in that class and with any variable, notice how we are first creating a obj of class and then calling the function but in second image we dont have to do all that and just call it simply. 

we use @classmethod to specify class methods also in addition to class methods we have class variables which exist within the class and is global to the class, houses in ts example. Also in a class method we pass cls as a argument which is just refrence of the class and whnever we have to access class variable, houses in this example we use cls.houses and to use the function in code we use `<ClassName>.<FunctionName>(<Arguments>)`Hat.sort("Harry") in here. Also whenever we return something from class method we return using this syntax-->> `return cls(name, house)` which will further create a object of datatype of the class name.........
![[Pasted image 20261109045858.png|710]]          ![[Pasted image 20261109050741.png|690]]

# -----------------------------------------------------INHERITANCE------------------------------------------------------

# 53.
So in python we can create mutiple classes and inherit a class which is now super/parent class to children class which will now share its methods, instance variables, etc to the decended class. In the image, there are 3 classes, Wizard is a super class of both Student and professor class and when ever either of 2 gets called, it also class the init method of super class using `super().__init__(name)` Also a thing to note is that parent class can not access attribute of children class cause inheritance goes in a downwards direction

![[Pasted image 20261109053923.png|791]]

# 54. Exception Hierarchy

![[Pasted image 20261109054334.png|455]]

#  55. Operator Overloading

we do operator overloading to fix this issue over here, yes we can do it with a simple logic too but this is jsut cool...So in python to do operator overloading of +, we use `__add__` function made in class which will automatically be called when 2 objects of the same datatype are added using +....
### THE FUNCTION=> `object.__add__(self,other)` here self means the left hand side of the operator and other means right hand side...

![[Pasted image 20261109055400.png|793]] ==> ==>   ![[Pasted image 20261109060019.png|584]]


# --------------------------------------------------------SETS-----------------------------------------------------------

# 56. 
To Overcome this long ahh code to to put some values in a list but not duplicate values we use sets... the syntax for the sets are like this
![[Pasted image 20261110023200.png]]         => => =>        ![[Pasted image 20261110024008.png|482]] 

# -------------------------------------------------GLOBAL VARIABLES----------------------------------------------------

# 57. 
Here we cant do this and receive a error cause we cant write global variables in a function which is defined without the global keyword and we can only read it, so how do we fix this? using global keyword like in the second image, but yeah ofc we preffer classes more then global variables

![[Pasted image 20261110030226.png|411]]      => => => =>  ![[Pasted image 20261110031037.png|450]]   => => => ![[Pasted image 20261110032009.png|370]]


# -----------------------------------------------------Constants---------------------------------------------------------

# 58. 
So contants are the variables which we can not change the values but in python we dont have a keyword or soemthing like "constants" so there is nothing stopping me from not not changing the meows value thats why we tend to capitalize every word of the variable to specify that it's value should not be change, also instead of hardcoding 3 anywhere it is a better practice to specify a variable for that 
			![[Pasted image 20261110033516.png|448]]           ![[Pasted image 20261110033626.png|440]]

# --------------------------------------------------------------------MYPY--------------------------------------------------------------

# 59. 
Because python dont have a data type system when specifiying variables, to check the code before releasing it to the world we tend to use my py to check if all the variables are using the intended data type we want.... here in the 2 nd image the **n:int** and **number:int** is a type hint which hints both python and mypy when running that the n and the number should be a int, and because it is not a int as you can see in number defination, we get a error. Also in image 2, -> None: means the the return value is always NONE so it throws a error cause we cant accept none in meows which is string

![[Pasted image 20261110034259.png|355]] ---> ![[Pasted image 20261110035654.png|329]]  ---> ---> --->![[Pasted image 20261110040000.png|561]]



# -------------------------------------------DOCUMENTATION OF FUNCTION (DOC STRINGS)------------------------------------------
# 60 
We use this format of docstring to document our own functions so that later on we dont have to create a documentation / how to use the function guide manually but we we can auto generate if we document our own functions in this format. It is a really widely used format
		![[Pasted image 20261110040954.png]]


# ---------------------------------------------------------ARGPASS-------------------------------------------------------
# 61
in 1st image where the number after -n 1 specifies how many meows i need, it is much harder to add support for all the letter like -a -b -c and what if the command line thingy is in diff order, to fix all these problems we use "ARGPASS" like in the image 2. So the args=parser.parse_args(); will automatically look in sys.argv for us we dont need to specify anything, also inside of this args have all the command line arguments after "-n" parsed by the parser also the default specifies the value after -n and the desciption and help is when the user type -h or --help in the cmd. Also we can pass type=int in add argument and then we dont have to worry about converting to int anywhere
	![[Pasted image 20261110042736.png|622]]    ![[Pasted image 20261110044305.png|768]]

# 62 
here we can not do something like this in image 1 cause it will send the whole list of coins to galleons, we use unpack, a single * symbol at the beginning of the name of list which unpacks  the list and send it to the individual argument, also it only works for list in this way, does not work for tuple and can be used in dict like in image 3... so we use 2 * for dictionaries which pass in this case 3 values with name which will be later matched with the names of the argument and conjusted/assigned to those variables and later used... also because we send it with names, we dont have to store them in order and can store in any order
![[Pasted image 20261110045152.png|698]]   ![[Pasted image 20261110045355.png|691]] 
									![[Pasted image 20261110050152.png]]

# 63
Positional Args And Kwargs are just same as the above point syntax- `*Args`  `**kwargs` also in the function   `*Args` always are specified first and `**kwargs`  are always specified in second
these are arguments which we can set in a function which will take any amount or arguments, either 1 or a 100 it doesnt matter in the case of `*args` it will make a tuple and  `**kwargs`  makes a dictionary... we can also you * in print to print every position of a list without the brackets and all
![[Pasted image 20261110051100.png|412]]   ![[Pasted image 20261110051416.png|396]]
![[Pasted image 20261110051111.png|412]]   ![[Pasted image 20261110051435.png|662]]


# --------------------------------------------------------MAPS-----------------------------------------------------------

# 64 
So in here we will pass a function and a list to map and map will automatically apply the function to everyone one of the lists's index and return it as a brand new list  like shown in image 2. Also we have to keep in mind to not give brackets when we are passing the function cause we dont have to just specify it and map will call it itslef
Before:
![[Pasted image 20261110052809.png]]          ![[Pasted image 20261110053221.png|506]]

## also really pythonic way of doing it is this:
![[Pasted image 20261110053452.png]]

# ------------------------------------------------------LIST COMPREHENSION-------------------------------------------

# 65. 

Before: 
![[Pasted image 20261110054643.png|868]]

After: Using Filter here... So basically unlike map filter needs a function to include which returns true or false for a question that should i include this value in the new list or not so the flow is that the filter calls is_gryffindor ans passing students dict asking should i include this element in the new dictionary, which is_gryffindor replies to with a return state that if the house of that student is gryffindor, keep it in the new dict... here lambda is just a concise way to build a throwaway helper function right inside the line of code where you need it. this means that it makes a one liner anonymous   function which returns the name of the student or 's' here

![[Pasted image 20261110055356.png|596]]
![[Pasted image 20261110055335.png|597]]

# ------------------------------------------------DICTIONARY COMPREHENSION----------------------------------------
# 66.  
How is the syntax diff from the list one? the gryffindors have a set of curly braces in it which will create a dict and not a list. Also here it is a list which dict in it, but what we want just one bigger dict with "name":"house", to do this we use the syntax in second image
    ![[Pasted image 20261110062235.png|726]]  ![[Pasted image 20261110062255.png]]


# 67. 
Instead Of the syntax in image 1 we can use something known as enumerate
![[Pasted image 20261110062438.png]]           ![[Pasted image 20261110062612.png|597]]
![[Pasted image 20261110062531.png|599]]           ![[Pasted image 20261110062627.png|601]]


# 68. Generators:
in the image 1 we have a function that generates sheep and when we cross 1 m mark of generating the sheep computer runs outta memory and does not print, to solve this problem we use generators like in image 2. We use the keyword "yield" in place of return to return one by one and not completely as a whole like in the image 1. 
##### THE YIELD KEYWORD WILL MAKE SURE THAT THE FUNCTION RETURN CHUNKS/LITTLE AMOUNT OF DATA IN THIS CASE DATA GENERATED BY 1 COMPLETION OF LOOP AND NOT THE WHOLE DATA AT ONCE
![[Pasted image 20261110063232.png]] ---> --->![[Pasted image 20261110064525.png|445]]


# 69. 
# Text To Speech -> PYTTSX3

   ![[Pasted image 20261110064608.png]]