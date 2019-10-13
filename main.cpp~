#include <iostream>

using namespace std;

class day
{
    int year,month,date,odd_days;
public:
    void getdata()
    {
        cout<<"\nEnter date : ";
        cin>>date;
        cout<<"\nEnter Month number : ";
        cin>>month;
        cout<<"\nEnter year : ";
        cin>>year;
    }
    void display()
    {
        cout<<"\nEntered Date is : ";
        cout<<date<<"-"<<month<<"-"<<year<<endl;
    }
    int calculate_previous()
    {
        int a,rem,rem1,d,e,f,g,h,h1,odd;
        a=year-1;
        rem=a%400;
        rem1=rem%100;
        d=rem/100;
        e=d*100;
        f=rem1/4;
        g=rem1-f;
        h=f*2+g*1;
        if(e==100)
            h1=5;
        else if(e==200)
            h1=3;
        else if(e==300)
            h1=1;
        else
            h1=0;
        odd=h+h1;
        return odd;

    }
    void calculate()
    {
        int i,j,odd1;
        i=month-1;
        if(year%4!=0)
        {
            if(i==1)
                j=3;
            else if(i==2)
                j=3;
            else if(i==3)
                j=6;
            else if(i==4)
                j=8;
            else if(i==5)
                j=11;
            else if(i==6)
                j=13;
            else if(i==7)
                j=16;
            else if(i==8)
                j=19;
            else if(i==9)
                j=21;
            else if(i==10)
                j=24;
            else if(i==11)
                j=26;
            else if(i==0)
                j=0;
        }
        else
        {
            if(i==1)
                j=3;
            else if(i==2)
                j=4;
            else if(i==3)
                j=7;
            else if(i==4)
                j=9;
            else if(i==5)
                j=12;
            else if(i==6)
                j=14;
            else if(i==7)
                j=17;
            else if(i==8)
                j=20;
            else if(i==9)
                j=22;
            else if(i==10)
                j=25;
            else if(i==11)
                j=27;
            else if(i==0)
                j=0;
        }
        odd1 = j+date;
        odd_days = odd1+calculate_previous();
        if(odd_days%7==0)
            cout<<"\nSunday";
        else if(odd_days%7==1)
            cout<<"\nMonday";
        else if(odd_days%7==2)
            cout<<"\nTuesday";
        else if(odd_days%7==3)
            cout<<"\nWednesday";
        else if(odd_days%7==4)
            cout<<"\nThursday";
        else if(odd_days%7==5)
            cout<<"\nFriday";
        else if(odd_days%7==6)
            cout<<"\nSaturday";

        cout<<"\n";
    }
};
int main()
{
    day d;
    int ch;
    cout<<"\n\nProject for Calculation of Day present at particular Date\n";
    do
    {
        cout<<"\nSelect Operation\n";
        cout<<"1: Date Entry to find day\n";
        cout<<"2: Display Entered date\n";
        cout<<"3: Calculate Day\n";
        cout<<"4: Exit\n";
        cout<<"Enter Your Choice : ";
        cin>>ch;
        switch(ch)
        {
            case 1: d.getdata();
                    break;
            case 2: d.display();
                    break;
            case 3: d.calculate();
                    break;
            case 4: break;

        }
    }while(ch!=4);

    return 0;
}
