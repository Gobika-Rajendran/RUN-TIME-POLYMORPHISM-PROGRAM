# RUN-TIME-POLYMORPHISM-PROGRAM
package runtimepolymorphism;
class Animal{
    void sound(){
        System.out.println("Animal make a sound");
    }
}
class Dog extends Animal{
    void sound(){
        System.out.println("Dog barks");
    }
}
class Cat extends Animal{
    void sound(){
        System.out.println("Cat meows");
    }
}

public class RuntimePolymorphism {

    public static void main(String[] args) {
        // TODO code application logic here
        Animal myAnimal;
        myAnimal = new Dog();
        myAnimal.sound();
        
        myAnimal = new Cat();
        myAnimal.sound();
    }
    
}

OUTPUT
Dog barks
Cat meows

