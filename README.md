# project3
class vehicle
{
    public string Brand;
    public int Year;
    public vehicle(string brand, int year)
    {
        Brand = brand;
        Year = year;
    }
    public void start()
    {
        Console.WriteLine(Brand + "is starting.");
    }
}
class Car: vehicle
{
    public int NumberOfDoors;
        public Car(string brand, int year, int numberOfDoors):base(brand, year)
    {
        NumberOfDoors = numberOfDoors;
    }
}
class Bus: vehicle
{
    public int Capacity;
    public Bus(string brand, int year, int capacity) : base(brand, year)
    {
        Capacity = capacity;
    }
}
class Motorcycle: vehicle
{
    public bool HasSidecare;
    public Motorcycle(string brand, int year, bool hasSidecare) : base(brand, year)
    {
        HasSidecare = hasSidecare;
    }
}
class program
{
    static void Main(string[]args)
    {
        Car car = new Car("Toyota", 2022, 4);
        Bus bus = new Bus("Mercedes", 2020, 50);
        Motorcycle motorcycle = new Motorcycle("Honda", 2023, false);
        car.start();
        bus.start();
        motorcycle.start();
    }
}
OUTPUT:
Toyotais starting.
Mercedesis starting.
Hondais starting.