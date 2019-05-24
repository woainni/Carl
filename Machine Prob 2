#include <iostream>
#include <math.h>

using namespace std;

int main(){
    int x1, y1, x2, y2, x3, y3, n = 3, intAngle;
    float a, b, c, area, perimeter, height, base, opp, adj, tangent, apothem, circumcircle; 
    double angle1, angle2, angle3;
    
    intAngle = ((n-2)*180); //formula to find the interior angle 
    cout << "Interior Angle: " << intAngle <<endl;
    
    cout << "Enter coordinates of the triangle.";
    cout << "\nEnter (x1, y1): ";
    cin >> x1 >> y1; // The user will input the first point (p1).
    cout << "\nEnter (x2, y2): ";
    cin >> x2 >> y2; // The user will input the second point (p2).  
    cout << "\nEnter (x3, y3): ";
    cin >> x3 >> y3; // The user will input the third point (p3).
    

    a = sqrt(pow((x1-x2),2.0)+pow((y1-y2),2.0)); //formula to find the length or distance between p1 and p2
    b = sqrt(pow((x2-x3),2.0)+pow((y2-y3),2.0)); //formula to find the length or distance between p2 and p3
    c = sqrt(pow((x3-x1),2.0)+pow((y3-y1),2.0)); //formula to find the length or distance between p3 and p1
    // a, b, c will be used to find the perimeter and to classify the triangle.    

     //Classifying the triangle:
     // all sides are equal
    if ((a==b)&&(b==c)){
        cout << "The triangle is equilateral." << endl;
    }
    
    // atleast 2 sides are equal
    else if ((a==b)||(b==c)){
        cout << "The triangle is isosceles." << endl;
    }
    
    // no sides are equal
    else{
        cout << "The triangle is scalene." << endl;
    }
    
    //Determining the area and perimeter of triangle:
    cout << "\nEnter base and height: ";
    cin >> base >> height; /* The user will input the base and heaight of triangle. 
    These will be used to find the area of the triangle. */
    
    area = 0.5*base*height; // formula to find the area of the triangle 
    perimeter = a + b + c; // formula to find the perimeter of the triangle
    
    cout << "Area: " << area << " squared units." <<endl;
    cout << "Perimeter: " << perimeter << " units." <<endl;
    
    
    //Classifying the type of triangle based on the angle:
    if (pow(a,2)+pow(b,2) > pow(c,2)){ //formula used to determine if it is an acute triangle by its side lengths
        cout << "It is classified as acute triangle." <<endl;
    }
    else if (pow(a,2)+pow(b,2) == pow(c,2)){ //formula used to determine if it is an right triangle by its side lengths
        cout << "It is classified as right triangle." <<endl;
    }
    else{
        cout << "It is classified as obtuse triangle." <<endl;
    }
    
    cout << "\nEnter opposite and adjacent side: ";
    cin >> opp >> adj; /* The user will input the opposite and adjacent side of triangle.
    These will be necessary to find the tangent which will be used in finding the apothem.*/
    
    tangent = opp/adj; //tangent will be used to find the apothem
    tangent = pow(tangent,-1.0); //formula to convert the tangent to degrees
    apothem = a/(2*tangent*(180/n)); //formula to find the apothem
    circumcircle = (a*b*c)/sqrt((a+b+c)*(b+c-a)*(c+a-b)*(a+b-c)); //formula to find the circumcircle
    
    cout << "Apothem: " <<apothem <<endl;
    cout << "Circumcircle: "<<circumcircle <<endl;
    
    return 0;
}
