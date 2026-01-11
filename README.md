# # Single
# 1misol

# class Telephone:
#     def __init__(self,model, year, color, country):
#         self.model = model
#         self.year = year
#         self.color = color
#         self.country = country
#     def get_info(self):
#         return f"Model: {self.model} Ishlab chiqilgan yili: {self.year} Rangi: {self.color} Ishlab chiqilgan Davlati: {self.country}"
# class Smartphone(Telephone):
#     def __init__(self, model, year, color, country, Os, ram, camera, batary):
#         super().__init__(model, year, color, country)
#         self.Os = Os
#         self.ram = ram
#         self.camera = camera
#         self.batary = batary
# c1 = Smartphone("Redmi", 2020, "oq", "China", "Android: 14", "8GB - 256GB", "50MP", 8000)
# c2 = Smartphone("OPPO", 2024, "qora", "China", "Android: 13", "6GB - 128GB", "50MP", 85000)
# c3 = Smartphone("Apple", 2025, "oq", "USA", "IOS 17", "8GB - 256GB", "38MP", 4500)
# print(c1.get_info())
# print(c2.get_info())
# print(c3.get_info())











# # 2 misol
# class Person:
#     def __init__(self, first_name, last_name, address, year):
#         self.year = year
#         self.first_name = first_name
#         self.last_name = last_name
#         self.address = address
        
#     def get_info(self):
#         return f"Ism: {self.first_name}, familiya: {self.last_name}, tugilgan yil: {self.year}"
    

# class Work(Person):
#     def __init__(self, first_name, last_name, address, year, company, employe, money):
#         super().__init__(first_name, last_name, address, year)
#         self.company = company
#         self.employe = employe
#         self.money = money

#     def get_info(self):
#         person_info = super().get_info() 
#         return f"{person_info}, kompaniya: {self.company}, lavozim: {self.employe}, maosh: {self.money}$"

# a1 = Work("Maruf", "Amonturdiyev", "Qashqadaryo", 2007, "Google", "Cybersecurity", 20000)
# a2 = Work("Shaxriyor", "Shaxiyorov", "Samarqand", 2003, "Amazon", "Software", 10000)


# print(a1.get_info())
# print(a2.get_info())




# # MULTIPLE
#  1misoll

# class Oqituvchi:
#     def __init__(self, ism, fan, tajriba_yili):
#         self.ism = ism
#         self.fan = fan
#         self.tajriba_yili = tajriba_yili

#     def dars_berish(self):
#         return f"{self.ism} {self.fan} fani bo‘yicha dars bermoqda"


# class Dasturchi(Oqituvchi):
#     def __init__(self, ism, fan, tajriba_yili, til, kompaniya):
#         super().__init__(ism, fan, tajriba_yili)
#         self.til = til
#         self.kompaniya = kompaniya

#     def kod_yozish(self):
#         return f"{self.ism} {self.til} tilida kod yozmoqda, kompaniya: {self.kompaniya}"


# class IT_Ustoz(Dasturchi):
#     def __init__(self, ism, fan, tajriba_yili, til, kompaniya, mentorlik_tajriba):
#         super().__init__(ism, fan, tajriba_yili, til, kompaniya)
#         self.mentorlik_tajriba = mentorlik_tajriba

#     def mentorlik(self):
#         return f"{self.ism} IT ustoz sifatida {self.mentorlik_tajriba} yil mentorlik qilmoqda"


# u1 = IT_Ustoz("Ali", "Informatika", 10, "Python", "IT Park", 5)

# print(u1.dars_berish())
# print(u1.kod_yozish())
# print(u1.mentorlik())

# # 2misol
# class Laptop:
#     def __init__(self, laptop_name, model):
#         self.laptop_name = laptop_name
#         self.model = model

#     def get_laptop_info(self):
#         return f"Laptop nomi: {self.laptop_name}, modeli: {self.model}"


# class Person:
#     def __init__(self, name, age):
#         self.name = name
#         self.age = age

#     def get_person_info(self):
#         return f"Ismi: {self.name}, yoshi: {self.age}"


# class Comment(Person, Laptop):
#     def __init__(self, name, age, laptop_name, model, text, rate=0):
#         Person.__init__(self, name, age)
#         Laptop.__init__(self, laptop_name, model)

#         self.text = text
#         self.rate = rate

#     def get_comment_info(self):
#         return f"Izoh: {self.text}, Bahosi: {self.rate}/5"



# comment1 = Comment(
#     name="Jahongir",
#     age=19,
#     laptop_name="ASUS",
#     model="ASUS TUF Gaming F15",
#     text="Yaxshi laptop",
#     rate=4
# )


# print(comment1.get_person_info())
# print(comment1.get_laptop_info())
# print(comment1.get_comment_info())






















# MULTI LEVEL
#1misol
# class Computer:
#     def __init__(self, brand, processor, ram, memory):
#         self.brand = brand
#         self.processor = processor
#         self.ram = ram
#         self.memory = memory

#     def get_computer_info(self):
#         return f"Brand: {self.brand}, Processor: {self.processor}, RAM: {self.ram}GB, Memory: {self.memory}GB"


# class Desktop(Computer):
#     def __init__(self, brand, processor, ram, memory, monitor_type, keyboard_type):
#         super().__init__(brand, processor, ram, memory)
#         self.monitor_type = monitor_type
#         self.keyboard_type = keyboard_type

#     def get_desktop_info(self):
#         return f"Monitor: {self.monitor_type}, Keyboard: {self.keyboard_type}"


# class Laptop(Desktop):
#     def __init__(self, brand, processor, ram, memory, monitor_type, keyboard_type, battery, portable=True):
#         super().__init__(brand, processor, ram, memory, monitor_type, keyboard_type)
#         self.battery = battery
#         self.portable = portable

#     def get_laptop_info(self):
#         return f"Battery: {self.battery}Wh, Portable: {self.portable}"



# l1 = Laptop("Dell", "Intel i7", 16, 512, "LED", "Mechanical", 60)
# l2 = Laptop("HP", "Intel i3", 8, 256, "OLED", "Mechanical", 90)


# print(l1.get_computer_info())
# print(l1.get_desktop_info())
# print(l1.get_laptop_info())
# print(l2.get_computer_info())
# print(l2.get_desktop_info())
# print(l2.get_laptop_info())




class Transport:
    def __init__(self, name, max_speed):
        self.name = name
        self.max_speed = max_speed

    def move(self):
        return self.name + " harakatlanmoqda"

    def show_speed(self):
        return "Maksimal tezlik: " + str(self.max_speed) + " km/soat"


class Car(Transport):
    def __init__(self, name, max_speed, wheels_count, fuel_type):
        super().__init__(name, max_speed)
        self.wheels_count = wheels_count
        self.fuel_type = fuel_type

    def wheels(self):
        return "G‘ildiraklar soni: " + str(self.wheels_count)

    def fuel(self):
        return "Yoqilg‘i turi: " + self.fuel_type


class ElectricCar(Car):
    def __init__(self, name, max_speed, wheels_count, battery_capacity):
        super().__init__(name, max_speed, wheels_count, "Elektr")
        self.battery_capacity = battery_capacity

    def battery(self):
        return "Batareya sig‘imi: " + str(self.battery_capacity) + " kWh"

    def charge(self):
        return "Mashina zaryadlanmoqda..."



e = ElectricCar(
    "Tesla Model 3",
    225,
    4,
    75
)


print(e.move())
print(e.show_speed())
print(e.wheels())
print(e.fuel())
print(e.battery())
print(e.charge())
