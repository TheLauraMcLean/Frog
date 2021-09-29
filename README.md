public class Frog {

    String name = "Name_not_set";
    int id = -1;
    int age = 0;
    String D;


    Frog(String theName, int theId, int theAge) {
        name = theName;
        id = theId;
        age = theAge;

    }

    void print() {
        System.out.println("**** Start of print method ******");
        System.out.println("Frog's name is " + name);
        System.out.println("Id  is " + id);

    }

    void printagegroup() {
        if (age < 22) {
            D = ("young");
        } else if (age < 50) {
            D = ("juvenile");
        } else if (age > 50) {
            D = ("adult");
        }
        System.out.println("Age group is " + D);

    }

    void reversedname() {

        char[] DE = name.toCharArray();
        for (int i = 0; i < name.length(); i++) {
            switch (name.charAt(i)) {
                case 'a':
                    System.out.print("i");
                    break;
                case 'n':
                    System.out.print("i");
                    break;
                case 'r':
                    System.out.print("o");
                    break;
                case 'F':
                    System.out.print("o");
                    break;
                default:
                    System.out.print(name.charAt(i));
            }

        }


    }
}






public class FrogProgram {

    public static void main(String[] args) {
        Frog myFrog = new Frog("Fred",1000,22);
        myFrog.print();
        myFrog.printagegroup();

        Frog myFrog2 = new Frog("Fran",1001,75);
        myFrog2.print();
        myFrog2.printagegroup();

        myFrog.reversedname();
        System.out.println();
        myFrog2.reversedname();

        }
    }
