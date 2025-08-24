# Calculator-Basic-Project

# Online Python compiler (interpreter) to run Python online.
# Write Python 3 code in this online editor and run it.


print('*****This is a basic calculator which helps to peroform operation like Add, Sub,Multiply, Divide,Square Root, Power****')

print("Specify the operation which you want to perform")

print ("Type 1 for addtion")
print ("Type 2 for subraction")
print ("Type 3 for multiplication")
print ("Type 4 for division")
print ("Type 5 for make square of the number")
print ("Type 6 for sqaure root")


import math
while True:

    print('---- Lets start the process----')

    value = (input('Enter the digit 1,2,3,4,5,6 --  '))

    if value in ('1','2','3','4','5','6'):
        try:
            if value in ('1','2','3','4'):

                a = int(input("Enter First Number   "))
                b = int(input("Enter Second Number  "))
            
            elif value in ('5','6'):

                x = int (input("Enter the value  "))
                    

        except ValueError:
            print ("Please enter the correct value")
            continue
        if value == '1':
            print(a+b)

        elif value == '2':
            print(a-b)

        elif value == '3':
            print(a*b)

        elif value == '4':
            try:

                print(a/b)
            except ZeroDivisionError :
                print('Please do not divide by zero')
                continue
        
   
        elif value == '5':
            print(x*x)

        elif value == '6':
            print (math.sqrt(x))


    
    
        retry = input ('For next calculation  "Press y for Yes" , "In case of different value program will be shut down"  ')

        if retry == 'y':
            continue
        

        else:
            break
            

    else:
        print("**** Please type a valid operation ****")


print ('Thanks for the time')
