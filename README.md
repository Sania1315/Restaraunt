# Restaraunt
Restaurant System
#include <iostream>
#include <fstream>
#include <string>
#include <sstream>
#include <iomanip>
#include <stdlib.h> 
using namespace std;
class restauraunt { 
	    float price,p;
	    int order,deal,side_order,additional;
	    float final_bill=0;
	    string customer_type;
		void family_deal()
	{
            	cout<<"\n\n\t\t**** F A M I L Y  D E A L S ****";
 	cout<<"\n\n\t\t ----Deal_1---- \n\t>> Zinger Burger x 3------Rs.250/-";
 	cout<<"\n\t>> Large Fries x 3------Rs.180/-";
 	cout<<"\n\t>> Drinks : Coca Cola/7up/Fanta (500ml) x 3-----Rs.90/-";
 	cout<<"\n \t -_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-";
 	cout<<"\n\n\t\t ----Deal_2---- \n\t>> Fried Rice x 3------Rs.200/-";
 	cout<<"\n\t>> Chowmein x 3-----Rs.220/-";
 	cout<<"\n\t>> Drinks : Coca Cola/7up/Fanta (500ml) x 3-----Rs.90/-";
 	cout<<"\n\t  -_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-";
 	cout<<"\n\n\t\t ----Deal_3---- \n\t>> Loaded Fries  x 3------Rs.230/-";
 	cout<<"\n\t>> Paratha Roll x 3-----Rs.200/-";
 	cout<<"\n\t>> Drinks : Coca Cola/7up/Fanta (500ml) x 3-----Rs.90/-";
 	cout<<"\n   ******************************************************************** \n";
	}
	void kid_meal()
	{
cout<<"\n\t\t**** K I D S  D E A L S ****"; 	
    cout<<"\n\n\t\t ----Deal_1---- \n\t>> Mini Chicken Burger x 1------Rs.150/-";
 	cout<<"\n\t>> Small Fries x 1-----Rs.120/-";
 	cout<<"\n\t>> Mango Juice x 1-----Rs.40/-";	
 	cout<<"\n \t -_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-";
 	cout<<"\n\n\t\t ----Deal_2---- \n\t>> Nuggets x 5------Rs.180/-";
 	cout<<"\n\t>> Small Fries x 1-----Rs.120/-";
 	cout<<"\n\t>>  Mango Juice x 1-----Rs.40/-";	
 	cout<<"\n \t -_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-";
 	cout<<"\n\n\t\t ----Deal_3---- \n\t>> Club Sandwitch x 1------Rs.160/-";
 	cout<<"\n\t>> Cup Cake x 2-----Rs.80/-";
 	cout<<"\n\t>> Mango Juice x 1-----Rs.40/-";
 	cout<<"\n   ******************************************************************** \n";
	}
	void student_meal()
	{
            	cout<<"\n\t\t**** S T U D E N T   D E A L S ****";
 	
    cout<<"\n\t\t ----Deal_1---- \n\t>> Paratha Roll x 1------Rs.200/-";
 	cout<<"\n\t>> Drinks : Coca Cola/7up/Fanta (500ml) x 1-----Rs.90/-";
    cout<<"\n \t -_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-";
 	cout<<"\n\n\t\t ----Deal_2---- \n\t>> Shawarma x 1------Rs.150/-";
 	cout<<"\n\t>> Drinks : Coca Cola/7up/Fanta (500ml) x 1-----Rs.90/-";
 	cout<<"\n \t -_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-";
 	cout<<"\n\n\t\t ----Deal_3---- \n\t>> Biryani x 1------Rs.240/-";
 	cout<<"\n\t>> Drinks : Coca Cola/7up/Fanta (500ml) x 1-----Rs.90/-";
    cout<<"\n   ******************************************************************** \n";
	}
	void lunch_deal()
	{
            	cout<<"\n\t\t**** L U N C H  D E A L S ****";
 	            
 	cout<<"\n\n\t\t ----Deal_1---- \n\t>> Fried Rice x 2------Rs.200/-";
 	cout<<"\n\t>> Chowmein x 2-----Rs.220/-";
 	cout<<"\n\t>> Drinks : Coca Cola/7up/Fanta (500ml) x 2-----Rs.90/-";
 	cout<<"\n \t -_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-";
 	cout<<"\n\n\t\t ----Deal_2---- \n\t>> Biryani x 1------Rs.240/-";
    cout<<"\n\t>> Drinks : Coca Cola/7up/Fanta (500ml) x 1-----Rs.90/-";
    cout<<"\n \t -_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-";
 	cout<<"\n\n\t\t ----Deal_3---- \n\t>> Zinger Burger x 3------Rs.250/-";
 	cout<<"\n\t>> Large Fries x 3------Rs.180/-";
 	cout<<"\n\t>> Drinks : Coca Cola/7up/Fanta (500ml) x 3-----Rs.90/-";
    cout<<"\n   ******************************************************************** ";
   }
   void side_orders()
	{
            	cout<<"\n\t\t   **** S I D E  O R D E R S ****";
            	cout<<"\n   ******************************************************************** \n";
 	cout<<"\n\t 1- Fries x 1 (Large)                      Rs.200";
	cout<<"\n\t 2- Coffee                                   Rs.150";
	cout<<"\n\t 3- Shawarma x 1                             Rs.150";
	cout<<"\n\t 4- Drinks:Coca Cola/7up/Fanta (500ml) x 3   Rs.90";
	cout<<"\n\t 5- Dip Sauce x 1                            Rs.80";
	cout<<"\n\t 6- Cup Cake x 1                             Rs.20";
	cout<<"\n\t 7- Mango Juice x 1                          Rs.40";
	cout<<"\n\t 8- Loaded Fries x 1                         Rs.230";
	cout<<"\n\t 9- Nuggets x 5                              Rs.180";
	cout<<"\n\t 10- Paratha Roll x 1                        Rs.200";
	cout<<"\n   ****************************************************************** \n";
}
float set_price(int cho, int d)
{
	 if (cho==1)
	 {
	 	if(d==1)
	 	{
	 	price=(250*3)+(180*3)+(90*3);
	 	return price;}
	 	if(d==2)
	 	{
	 	price=(200*3)+(220*3)+(90*3);
	 	return price;}
	 	if(d==3)
	 	{
	 	price=(230*3)+(200*3)+(90*3);
	 	return price;}
	 }
    //Kids
     if (cho==2)
	 {
	 	if(d==1)
	 	{
	 	price=150+120+40;
	 	return price;}
	 	if(d==2)
	 	{
	 	price=180+120+40;
	 	return price;}
	 	if(d==3)
	 	{
	 	price=160+80+80+40;
	 	return price;}
	 }
	 //Student
	  if (cho==3)
	 {
	 	if(d==1)
	 	{
	 	price=200+90;
	 	return price;}
	 	if(d==2)
	 	{
	 	price=150+90;
	 	return price;}
	 	if(d==3)
	 	{
	 	price=240+90;
	 	return price;}
	 }
	 //Lunch
	  if (cho==4)
	 {
	 	if(d==1)
	 	{
	 	price=(200*2)+(220*2)+(90*2);
	 	return price;}
	 	if(d==2)
	 	{
	 	price=240+90;
	 	return price;}
	 	if(d==3)
	 	{
	 	price=(250*3)+(180*3)+(90*3);
	 	return price;}
	 }
	 //side
	  if (cho==5)
	 {
	 	if(d==1)
	 	{
	 	price=200;
	 	return price;}
	 	if(d==2)
	 	{
	 	price=150;
	 	return price;}
	 	if(d==3)
	 	{
	 	price=150;
	 	return price;}
	 		if(d==4)
	 	{
	 	price=90;
	 	return price;}
	 	if(d==5)
	 	{
	 	price=80;
	 	return price;}
	 	if(d==6)
	 	{
	 	price=20;
	 	return price;}
	 		if(d==7)
	 	{
	 	price=40;
	 	return price;}
	 	if(d==8)
	 	{
	 	price=230;
	 	return price;}
	 	if(d==9)
	 	{
	 	price=180;
	 	return price;}
	 	if(d==10)
	 	{
	 	price=200;
	 	return price;}
	 }
}
	public:
		restauraunt ()
		{
			price=0.00;
			order=7;
			deal=6;
			side_order=9;
			additional=9;
		}
		restauraunt (float p, int o, int d)
		{
			price=p;
			order=o;
			deal=d;
		}
		void display ()
		{
		cout<<"\n\n\t ******************************************************************** \n";
		cout<<"\t\t--------- Welcome to Shampoo's Resturant ----------"<<endl;
		cout<<"\t ******************************************************************** \n\n";
	    cout<<"\t\t _-_-_-_-_-_ M E N U  D I S P L A Y E D _-_-_-_-_-_ \n";
		cout<<"\t ******************************************************************** \n";
			family_deal();
	        kid_meal();
	        student_meal();
	        lunch_deal();
	        side_orders();
		}
		int orders()
		{   
		    cout<<"   ------------------------------------------------------";
		    cout<<"\n\t\t TIME TO PLACE YOU ORDER \n";
		    cout<<"   ------------------------------------------------------";
			cout<<"\n\n\t\tWhat do u want to eat ?";
 			cout<<"\n\n\t\t ~  Press 1 for Family Deals  ~  \n\t\t ~  Press 2 for Kid's Meals   ~ ";
 			cout<<"\n\t\t ~  Press 3 for Student Deals ~  \n\t\t ~  Press 4 for Lunch Deals   ~ ";
			cout<<"\n\t\t ~  Press 5 for Side Orders   ~  ";
			cout<<"\n   ---------------------------------------------------------------------";
			cout<<"\n\n\t\t\tEnter Nmuber here : ";
			cin>>order;
			cout<<"\n   ---------------------------------------------------------------------";
			system("cls") ;
			if (order == 1)
			{family_deal();}
			if (order ==2 )
			{kid_meal();}
			if (order ==3 )
			{student_meal();}
			if (order ==4)
			{lunch_deal();}
			if (order==1 || order==2 || order==3 || order==4)
			{ cout<<"\t \t ~  Press 1 for deal 1 !";
			 cout<<"\n\t \t ~  Press 2 for deal 2 !";
			 cout<<"\n\t \t ~  Press 3 for deal 3 !";
			 cout<<"\n   ---------------------------------------------------------------------";
			 cout<<"\n\t\tEnter Order here : ";
			 cin>>deal;
			cout<<"   --------------------------------------------------------------------- \n";
			 system("cls") ;
			p=set_price(order,deal);
			final_bill=final_bill+p;}
			if (order==5)
			{ side_orders();
			cout<<"\n\tKindly read the instructions carefully......... \n";
			cout<<" \n\t ~  Press 1 for Fries \n \t ~  Press 2 for Coffee \n";
			cout<<" \t ~  Press 3 for Shawarma \n \t ~  Press 4 for Drinks:Coca Cola/7up/Fanta (500ml)  \n";
			cout<<" \t ~  Press 5 for Dip Sauce \n \t ~  Press 6 for Cup Cake \n";
			cout<<" \t ~  Press 7 for Mango Juice \n \t ~  Press 8 for Loaded Fries \n";
			cout<<" \t ~  Press 9 for Nuggets \n \t ~  Press 10 for Paratha Roll \n";
    		cout<<"\n\t\t Enter Number here : ";
			cin>>side_order;
			system("cls") ;
			p=set_price(order,side_order);
			final_bill=final_bill+p;}
		}	
		int additional_orders()
		{
			cout<<" \n\t Do you want to continue or exit ? \n\n\t Press 1 to continue and 2 to exit :";
			cin>>additional;
			return additional;
		}	
		int display_bill()
		{
			cout<<"\n\tARE THEY SPECIAL CUSTOMERS OR NORMAL ? \n     WRITE Special for speical customers and Normal for normal customers : ";
			cin>>customer_type;
		if (customer_type=="Normal" || customer_type=="normal" )
			{
              cout<<"\t ---------------------------------------------------- \n";
			  cout<<"\t\t\t Total bill is : "<<final_bill<<endl;
			  cout<<"\t ---------------------------------------------------- \n";
		   }
				if (customer_type=="Special" || customer_type=="special")
		   {
		   	    cout<<"\n\t ----------------------------------------------------";
		   		cout<<"\n\n\t\t IS SPECIAL CUSTOMER A Teacher, A student, or disabled : ";
		   		cin>>customer_type;
			if (customer_type=="Teacher" || customer_type=="teacher")
		   		{
		   			final_bill=final_bill*0;
		   		cout<<"\t ---------------------------------------------------- \n";
		   		cout<<"\t\t\t Total bill is : "<<final_bill*0<<endl;
		   		cout<<"***************Your sacrifices don't go unnoticed*************\n";
		   		cout<<"\t\t\tEnjoy Your Meal :)\n";
		   		cout<<"\t ---------------------------------------------------- \n";
			    }
			if (customer_type=="Student" || customer_type=="student")
			    {
			    	final_bill=final_bill*0.5;
			    cout<<"\t ---------------------------------------------------- \n";
			   	cout<<"\t\t\tTotal bill is : "<<final_bill<<endl;
			   	cout<<"\t ---------------------------------------------------- \n";
				}
		 if (customer_type=="Disabled" || customer_type=="disabled")
			   	{
			   		final_bill=final_bill*0.7;
			   	cout<<"\t ---------------------------------------------------- \n";
			   	 cout<<"\t\t\t Total bill is : "<<final_bill<<endl;
			   	 cout<<"\t ---------------------------------------------------- \n";
				}
		   }
		}
};
struct node{
	string kitchen_items,amount;
	int price;
	node *next;
};
class Link{
	node *head=NULL;
	public:
	void insert(string n, int i, string d)
	{
		node *temp=head;
		while (temp != NULL)
		{
			if (temp->kitchen_items == n)
			{
				cout<<endl<<"\t Kitchen Item "<<temp->kitchen_items<<" already exist"<<endl;
				return;
			}
			temp=temp->next;
		}
		node *new_node = new node;
		if(head == NULL)
		{ 
			new_node->kitchen_items = n;
			new_node->price = i;
			new_node->amount = d;
			new_node->next=NULL;
			head=new_node;
		}
		else{
			node *temp=head;
			while(temp->next != NULL){
				temp=temp->next; 
			}
			new_node->kitchen_items = n;
			new_node->price = i;
			new_node->amount = d;
			new_node->next = NULL;
			temp->next = new_node;
		}
	}
		
