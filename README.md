## Task1
function findArea(length, width) {
    return length * width;
}

// Input values
let length = 5;
let width = 3;

// Calculate and output the area
let area = findArea(length, width);
console.log("The area of the rectangle is: " + area);

## Task2
public class Circle {
    public static void main(String[] args) {
        // Given radius of the circle
        double radius = 5;
        
        // Calculate the diameter, circumference, and area
        double diameter = 2 * radius;
        double circumference = 2 * Math.PI * radius;
        double area = Math.PI * radius * radius;
        
        // Output the results
        System.out.println("Diameter: " + diameter);
        System.out.println("Circumference: " + String.format("%.4f", circumference));
        System.out.println("Area: " + String.format("%.3f", area));
    }
}
