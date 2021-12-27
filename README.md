# Pure-virtual-funcation
#include<iostream>
using namespace std;
class A{
	public:
		void virtual show()=0;
};
class B:public A{
		public:
		void show(){
			cout<<"child class b"<<endl;
		}
	
};
class C:public A{
		public:
		void show(){
			cout<<"child class C"<<endl;
		}
	
};
int main(){
	
	int op;
	A *ptr[5];
	B ob1;
	C ob2;
	for(int i=1;i<=5;i++){
		cout<<"Enter 1 for parent class\nEnter 2 for child class\nEnter 3 for child2"<<endl;
		cin>>op;
		if(op==1){
			//	ptr[i]=&ob;
	ptr[i]->show();
		
			
		}
		else if(op==2){
		//	ptr[i]=&ob1;
	
	ptr[i]=&ob1;
	ptr[i]->show();

		}
		else {
				ptr[i]=&ob2;
	ptr[i]->show();
	
		}
		
	

}
	return 0;
}
