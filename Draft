#include<iostream>
using namespace std;
class member{
private:
    string name,id;
public:
    member(){
    name=' ';
    id='0000-0-00-000';}
    void set(){
    cout<<"Enter Name:";
    cin>>name;
    cout<<endl<<"Enter ID Number:";
    cin>>id;
    }
    void get(){
    cout<<endl<<"Name : "<<name;
    cout<<endl<<"ID : "<<id;
    }
};
class Income{
public:
    float tax(float inc){
    float yearlyIncome;
    yearlyIncome=inc*12;
    if(yearlyIncome>=250000 && yearlyIncome<=400000){
        return (yearlyIncome*.1);
    }
    else if(yearlyIncome>400000 && yearlyIncome<=500000){
        return (yearlyIncome*.15);
    }
    else if(yearlyIncome>500000 && yearlyIncome<=600000){
        return (yearlyIncome*.2);
    }
    else if(yearlyIncome>600000 && yearlyIncome<=3000000){
        return (yearlyIncome*.25);
    }
    else if(yearlyIncome>3000000){
        return (yearlyIncome*.30);
    }
    else
        return 0;
}
};

class boardMember: public member,public Income{
private:
    string position;
    float income;
public:

    boardMember(){
        position='member';
    }
    void set(){
    member::set();
    cout<<endl<<"Enter position of the board member";
    cin>>position;
    cout<<endl<<"Enter monthly income:";
    cin>>income;
    }
    void get(){
    member::get();
    cout<<endl<<"Position:"<<position;
    float tTax=Income::tax(income);
    cout<<endl<<"Income tax:"<<tTax;
    }

};
class serviceHolder:public member{
private:
    string position;
public:
    serviceHolder(){
    position='Employee';
    }
    void set(){
        member::set();
        cout<<endl<<"Enter Position of the service holder";
        cin>>position;
    }
    string get(){
    member::get();
    cout<<endl<<"Position:"<<position;
    return position;
    }
};
class student:public member{
private:
    string degree;
public:
    student(){
    degree='Bachelor';
    }
    void set(){
        member::set();
        cout<<endl<<"Enter the Degree:";
        cin>>degree;
    }
    string get(){
        member::get();
        cout<<endl<<"Degree:"<<degree;
        return degree;
    }

};
class security:public member{
private:
    int shift;
    string agency;
    float income;
public:
    security(){
    shift=0;
    agency=' ';
    }
    void set(){
        member::set();
        cout<<endl<<"Enter Shift:";
        cin>>shift;
        cout<<endl<<"Enter Agency:";
        cin>>agency;
        cout<<endl<<"Enter monthly income:";
        cin>>income;
    }
    void get(){
        member::get();
        cout<<endl<<"Shift:"<<shift<<endl<<"Agency:"<<agency;

    }

};
class faculty:public member{
private:
    string subject,position;
    int roomNumber;
    float income;
public:
    faculty(){
    subject='CSE';
    position='lecturer';

    }
    void set(){
        member::set();
        cout<<endl<<"Enter Subject:";
        cin>>subject;
        cout<<endl<<"Enter Position:";
        cin>>position;
        cout<<endl<<"Enter Room Number:";
        cin>>roomNumber;
        cout<<endl<<"Enter monthly income:";
        cin>>income;

    }
    void get(){
        member::get();
        cout<<endl<<"Subject:"<<subject;
        cout<<endl<<"Position:"<<position;

    }

};
class doctor:public serviceHolder{
private:
    string specialist;
    float income;
public:
    doctor(){
    specialist='medicine';
    }
    void set(){
    serviceHolder::set();
    cout<<endl<<"Doctors's specialty:";
    cin>>specialist;
    cout<<endl<<"Enter monthly income:";
    cin>>income;
    }
    void get(){
    serviceHolder::get();
    cout<<endl<<"Specialist:"<<specialist;
    }
};
class officeStaff:public serviceHolder{
private:
    string position;
    float income;
public:
    officeStaff(){
    position='General';
    }
    void set(){
    serviceHolder::set();
    cout<<endl<<"Enter position of the staff:";
    cout<<position;
    cout<<endl<<"Enter monthly income:";
    cin>>income;
    }
    void get(){
    serviceHolder::get();
    cout<<endl<<"Position:"<<position;
    }
};
class messenger:public serviceHolder{
private:
    float income;
public:
    void set(){
    serviceHolder::set();
    cout<<endl<<"Enter monthly income:";
    cin>>income;
    }
    void get(){
    serviceHolder::get();
    }
};
class masters:public student{
private:
    string subject;
public:
    masters(){
    subject='MS';
    }
    void set(){
    student::set();
    cout<<endl<<"Enter the Subject:";
    cin>>subject;
    }
    void get(){
    student::get();
    cout<<endl<<"Subject:"<<subject;
    }
};
class bachelor:public student{
private:
    string subject;
    float cgpa;
public:
    bachelor(){
    subject='MS';
    cgpa=0;
    }
    void set(){
    student::set();
    cout<<endl<<"Enter the Subject:";
    cin>>subject;
    cout<<endl<<"Enter the Cgpa:";
    cin>>cgpa;
    }
    void get(){
    student::get();
    cout<<endl<<"Subject:"<<subject;
    cout<<endl<<"Cgpa"<<cgpa;
    }
};

int main(){

    boardMember b1;
    b1.set();
    b1.get();
    return 0;
}

