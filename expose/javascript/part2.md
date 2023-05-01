1. Line 12 will print out **3** because the for loop iterates 3 times from the array of size 3. Since **var** has function scope, **console.log** has access to any var variable within the function its in. 
2. Line 13 will print out **150** since that was the last price the for loop discounted. Since **var** has function scope, **console.log** has access to any var variable within the function its in.  
3. Line 14 will print out **150** since that was the last price that was finalized in the for loop. Since **console.log** and *finalprice* are in the same function, *finalprice* can be accessed.
4. Given an array of prices and a discount price, the function will return a new array of the same size with each price in the array discounted by the given discount price. In this case the function returns [50, 100, 150]
5. At Line 12 the code will return an **error**. Since **let** has block scope, the varaible *i* can only be accessed within the for loop thus *i* is not defined when the code reaches **console.log**.
6. At Line 13 the code will return an **error**. Since **let** has block scope, the varaible *discountedPrice* can only be accessed within the for loop thus *discountedPrice* is not defined when the code reaches **console.log**.
7. Line 14 will print out **150** since *finalprice* and **console.log** are in the same block.
8. Just like **4.**, Since there are no errors, the function returns [50, 100, 150].
9. At line 11 the code will return an **error**. Since **let** has block scope, the variable *i* can only be accessed within the for loop thus *i* is not defined when the code reaches **console.log**.
10. Line 12 will print out 3 which is the length of the input array. Since **console.log** and **const** are in the same block and *length* does not get reassigned, the function works as intended.
11. The function returns [50, 100, 150]. The program does not throw an error since the **const** variable *discountedPrice* is not reassigned within it's block. Each iteration of the for loop just initializes *discountedPrice* as if it was the first time seeing the variable name.
12. A: student.name \
B: student['Grad Year'] \
C: student.greeting(); \
D: student['Favorite Teacher'].name \
E: student.courseload[0]
13.  A: '32'. 2 got converted to a string and then gets concatenated with the 3 \
B: 1. The string 3 gets converted to a number and gets subtracted outputting 1 \
C: 3. The null gets coverted to a 0 and gets added to 3 which equals 3 \
D: '3null'. The null gets converted to the string 'null' which gets concatenanted with string 3. \
E: 4. True gets converted to 1 which gets added to 3 giving 4 to the output. \
F: 0. Both false and null get converted to 0 which added output 0. \
G: '3undefined'. Undefined gets converted to the string undefined and then gets concantenated with the string 3. \
H: NaN. undefined is equal to NaN when it gets converted to a number. A number minus NaN outputs NaN 
14.  A: true. The string 2 gets converted to a number and 2 is greater than 1 so it returns true. \
B: false. 12 is lexigraphically less than 2 thus '2' < '12' returns false. \
C: true. String 2 gets converted to a number and 2 is equal to 2 thus it returns true. \
D: false. Since its a triple equals, the string 2 does not get converted to a number and a string is not equal to a number thus it returns false. \
E: false. true gets converted to a 1. 1 does not equal 2 thus it returns false. \
F: true. When 2 gets converted to a Boolean it gets set to true and thus it returns true.
15.   == checks two different values with type conversion while === checks two different values without type conversion (strict comparison).
16. -
17. The function will return an array with values [2,4,6]. When we call the modifyArray function we send in the array we want to change and the function we are using to modify that array. Inside modifyArray we create a new array. For each item in the old array, we pass that item to the function we sent as a parameter which in this case doubles the number. This function returns the doubled number which we then push into the array. At the end we return the new array.
18. -
19. 1,3,4,2. When the function is called, 1 gets printed, 2 gets put in timeout for one second, then 3 gets put in a timeout for 0 milliseconds (instant) and thus gets printed. 4 then gets printed. After the 1000 milliseconds have run out, 2 finally gets printed. 