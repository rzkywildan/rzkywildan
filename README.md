## Task1
public class Main {
  public static void main(String[] args) {
    int length = 5;  
    int width = 3;  
    int area = length * width;  
    System.out.println("Area of rectangle: " + area);  
  }
}
## Task2
function circleProperties(radius) {
    const diameter = 2 * radius;
    const circumference = 2 * Math.PI * radius;
    const area = Math.PI * Math.pow(radius, 2);

    console.log(`Diameter: ${diameter}`);
    console.log(`Circumference: ${circumference.toFixed(4)}`);
    console.log(`Area: ${area.toFixed(4)}`);
}

// Example usage
const radius = 5;
circleProperties(radius);
