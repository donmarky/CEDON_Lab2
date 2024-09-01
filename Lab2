import java.util.Scanner;

// Base class to represent a cylinder
class Cylinder {
    protected double radius;  // Radius of the cylinder
    protected double height;  // Height of the cylinder

    // Constructor to initialize the radius and height
    public Cylinder(double radius, double height) {
        this.radius = radius;
        this.height = height;
    }

    // Method to compute the surface area of the cylinder
    public double computeSurfaceArea() {
        return 2 * Math.PI * radius * (radius + height);
    }
}

// Derived class to compute the volume of the cylinder
class VolumeOfCylinder extends Cylinder {

    // Constructor to initialize the radius and height using the base class constructor
    public VolumeOfCylinder(double radius, double height) {
        super(radius, height);
    }

    // Method to compute the volume of the cylinder
    public double computeVolume() {
        return Math.PI * radius * radius * height;
    }
}

public class CylinderDemo {
    public static void main(String[] args) {
        // Create a Scanner object to read input from the user
        Scanner scanner = new Scanner(System.in);

        // Prompt the user to enter the radius and height of the cylinder
        System.out.print("Enter the radius of the cylinder: ");
        double radius = scanner.nextDouble();
        System.out.print("Enter the height of the cylinder: ");
        double height = scanner.nextDouble();

        // Create an instance of VolumeOfCylinder with the user-provided radius and height
        VolumeOfCylinder cylinder = new VolumeOfCylinder(radius, height);
        System.out.println();


        // Compute and print the surface area and volume of the cylinder
        System.out.println("Surface Area of the Cylinder: " + cylinder.computeSurfaceArea());
        System.out.println("Volume of the Cylinder: " + cylinder.computeVolume());

        // Close the scanner
        scanner.close();
    }
}
