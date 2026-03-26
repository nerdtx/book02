\newpage

## Homework Assignment: Classes, Inheritance, and Composition

### Overview:

In this assignment, you will build a system of airplane classes using Python’s
object-oriented programming features. You'll model different types of planes,
use inheritance for specialization, and apply composition to include components
like engines and weapons.

### Part 1: Define a Base `Airplane` Class

Create a class named `Airplane` with the following:

* Attributes: `tail_number`, `manufacturer`, `range_km`
* Methods:

  * `describe()` – prints basic information about the aircraft
  * `fly()` – prints: "`[tail_number] is taking off!`"
* Class Variable: `fleet_count` – keeps a count of all airplanes created

### Part 2: Create Subclasses for Passenger and Fighter Planes

Create two subclasses that inherit from `Airplane`:

#### `PassengerPlane`:

* Additional attributes: `seating_capacity`
* Override the `fly()` method to print: "`[tail_number] is boarding passengers
  and taking off.`"

#### `FighterPlane`:

* Additional attributes: `armament_type`
* Override the `fly()` method to print: "`[tail_number] is scrambling with
  weapons ready.`"
* Add a new method `engage()` that prints: "`[tail_number] is engaging with
  [armament_type].`"

### Part 3: Use Composition for Engines and Weapons

Create additional classes:

#### `JetEngine`:

* Attributes: `thrust_kn`, `manufacturer`
* Method: `start()` – prints: "`Engine by [manufacturer] generating [thrust_kn]
  kN of thrust.`"

#### `WeaponSystem` (used only by `FighterPlane`):

* Attributes: `missile_count`, `countermeasures`
* Method: `status()` – prints a summary of remaining missiles and
  countermeasures

Modify your `FighterPlane` class to accept and store instances of both
`JetEngine` and `WeaponSystem` as part of its initialization (i.e.,
composition).

### Part 4: Demonstrate Inheritance, Polymorphism, and Composition

Write a short script that does the following:

* Creates multiple `PassengerPlane` and `FighterPlane` instances
* Stores them in a list
* Iterates over the list and calls `fly()` on each plane (demonstrates
  **polymorphism**)
* Calls component methods (e.g., `start()`, `status()`) from composed objects

### Bonus Challenge (Optional)

* Add a `to_dict()` method to each plane that returns all relevant data, including information from composed objects.
* Track how many `PassengerPlane` and `FighterPlane` objects were created using
  class variables on those subclasses.

### Submission

* Submit one `.py` file with:

  * All class definitions
  * Clear labels for each part using comments
  * Demonstration code at the bottom with `print()` statements showing that each
    part works

