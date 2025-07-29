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
    
