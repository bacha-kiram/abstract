# abstract
abstract.java
abstract class Animal {
    abstract void makeSound();

    void eat() {
        System.out.println("Animal eats food.");
    }
}

class Cat extends Animal {
    void makeSound() {
        System.out.println("Meow!");
    }
}

class Main {
    public static void main(String[] args) {
        Cat c = new Cat();
        c.makeSound(); 
        c.eat();       
    }
}
