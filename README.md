Assignment 1 Question 2
import json
dict1 = {'Haryana':'Chandigarh','Maharashtra':'Mumbai','Karnataka':'Bangluru','Rajasthan':'Jaipur','Uttar Pradesh':'Lucknow','Gujarat':'Gandhinagar','Goa':'Panaji'}
file = open(r"C:\Users\Hp\OneDrive\Desktop\Edyoda Practice\Edyoda Python Assignment 6\assignment_7_file.json","w")
json.dump(dict1,file)


OUTPUT IN JSON FILE
{"Haryana": "Chandigarh", "Maharashtra": "Mumbai", "Karnataka": "Bangluru", "Rajasthan": "Jaipur", "Uttar Pradesh": "Lucknow", "Gujarat": "Gandhinagar", "Goa": "Panaji"}

Assignment 2:-

class Dog:
    def __init__(self,name,age,coat_color):
        self.name = name
        self.age = age
        self.coat_color = coat_color

    def description(self):
        print(f"Name : {self.name} \nAge : {self.age}")
    
    def get_info(self):
        print(f"Coat_color : {self.coat_color}")
    
class JackRussellTerrier(Dog):
    def __init__(self, name, age, coat_color,trained):
        super().__init__(name, age, coat_color)
        self.trained = trained
    
    def owner(self):
        print(f"Owner of {self.name} dog is Mr. John.")
        
    def city(self):
        print(f"{self.name} lives in Los Angeles with his owner.")

class Bulldog(Dog):
    def __init__(self, name, age, coat_color,friendly):
        super().__init__(name, age, coat_color)
        self.friendly = friendly

    def height(self):
        print(f"Height of {self.name} is 2 feet.")
    
    def weight(self):
        print(f"Weight of {self.name} is 50kg.")

dog = Dog("Pablo",4,"Black and White")
dog.description()
dog.get_info()

jack = JackRussellTerrier("Skuby",5,"Black","yes")
jack.description()
jack.get_info()
jack.owner()
jack.city()

bull = Bulldog("Tyson",3,"Brown","Yes")
bull.description()
bull.get_info()
bull.height()
bull.weight()


OUTPUT:-
Name : Pablo 
Age : 4
Coat_color : Black and White
Name : Skuby 
Age : 5
Coat_color : Black
Owner of Skuby dog is Mr. John.
Skuby lives in Los Angeles with his owner.
Name : Tyson 
Age : 3
Coat_color : Brown
Height of Tyson is 2 feet.
Weight of Tyson is 50kg.
