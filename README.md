#Dictionary
#Examples
dictionary = {"Name":"Nivesh","Address":"Bokaro","Age":"23"}
print(dictionary["Age"])

#Iteration in Dictionary
for i in dictionary:
    print(i)
#Iteration in Dictionary @Using Value Functions.
for j in dictionary.values():
    print(j)
#Iteration in Dictionary @items Functions.
for m,n in dictionary.items():
    print(m,":",n)

#Dictionary top 5 functions.
#Examples
dictionary = {"Name":"Nivesh","Address":"Bokaro","Age":"23"}

print(dictionary.get("Name"))    #using get
print(dictionary.items())        #using items
print(dictionary.keys())          #using keys
print(dictionary.values())        #using value
print(dictionary.copy())          #using copy 

#write a python program to sort a dictionary by vale.
data = {"a":1,"b":6,"c":3,"d":100,"e":17}
print(sorted(data.values()))

#write a python script to print a dictionary where the keys are numbers between 1 and 15 and tha value are square of keys.
datas = {}
for j in range (1,16):
       print(j*j)

#write a program to multiply all the items in a dictionary.
nivesh = {"a":2,"b":4,"c":16}
product=1
for i in nivesh.values():
       product *= i
       print(product)

#write a python program to sort a dictionary by key.
key = {96:"a",177:"z",50:"b",12:"d"}
print(sorted(key.keys()))
