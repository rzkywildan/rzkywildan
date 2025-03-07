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

## Task3
function findThirdAngle(a, b) {
    if (a <= 0 || b <= 0 || a + b >= 180) {
        console.log("Invalid angles");
        return;
    }
    
    const thirdAngle = 180 - (a + b);
    console.log(`Third Angle: ${thirdAngle}`);
}

// Example usage
const angle1 = 80;
const angle2 = 65;
findThirdAngle(angle1, angle2);

## Task4
function dateDifference(date1, date2) {
    const d1 = new Date(date1);
    const d2 = new Date(date2);
    
    // Calculate difference in time (milliseconds)
    const timeDiff = Math.abs(d2 - d1);
    
    // Convert milliseconds to days
    const dayDiff = Math.ceil(timeDiff / (1000 * 60 * 60 * 24));
    
    console.log(`Difference in days: ${dayDiff}`);
}

// Example usage
const date1 = "2024-03-19";
const date2 = "2024-03-21";
dateDifference(date1, date2);

## Task5
function getInitials(name) {
    const words = name.split(" ");
    let initials = "";
    
    for (let word of words) {
        if (word.length > 0) {
            initials += word[0].toUpperCase();
        }
    }
    
    console.log(`Initials: ${initials}`);
}

// Example usage
const fullName = "John Doe";
getInitials(fullName);
