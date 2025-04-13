# abstract
abstract.java
abstract class Animal {
    // دالة مجردة (يجب تنفيذها في الأبناء)
    abstract void makeSound();

    // دالة عادية
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
        // Animal a = new Animal(); ❌ غير مسموح (كلاس مجرد)
        Cat c = new Cat();
        c.makeSound(); // Meow!
        c.eat();       // Animal eats food.
    }
}
