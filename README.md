#include <iostream.h> 

#include <conio.h> 

class Base { 

public: 

void displayBase() { 

cout<<"This is the base class\n"; 

} 

}; 

class DerivedSingle: public Base{ 

public: 

void displayDerivedSingle() { 

cout<<"This is the Derived single class using single inheritance\n"; 

} 

}; 

class A { 

public: 

void displayA() { 

cout<<"This is the class A\n"; 

} 

}; 

class B { 

public: 

void displayB() { 

cout<<"This is the class B\n"; 
} 

}; 

class DerivedMultiple: public A, public B{ 

public: 

void displayDerivedMultiple(){ 

cout<<"This is the derived multiple class using multiple inheritance\n"; 

} 

}; 

class GrandParent{ 

public: 

void displayGrandParent(){ 

cout<<"This is the grandparent class\n"; 

} 

}; 

class Parent: public GrandParent{ 

public: 

void displayParent(){ 

cout<<"This is the parent class\n"; 

} 

}; 

class Child: public Parent{ 

public: 

void displayChild(){ 

cout<<"This is the child class\n"; 

}
}; 

class BaseForHierarchy{ 

public: 

void displayBaseForHierarchy(){ 

cout<<"This is the Base for hierarchy class\n"; 

} 

}; 

class Derived1: public BaseForHierarchy{ 

public: 

void displayDerived1(){ 

cout<<"This is the derived1 class\n"; 

} 

}; 

class Derived2: public BaseForHierarchy{ 

public: 

void displayDerived2(){ 

cout<<"This is the derived2 class\n"; 

} 

}; 

int main(){ 

DerivedSingle ds; 

ds. displayBase(); 

ds. displayDerivedSingle(); 

DerivedMultiple dm; 

dm. displayA(); 

dm. displayB(); 

dm. displayDerivedMultiple(); 

Child child; 

child. displayGrandParent(); 

child. displayParent(); 

child. displayChild(); 

Derived1 d1; 

Derived2 d2; 

d1. displayBaseForHierarchy(); 

d1. displayDerived1(); 

d2. displayBaseForHierarchy(); 

d2. displayDerived2(); 

getch(); 

return 0; 

}
