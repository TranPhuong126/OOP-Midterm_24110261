import math

class Point:
    def __init__(self, x=0, y=1):
        self.__x = x
        self.__y = y

    def read(self):
        data = input("Nhập tọa độ điểm B(x y): ").split()  
        self.__x = int(data[0])
        self.__y = int(data[1])

    def display(self):
        print(f"({self.__x}, {self.__y})")

    def move(self, dx, dy):
        self.__x += dx
        self.__y += dy

    def get_x(self):
        return self.__x

    def get_y(self):
        return self.__y

    def distance_to_origin(self):
        return math.sqrt(self.__x**2 + self.__y**2)

    def distance_to(self, other_point):
        dx = self.__x - other_point.get_x()
        dy = self.__y - other_point.get_y()
        return math.sqrt(dx**2 + dy**2)

class PointTest:
    
    def main():
        A = Point(3, 4)
        print("Tọa độ điểm A:")
        A.display()

        B = Point()
        B.read()  
        print("Tọa độ điểm B:")
        B.display()  

        C = Point(-B.get_x(), -B.get_y())
        print("Tọa độ điểm C (đối xứng với điểm B qua gốc tọa độ):")
        C.display()

        print("Khoảng cách từ điểm B đến gốc tọa độ:")
        print(B.distance_to_origin())

        print("Khoảng cách từ điểm A đến điểm B:")
        print(A.distance_to(B))

if __name__ == "__main__":
    PointTest.main()
