# namespace-assignment

# Assignment : 

  The Galactic Navigation System

 # Scenario: 
 
 You are building a navigation system for a space station. Two different teams have written code for 

 "Coordinates":Team Solar: Uses (x, y, z) coordinates for positions within our solar system.
 
 Team DeepSpace: Uses (Sector, Quadrant) coordinates for locations outside our system.
 
 Without namespaces, your program would crash because the computer wouldn't know which Coordinate struct to use.
 
 # Part 1: 
 
 Setup the Namespaces. Create a header file or a section of your code containing two namespaces:
 
 Namespace Solar:
 
 a) Create a struct named Point containing three double variables: x, y, and z.
 
 b) Create a function print() that displays these values.
 
 Namespace DeepSpace:
 
 a) Create a struct named Point containing two int variables: sectorID and quadrantID.
 
 b) Create a function print() that displays these values.
 
 Part 2: The Main Logic. In your main() function, perform the following tasks:
 
 Direct Access: Use the scope resolution operator (::) to create one Solar::Point and one DeepSpace::Point.
 
 The using Declaration: Use a specific using declaration (not the whole namespace) so you can call the Solar version of print() without the Solar:: prefix.
 
 Namespace Aliasing: Create an alias for DeepSpace called DS. Use this alias to call the DeepSpace version of print().
 
 # Part 3: 
 
 The "Collision" Challenge
 
 Try to add using namespace Solar; and using namespace DeepSpace; at the same time at the top of your main function.
 
