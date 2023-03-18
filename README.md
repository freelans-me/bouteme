<  завдання 1   > 
class Parent1:
    def __init__(self):
        self.attribute1 = "Parent1 attribute"
    
    def method1(self):
        print("This is Parent1 method")

class Parent2:
    def __init__(self):
        self.attribute2 = "Parent2 attribute"
    
    def method2(self):
        print("This is Parent2 method")

class Child(Parent1, Parent2):
    def __init__(self):
        super().__init__()
        self.attribute3 = "Child attribute"
    
    def method3(self):
        print("This is Child method")
        
        
        
    <     завдання 2     >
         import random

class Encoder:
    def __init__(self, num):
        self.__num = num
    
    def __random_operation(self):
        return random.choice([self.__num + 10, self.__num - 10, self.__num * 2, self.__num / 2])
    
    def encode(self):
        self.__num = self.__random_operation()
    
    def decode(self):
        return self.__num
