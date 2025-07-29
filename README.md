# Files
file=open('nnnn.txt','r')
data=file.read()
print("File data in nnnn.txt:",data)
file.close()
OUTPUT:
File data in nnnn.txt: 
----------------------------------------------------------------------------------------------------
f=open('nnnn.txt','w')
f.write("the fruits was collapsed...")
f.close()
----------------------------------------------------------------------------------------------------
f=open('nnnn.txt','a')
f.write("A girl sat beside of me")
f.close()
---------------------------------------------------------------------------------------------------
filename='nnnn.txt'
with open(filename,'w')as f:
    f.write("My favourite colour is Pink.\n")
with open(filename,'r+')as file:
    print("latest data:")
    print(file.read())
    file.seek(0)
    userinput=input("\n enter to overwrite from begging...")
    file.write(userinput)
    file.seek(0)
    print("\n file after writing by r+")
    print(file.read())
    OUTPUT:
    latest data:
My  favourite colour is Pink.


 enter to overwrite from begging... Gopi

 file after writing by r+
Gopifavourite colour is Pink.
-----------------------------------------------------------------------------------------------------
filename=input("Enter filename with extensions")
with open(filename,'r')as file:
    text=file.read()
    letter= input("Enter a char to search frequency:")
    count=0
    for char in text:
        if char== letter:
            count+=1
print(letter,"appears",count,"times in the file")
OUTPUT:
Enter filename with extensions line.txt
Enter a char to search frequency: e
e appears 2 times in the file
-------------------------------------------------------------------------------------------------