	void display(){
		node *temp=head;
		while(temp!=NULL){
			cout<<" "<<temp->kitchen_items<<"\t\t\t"<<temp->price<<" \t\t\t\t"<<temp->amount<<endl;
			temp=temp->next;
		}
	}
};

int main() {
	restauraunt r1,r2(0.00,8,7),r;
	int add;
	string opt;
	cout<<"\tDo you want to display restauraunt information\n?";
    cout<<"Type yes To Display And anyother key to take orders : ";
    cin>>opt;
    if (opt=="yes" || opt=="Yes")
{
		Link list;
	int price;
	string kitchen_items,amount,opt;
	cout<<"\n   ---------------------------------------------------------------------\n"; 
	cout<<"\t\tInformation of Contracts Available "<<endl;
	cout<<"   ---------------------------------------------------------------------\n"; 
    cout<<"\t Do you want to insert any item in the list ?";
	cout<<"\n Type yes to insert any other key to display already existing List : ";
	cin>>opt;
	list.insert("White Bread",90000,"12 Packets");
	list.insert("Plane Chicken",212006,"12 Kilo");
	list.insert("Brown Chicken",212003,"12 Kilo");
	list.insert("Lamb Meat",211209,"17.5 Kilo");
	list.insert("Goat Meat",211205,"17.5 Kilo");
	list.insert("Cow Meat",211208,"17.5 Kilo");
	list.insert("Mushrooms",510000,"18 bottles");
	list.insert("Black Olives",55000,"15 bottles");
	list.insert("Mash Potatoes",58000,"17 kilo");
	list.insert("Organs Butter",51999,"15 kilo");
	list.insert("Dalda Oil",57000,"10 kilo");
	list.insert("Dalda Ghee",59000,"18 kilo");
	if (opt == "Yes" || opt=="yes")
	{
	while (opt!="NO")
{
	cout<<" ------------------------------------------------------------  "<<endl;
    cout<<"\t\tEnter Data of Kitchen Items"<<endl<<" ------------------------------------------------------------  "<<endl;
	cout<<"\t\tEnter Name of Food Item here : ";
	cin.ignore(50,'\n');
	getline(cin,kitchen_items);
	cout<<"\t\tEnter Price of item here: ";
	cin>>price;
	cout<<"\t\tEnter Amount available here : ";
	cin.ignore(60,'\n');
    getline(cin,amount);
		list.insert(kitchen_items,price,amount);
	cout<<"     Do You Want To Insert More Records ? \n Type NO to terminate : ";
	cin>>opt;
	cout<<"\n---------------------------------------------------------------------------";
cout<<"\nFood Item \t\t\t Price \t\t\t\t Amount \n";
	cout<<" --------------------------------------------------------------------------"<<endl;
list.display();
}
}
else
{ 
cout<<"\n---------------------------------------------------------------------------"<<endl;
cout<<"Food Item \t\t\t Price \t\t\t\t Amount \n";
cout<<"---------------------------------------------------------------------------"<<endl;
list.display();
}
  cout<<"\n\t\t Press 1 to display Kitchen Appliances & Bills and 2 to siplay Employee Records:  ";
  cin>>opt;
  if (opt=="1")
  {
    	cout<<cout<<"\n   ---------------------------------------------------------------------\n"; 
	cout<<"\t\tInformation of Kitchen Appliances & Bills"<<endl;
	cout<<"   ---------------------------------------------------------------------\n"; 
	int size=10;
string equipments[size];
string equipments_quantity[size];
int equipments_payment[size];
string line;
ifstream file3("Contract.csv");
int i=0;
while (getline(file3, line)) 
{
    string rand;
     istringstream iss(line);
    getline(iss, equipments[i], ',');
     getline(iss, equipments_quantity[i], ',');
    iss >> equipments_payment[i];
    getline(iss, rand, ',');
   i++;
}

cout<<"EQUIPMENTS"<<"\t\t\t"<<"QUANTITY"<<"\t\t\t"<<"PAYMENT"<<endl;
cout<<"---------------------------------------------------------------------------"<<endl;

for(int i=0;i<size;i++){
	
   cout<<equipments[i]<<"\t\t\t"<<equipments_quantity[i]<<"\t\t\t\t"<<equipments_payment[i]<<endl;
}
}
else
{
	int size=10;
string duty[size];
string name[size];
string pays[size];
int duty_hours[size];

   
string line;
ifstream file3("Employeee.csv");
int i=0;
while (getline(file3, line)) 
{
    string rand;
     istringstream iss(line); 
    getline(iss, duty[i], ',');
    getline(iss, name[i], ',');
    getline(iss,  pays[i], ',');
    iss >>  duty_hours[i];    
    i++;
}
cout<<"DUTY"<<"\t\t\t"<<"NAME"<<"\t\t\t\t"<<"PAYS"<<"\t\t\t"<<"DUTY HOURS"<<endl;
for(int i=0;i<size;i++)
cout<<duty[i]<<"\t\t\t"<<name[i]<<"\t\t\t"<<pays[i]<<"\t\t\t"<<duty_hours[i]<<endl;

}

}


else
    {
	do {
	r.display();
	r.orders();
	r.display_bill(); 
	add=r.additional_orders();
	system("cls") ;
	cout<<" \n ****************************************\n";
	cout<<"\t\tHAPPY MEAL \n\tSEE YOU SOON :)"<<endl;
	cout<<" ****************************************\n";
    } while (add!=2);
}
	return 0;
}
