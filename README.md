from tqdm import tqdm
import time
n=100
for i in tqdm (range (n),desc="Loading…"):
    time.sleep(0.01)
print("Welcome To ") 
print(" \t \"Big Bazaar\" Shop")
print("Christmas Sale '20%' Offer")
tot=[]
c=0
m={"1":"Milk","2":"Egg","3":"Fish","4":"Chicken","5":"Bread","6":"Sugar","7":"Iodized Salt","8":"DryChilli",
   "9":"RockSalt","10":"Butter"}
print(m)
while c <=3:
    m={"1":["Milk",10],"2":["Egg",3],"3":["Fish",60],"4":["Chicken",150],"5":["Bread",40],"6":["Sugar",20],"7":["Iodized Salt",50],
       "8":["DryChilli",30],"9":["RockSalt",30],"10":["Butter",51]}
    a=input("Enter your product:")
    if a in m:
      print(m[a][0]," is available")
      print(m[a][0],"price=",m[a][1])
      q=int(input("Enter a quantity :"))
      #print(m[a][0],"x",q,"=",q*m[a][1])
      print("your Bill is=",q*m[a][1])
      tot.append(q*m[a][1])
      k=0
      for i in tot:
        k=k+i
    else:
        print("Sorry Sir/Mam your product is not available ")
        print("Please select any other iteam you want")
        c=c+1
    m=input("Do you want continue your purchase:y/n:")

    if  m=='y' or m=='Y':
          continue
    else:
        p=50
        for i in tqdm (range (p),desc="Loading…"):
            time.sleep(0.01)
        print()
        print("\t---Total Bill is :",k,"---")
        print()
        j=(20/100)*k
        print("\t$$-Discount Bill :",k-j,"-$$")
        print()
        break
print("**Thank you for visiting out Shope** ")
print("--------------------------------------------------------------------------------------------------------------")
print("**Please Fill your Details Below for MemberShip **")
print("--------------------------------------------------------------------------------------------------------------")

w=input("Do you Want Create BIG BAZAAR MemberShip Account:y/n:")
if w=='y' or w=='Y':
    n= int(input("Enter a no of Account want to create:"))
    for i in range(n):
        n=input("Enter a name:")
        a=input("Enter your Address:")
        ph=int(input("Enter a Phone no:"))
        print("Name :",n)
        print("Address :",a)
        print("Phone No :",ph)
        print("**Thank you for creating Membership**")
        print()
        p=100
        for i in tqdm (range (p),desc="Loading…"):
            time.sleep(0.01)
        print()
        print("\t--This is your \"Big Bazaar\""," ","No:","\'*",ph,"002*\'--",sep="")
        print()
        print("From your next \"Big Bazaar\" purchase point added on your Membership Card ")
        print(" \t \t********** ")
        print("\t #Thank You ","Mr/Ms/Mrs.",n,"#",sep="")
        print("\t \t #Welcome...#")
else:
    print()
    print("From your next \"Big Bazaar\" purchase point added on your Membership Card ")
    print(" \t \t********** ")
    print("\t #Thank You ","Mr/Ms/Mrs","#")
    print("\t \t #Welcome...#")
    print("------------------------------------------------------------------------------------------------------------")
