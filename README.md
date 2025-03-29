# file_handling-Pandas-EXCEL

SOURCE CODE::::
import os

filename = "example.txt"

if os.path.exists(filename):
    print("File exists")
else:
    print("File not found. Creating the file...")
    with open(filename, "w") as file:
        file.write("This is a new file.") 
    print("File created successfully.")


file = open("example.txt","r")
content = file.read()
file.close()
print("File Content:", content)

file = open("example.txt","w")
file.write("hello nauman irshad!\n")

file = open("example.txt","r")
content = file.read()
print("File Content:", content)


file = open("example.txt","r")
print(file.read (5))
file.close()

file = open("example.txt","r")
lines= file.readlines()
print(lines)
file.close()

with open("example.txt","r") as file:
    content= file.read()
    print(content)

