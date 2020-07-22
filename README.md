# PythonPractical5
#Syntax Errors
# x = int(input("Enter a number")) #4
#
# while x%2 == 0:
#     print("You have entered an even number")
#     break
# else:
#     print("You have entered an odd number")


#Logical Errors (Semantic error)
#
# x = float(input("Enter a number: "))
# y = float(input("Enter a number: "))
#
# #BODMAS
#
# z = x+y / 2
# print("The average is: " + str(z))
#
# #Runtime Error
#
# # some common examples:
# # division by zero
# # performing an operation on incompatible types
# # using an identifier which has not been defined
# # accessing a list element, dictionary value or object attribute which doesn’t exist
# # trying to access a file which doesn’t exist
#
# a = open("demofile.txt")
# b = open("demo2file.txt")
#
# print("Something")

#=======================================================================================

#Try; except; else; finally; raise

# The try block lets you test a block of code for errors.

# The except block lets you handle the error.

# The finally block lets you execute code, regardless of the result of the try- and except blocks.

#Exception Handling
# try:
#     print("Line1")
#     print("Line2")
#     print(x) #Raises an exception
#     print("Line3")
# except:
#     print("oops something went wrong!")
    #sendEmail()

#Many Exceptions


# try:
#
#     print(2/0) #ZeroDivisionError exception raised
#     # print(z) #NameError exception is raised
# except NameError:
#     print("Variable z is not defined")
# except ZeroDivisionError:
#     print("You cant divide by zero")
# except:
#     print("Something went wrong!")

#Else

# You can use the else keyword to define a block of code to be executed if no errors were raised:

# try:
#     print("Hello")
#     #print(2/0)
# except:
#     print("Something went wrong")
# else:
#     print("Nothing went wrong")
#
# try:
#     print("Hello")
# except:
#     print("something went wrong")
# else:
#     print("nothing went wrong")

#Finally

#The finally block, if specified, will be executed regardless if the try block raises an error or not.

# try:
#     # print(x)
#     print("Working")
# except:
#     print("Something went wrong")
# finally:
#     print("The 'try except' is finished")
#
# try:
#     # x = 5
#     print(x)
# except:
#     print("something went wrong")
# finally:
#     print("the 'try except' is finished")
#
#Finally block can be useful to close objects and clean up resources:

# try:
#     f = open("demoFile.txt")
#     f.write("Something")
# except:
#     print("Something went wrong when writing to the file")
# finally:
#     f.close()

#Raise an exception

#To throw (or raise) an exception, use the 'raise' keyword.
#
# x = -1
#
# if x < 0:
#     raise Exception("Sorry, no numbers below zero allowed")

# y = -1
#
# if y < 0:
#     raise Exception("Check Jira")

#You can define what kind of error to raise, and the text to print to the user.


x = "hello"

if not type(x) is int:
    raise TypeError("Only integers are allowed")

x = "hello"

if not type(x) is int:
    raise TypeError("Only int Allowed")










