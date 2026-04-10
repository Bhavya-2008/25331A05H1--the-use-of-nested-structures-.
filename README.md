# 25331A05H1--the-use-of-nested-structures-.
#include <stdio.h> 
#include <string.h> 
struct Address { 
char city[30]; 
int pincode; 
}; 
struct Student { 
int roll_no; 
char name[50]; 
struct Address addr;  // Nested structure 
}; 
int main() { 
struct Student s1; 
// Assign values 
s1.roll_no = 101; 
strcpy(s1.name, "Bhavya"); 
strcpy(s1.addr.city, "VZM"); 
s1.addr.pincode = 535006; 
// Access members 
printf("Student Details:\n"); 
printf("Roll No: %d\n", s1.roll_no); 
printf("Name: %s\n", s1.name); 
printf("City: %s\n", s1.addr.city); 
printf("Pincode: %d\n", s1.addr.pincode);
return(0);
}
