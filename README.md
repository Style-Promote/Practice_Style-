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
