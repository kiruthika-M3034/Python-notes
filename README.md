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

  
