# 25331A05H1--the-use-of-nested-structures-.
#include <stdio.h>
struct Date {
    int day;
    int month;
    int year;
};
struct Student {
    int rollNo;
    char name[20];
    struct Date dob; 
};
int main() {
    struct Student s1 = {1, "Bhavya", {04,02,2008}};
    printf("Student: %s\n", s1.name);
    printf("DOB: %d/%d/%d\n", s1.dob.day, s1.dob.month, s1.dob.year);
    return 0;
}
