from datetime import date
class person:
      def __init__(self,name,country,dob):
           self.name=name
           self.country=country
           self.dob=dob
      def calage(self): 
          today=date.today()
          age = today.year-self.dob.year

          if today < date(today.year,self.dob.month, self.dob.day):
             age -= 1

          return age


p1 = person("saikumar", "ongole",date(2006, 7, 3))

print("calculated age for each person")
print("******************************")
print("person 1:")
print("Name:",p1.name)
print("Country:",p1.country)
print("Date of birth:",p1.dob)
print("Age:", p1.calage())
