#include <iostream>
#include <fstream>
#include <string.h>
#include <conio.h>
#include <stdlib.h>

//..Made By Arian Miraki..//


using namespace std;

struct Hotel{
	string Name;
	string Family;
	int ID;
	int Age;
	float Date;
	int Phone;
	int age;
}HO[8];



main(){
	
	fstream file;
	file.open("Data Hotel Arian.txt",ios::app);
    cout<<"Welcome To ARIAN Hotel"<<endl;
    cout<<"......................"<<endl;
    for(int i;i<1000;i++){
    	
    	cout<<"PLS ENTER NAME: "<<endl;
    	cin>>HO[i].Name;
    	file<<"Name: "<<HO[i].Name<<endl;
    	
    	cout<<"PLS ENTER FAMILY: "<<endl;
    	cin>>HO[i].Family;
    	file<<"Family: "<<HO[i].Family<<endl;
    	
    	cout<<"PLS ENTER ID: "<<endl;
    	cin>>HO[i].ID;
    	file<<"ID: "<<HO[i].ID<<endl;
    	
    	cout<<"PLS ENTER AGE: "<<endl;
    	cin>>HO[i].Age;
    	file<<"Age: "<<HO[i].Age<<endl;
    	
    	cout<<"PLS ENTER DATE: "<<endl;
    	cin>>HO[i].Date;
    	file<<"Date: "<<HO[i].Date<<endl;
    	
    	cout<<"PLS ENTER PHONE: "<<endl;
    	cin>>HO[i].Phone;
    	file<<"Phone: "<<HO[i].Phone<<endl;
    	
    	return 0;
    	
	}
	file.close();
	getch();
    
}
