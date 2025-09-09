# Python-notes
Python notes-learning-solving

# DATA TYPES AND VARIABLES
int,str,bool,float

# COLLECTIONS
  1)List  - ordered,mutable(It can be changed after created)
  2)Tuple - ordered, immutable(cant be changed after created)
  3)set   - unordered,
  4)Dict  - key-value pairs

# LOOPS AND CONDITION
  1) if/elif/else  - runs on condition, if condition is false, it skips and goes to the next condition.
  2) for loop      - repeat a block of code for each item or range
  3) while loop    - repeats while the condition true
     *break         - stops the loop
     continue      - skip the current iteration*
     
# ARRAYS 
  Array is a collection of elements, stored in continuous memory locations of SAME DATA TYPE   (fast in memory, easy to access with index)
               DIFFERENCE BETWEEN LIST AND ARRAY
                               LIST                                         ARRAY
                 1) data type    -  can store mixed data type      |      stores only same type 
                 2)felixable     -  less flexible                  |        more flexible
                 3) speed        -  faster for numbers             |      slower for num operations
                 4) example       
                 
                         nums=[1,2,3,4]                            |    import array
                         print(nums[0])                                 arr=array.array('i',[1,2,3,4])
                                                                        print(arr[0])

# STRINGS
  sequences of characters inside quotes( '' , " " , '''  or """ )
     s = "hello" or 'hello' """hello"""

      triple quotes is also used for multi-line comments.
      # is for single line comment   (They do not run, its human readable)

  1.creating strings
  
     s="hello" 
     s2='hello'
     s3="""hello"""
     
 2. accessing characters
    
        s="python"
        print(s[o])      #first character's index                                    output: 'p'
        print(s[-1])     #last character's index                                     output: 'n'

4.slicing 

       s="programming language"
       print(s[0:6])              #'progra'            the slicing gives 0 to 6-1 (it works like n-1)
       print(s[ :5])              #'progr'             if the starting point is not mentioned it will start as from zero
       print([-1:-5])             #'egau'              we can use negative index for slicing too

5. changing case
   s="python Programming"
   
       s.upper()          #'PYTHON PROGRAMMING'
       s.lower()          #'python programming'
       s.capitalize()     #'Python Programming'    (capitalize the first letter)
       s.title()          #'Python Programming'
       s.swapcase()       #'pYTHON pROGRAMMING'    (swap upper to lower & viceversa)
   
7. checking content
   It will check whether its true or not based on content

       s.isdigit()   # True if all digits
       s.isalnum()   # True if letters+numbers
       s.islower()   # True if all lowercase
       s.isupper()   # True if all uppercase
       s.isspace()   # True if only whitespace

8. Replacing & Stripping
   
       s.replace("fun", "awesome")   # 'Python is awesome'
       s.strip()   # remove spaces from start/end
       s.lstrip()  # remove spaces from left
       s.rstrip()  # remove spaces from right

9. Splitting & Joining
    
       s = "I love Python"
       words = s.split()       # ['I', 'love', 'Python']
       grouped = ",".join(words)   # 'I,love,Python'

10. Concatenation & Repetition
    
        s1 + s2        # 'HelloWorld'
        s1 * 3         # 'HelloHelloHello'

11. Startswith & Endswith
    
        s = "Python"
        s.startswith("Py")  # True     (gives the first occurense) 
        s.endswith("on")    # True

notes: 
\n   # new line
\t   # tab
\\   # backslash
\"   # double quote
\'   # single quote

name = "Kiruthi"
age = 18

'format method'
print("My name is {}, age {}".format(name, age))

'f-string (Python 3.6+)'
print(f"My name is {name}, age {age}")

# Functions in Python
   What is a Function?
       A function is a block of reusable code that performs a specific task.
       Helps avoid repetition and organize your program.

        def hello():
            print("Hello Kiruthi")
            
  def → keyword to define a function
  greet → function name
  () → parameters (empty here)
  : → start of function block
  Indentation is mandatory

  when the function is called, the block of code under it will run.   for eg. hello()                          output: Hello Kiruthi

  1) Function Parameters
    Functions can take inputs (arguments).
         
         def hello(name):
    print(f"Hello {name}")
    hello("sudha")

  output: Hello sudha

 2) Default Parameters

        def greet(name="Guest"):
        print(f"Hello {name}")
        greet()                                                              # Hello Guest
        greet("Kiki")                                                        # Hello Kiki

  3) Return Statement
     Functions can return a value.

         def add(a, b):
         return a + b
         result = add(5, 10)
         print(result)                                                       # 15

  4)positional arguement 
  
    def info(name, age):
        print(f"{name} is {age} years old")
    info("Kiki", 18)                                                        #Kiki is 18 years old

  5)keyword arguement 
  
    def info(name, age):
        print(f"{name} is {age} years old")
    info(age=18, name="Kiki") # keyword arguments                          #Kiki is 18 years old

  6) Variable-length Arguments
        *args → for multiple positional arguments
        **kwargs → for multiple keyword arguments

    def sum_all(*args):
       return sum(args)
    print(sum_all(1,2,3,4))                                                 # 10

    def show_info(**kwargs):
        print(kwargs)
    show_info(subject='python', mark=94)                                    # {'subject': 'python', 'mark': 94}

  7) Lambda (Anonymous) Functions

    square = lambda x: x**2
    print(square(5))                                                      # 25
Useful for short one-line functions

  8) Scope of Variables
         Local variable → inside function, cannot be accessed outside
         Global variable → defined outside, can be accessed anywhere

    x = 10   #global

    def func():
        y = 5  # local
    print(x, y)
    func()
    print(y)  # Error, y is local

  9) Docstrings in Functions

    def greet(name):
        """This function greets the person with given name."""
        print(f"Hello {name}")
    print(greet.__doc__)
