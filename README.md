### Hi there 👋

<!--
**Nitheeshkanna/nitheeshkanna** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->

print("Welcome To ") 
print(" \t \"Big Bazaar\" Shop")
tot=[]
c=0
m={"1":"Milk","2":"Egg","3":"Fish","4":"Chicken","5":"Bread","6":"Sugar","7":"Iodized Salt","8":"DryChilli",
   "9":"RockSalt","10":"Butter"}
print(m)
while c < 3:
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
        print("---Total Bill is :",k,"---")
        break
print("**Thank you for visiting out Shope** ")
print("**Please Fill your details for MemberShip **")
n= int(input("Enter a no of Account create:"))
for i in range(n):
    n=input("Enter a name:")
    a=input("Enter your Address:")
    ph=int(input("Enter a Phone no:"))
    print("Name :",n)
    print("Address :",a)
    print("Phone No :",ph)
    print("**Thank you for creating Membership**")
    print("\t--This is your \"Big Bazaar\"",",","\'*",ph,"002*\'--",sep="")
    print("From your next \"Big Bazaar\" purchase point added on it ")
    print(" \t********** ")
