<b>Part One</b>
<br><i>Create a class for vehicle. Each vehicle instance should have the following properties:</i>

make<br>
model<br>
year<br>
<p>Each vehicle instance should have access to a method called honk, which returns the string “Beep.”</p>

<p>let myFirstVehicle = new Vehicle("Honda", "Monster Truck", 1999);
<br>myFirstVehicle.honk(); // "Beep."
<br>Each vehicle instance should have a method called toString, which returns the string containing the make, model and year.</p>

<p>let myFirstVehicle = new Vehicle("Honda", "Monster Truck", 1999);
<br>myFirstVehicle.toString(); // "The vehicle is a Honda Monster Truck from 1999."
</p>
<p><b>Part Two</b>
<br><i>Create a class for a car. The Car class should inherit from Vehicle and each car instance should have a property called numWheels which has a value of 4.</i></p>

let myFirstCar = new Car("Toyota", "Corolla", 2005);<br>
myFirstCar.toString(); // "The vehicle is a Toyota Corolla from 2005."<br>
myFirstCar.honk();     // "Beep."<br>
myFirstCar.numWheels;  // 4</p>

<p><b>Part Three</b><br>
<i>Create a class for a Motorcycle. This class should inherit from Vehicle and each motorcycle instance should have a property called numWheels which has a value of 2. It should also have a revEngine method which returns “VROOM!!!”</i></p>

let myFirstMotorcycle = new Motorcycle("Honda", "Nighthawk", 2000);<br>
myFirstMotorcycle.toString(); // "The vehicle is a Honda Nighthawk from 2000."
<p>
myFirstMotorcycle.honk();     // "Beep."
myFirstMotorcycle.revEngine(); // "VROOM!!!"
myFirstMotorcycle.numWheels;  // 2
</p>
<br>
<p><b>Part Four</b><br>
<i>Create a class for a Garage. It should have a property called vehicles which will store an array of vehicles, and a property called capacity which is a number indicating how many vehicles will fit in the garage. When you create a garage, vehicles will always be empty; you only need to provide the capacity.</i></p>
<br>
<p><i>A garage should also have an add method, which attempts to add a vehicle to the array of vehicles. However, if you try to add something which is not a vehicle, the garage should return the message “Only vehicles are allowed in here!”. Also, if the garage is at capacity, it should say “Sorry, we’re full.”</i></p>
<br>
<p>let garage = new Garage(2);<br>
garage.vehicles; // []<br>
garage.add(new Car("Hyundai", "Elantra", 2015)); // "Vehicle added!"<br>
garage.vehicles; // [Car]<br>
garage.add("Taco"); // "Only vehicles are allowed in here!"<br></p>

<p>garage.add(new Motorcycle("Honda", "Nighthawk", 2000)); // "Vehicle added!"<br>
garage.vehicles; // [Car, Motorcycle]<br><br>
garage.add(new Motorcycle("Honda", "Nighthawk", 2001));// "Sorry, we're full."<br></p>
