class animal{
    public void specificanimal() {
    System.out.println("Chicken");
}
}
    
class Bird {
    public void makeSound() {
        System.out.println("Some bird sound");
    }
}

class Chicken extends Bird {
  
    public void makeSound() {
        System.out.println("Cock-a-doodle-doo!");
    }
}

public class Main {
    public static void main(String[] args) {
        Bird genericBird = new Bird();
        Chicken myChicken = new Chicken();
        animal myanimal = new animal();
 
        myanimal.specificanimal(); 
        genericBird.makeSound(); // Output: Some bird sound
        myChicken.makeSound();   // Output: Cock-a-doodle-doo!
    }
}
