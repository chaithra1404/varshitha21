
class Cloth:

def __init__(self, name, brand, size, price = 0 ):
    self.name = name
    self.brand = brand
    self.size = size
    self.price = price
class ClothStore:

cloths = []
selectedCloth = []

def __init__(self, name, brand, size, price ):
    b = Cloth(name,brand,size = size, price = price)
    self.cloths.append(b)

def show(self):
    print("============== AVAILBALE CLOTHS ==========")
    
    pos=0

    for cloth in self.cloths:
        print("============ ", pos, " ==========") 
        pos += 1   
        self.display(cloth)
        

def select(self):
    print("========== SELECT A CLOTH =======")
    print("====== HOW MANY CLOTH YOU WANT? ======")
    neededCloths = int(input())

    for i in range(0, neededCloths ):
        print("====== INPUT THE CLOTH NO ======")
        selectedCloth = int(input())
        print("========== SELECTED A CLOTH =======")
        b = self.getClothById(selectedCloth - 1)
        self.selectedCloth.append(b)
        print(self.display(b))

def getClothById(self, position):
    return self.cloths[position]

def display(self, cloth):
    print("Cloth name : ", cloth.name)
    print("Cloth SIZE : ", cloth.size)
    print("Cloth Price : ", cloth.price)
    print("Cloth Brand : ",cloth.brand)

def selectedCloths(self):
    return self.selectedCloth
class BillCounter:

cloths = []
def __init__(self, myCloths):
    self.cloths = myCloths

def display(self):
    pos = 0
    for cloth in self.cloths:
        print("============ BILL COUNTER CLOTHS ========")
        pos += 1
        print("============ CLOTH NO", pos,"========")
        print("Cloth name : ", cloth.name)
        print("Cloth SIZE : ", cloth.size)
        print("Cloth Price : ", cloth.price)
        print("Cloth Brand : ",cloth.brand)

def getTotal(self):
    total = sum(map(lambda b : b.price, self.cloths))
    print("=========== TOTAL PRICE =======")
    print(total)

def getMax(self):
    total = max(map(lambda b : b.price, self.cloths))
    print("=========== MAX PRICE =======")
    print(total)

def getMin(self):
    total = min(map(lambda b : b.price, self.cloths))
    print("=========== MIN PRICE =======")
    print(total)

def getBrands(self):
    print("================== BRANDS =============")
    brands = map(lambda a : a.brand, self.cloths)
    for brand in brands:
        print(brand)


def delete(self):
    print("=========== DO YOU WANT DELETE? 1 = YES, 0 = NO")
    choice = int(input())
    if (choice == 1):
        print("=========== ENTER CLOTH NUMBER =======")
        position = int(input())
        self.cloths.remove(self.getClothById(position))
    else:
        print("=========== NO CLOTHS =========")

def getClothById(self, position):
    return self.cloths[position - 1]
if "MAIN":

print("========== WELCOME TO CLOTH STORE ==========")

bs = ClothStore("kurtha", "biba", "s", 599)
bs = ClothStore("hoodie", "gucci", "xxl", 899)
bs = ClothStore("jacket", "nike", "xl", 999)
bs = ClothStore("t-shirt", "adidas", "xxxl", 1399)

bs.show()

bs.select()

selectedCloths = bs.selectedCloths()

print(selectedCloths)

bc = BillCounter(selectedCloths)

bc.display()

bc.delete()

bc.getTotal()

bc.getMax()

bc.getMin()

bc.getBrands()
