# week5pythonassignment
class Smartphone:
    def __init__(self, brand, model, ram, storage):
        self.brand = brand
        self.model = model
        self.ram = ram
        self.storage = storage

    def call(self):
        print("Making a call")

    def message(self):
        print("Sending a message")

    def browse(self):
        print("Browsing the internet")
class Device:
    def __init__(self, brand, model):
        self.brand = brand
        self.model = model

    def call(self):
        print("Making a call")

    def message(self):
        print("Sending a message")

class Smartphone(Device):
    def __init__(self, brand, model, ram, storage):
        super().__init__(brand, model)
        self.ram = ram
        self.storage = storage

    def browse(self):
        print("Browsing the internet")
class Car:
    def __init__(self, make, model, year):
        self.make = make
        self.model = model
        self.year = year

    def move(self):
        print("Driving")

class Plane:
    def __init__(self, make, model, year, capacity):
        self.make = make
        self.model = model
        self.year = year
        self.capacity = capacity

    def move(self):
        print("Flying")

car = Car("Toyota", "Camry", 2020)
plane = Plane("Boeing", "747", 1998, 416)

car.move()  # Output: "Driving"
plane.move()  # Output: "Flying"
