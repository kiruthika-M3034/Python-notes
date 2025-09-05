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

      triple 
