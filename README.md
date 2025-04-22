# Assignment.5
Create a constructor in both base and derived class. Use super() to call base class constructor in java?
// Base class
class Animal {
    String name;

    // Constructor of base class
    public Animal(String name) {
        this.name = name;
        System.out.println("Animal constructor called. Name: " + name);
    }
}

// Derived class
class Dog extends Animal {
    String breed;

    // Constructor of derived class
    public Dog(String name, String breed) {
        super(name); // Calling the constructor of the base class
        this.breed = breed;
        System.out.println("Dog constructor called. Breed: " + breed);
    }
}

// Main class to test the constructors
public class Main {
    public static void main(String[] args) {
        Dog myDog = new Dog("Buddy", "Golden Retriever");
    }
}
