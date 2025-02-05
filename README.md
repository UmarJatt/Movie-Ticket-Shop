# Movie-Ticket-Shop
#include<iostream>
using namespace std;
struct issue_date
{

    int dd,yy;
    string mm;
};

void anything()
{

    cout<<"There are three industrial movies avaliable \n1.hollywood\n2.bollywood\n3.lollywood"<<endl;
    int x;
    cin>>x;
    switch(x)
    {
    case 1:
        cout<<"HOLLYWOOD"<<endl;
      cout<<"1.Forrest Gump \t Hero: Tom Hanks"<<endl;
        cout<<"2.The Dark Knight \t Hero: Christian Bale as Batman/Bruce Wayne"<<endl;
        cout<<"3.Iron Man \t Hero: Robert Downey Jr. as Tony Stark/Iron Man"<<endl;
        cout<<"4.The Matrix \t Hero: Keanu Reeves as Neo"<<endl;
        cout<<"5.Gladiator \t Hero: Russell Crowe as Maximus"<<endl;
        int movienum;
        cin>>movienum;
        switch(movienum)
        {
        case 1:
            cout<<"Forrest Gump \t Hero: Tom Hanks";
            break;
        case 2:
            cout<<"The Dark Knight \t Hero: Christian Bale as Batman/Bruce Wayne";
            break;
        case 3:
            cout<<"Iron Man \t Hero: Robert Downey Jr. as Tony Stark/Iron Man";
            break;
        case 4:
            cout<<"The Matrix \t Hero: Keanu Reeves as Neo";
            break;
        case 5:
            cout<<"Gladiator \t Hero: Russell Crowe as Maximus";
            break;
        default:
            cout<<"Invalid";
            break;
        }
        break;
    case 2:
        cout<<"BOLLYWOOD"<<endl;
        cout<<"1.Dangal \t Hero: Aamir Khan"<<endl;
        cout<<"2.Bajrangi Bhaijaan \t Hero: Salman Khan"<<endl;
        cout<<"3.Padmaavat \t Hero: Ranveer Singhr"<<endl;
        cout<<"4.3 Idiots \t Hero: Aamir Khan"<<endl;
        cout<<"5.Kabir Singh \t Hero: Shahid Kapoor"<<endl;
        int movienumb;
        cin>>movienumb;
        switch(movienumb)
        {
        case 1:
            cout<<"Dangal \t Hero: Aamir Khan";
            break;
        case 2:
            cout<<"Bajrangi Bhaijaan \t Hero: Salman Khan";
            break;
        case 3:
            cout<<"Padmaavat \t Hero: Ranveer Singhr";
            break;
        case 4:
            cout<<"3 Idiots \t Hero: Aamir Khan";
            break;
        case 5:
            cout<<"Kabir Singh \t Hero: Shahid Kapoor";
            break;
        default:
            cout<<"Invlaid";
            break;

        }
        break;
    case 3:
        cout<<"LOLLYWOOD"<<endl;
        cout<<"1.Actor in Law \t Hero: Fahad Mustafa"<<endl;
        cout<<"2.Jawani Phir Nahi Ani \t Hero: Humayun Saeed"<<endl;
        cout<<"3.Teefa in Trouble \t Hero: Ali Zafar"<<endl;
        cout<<"4.Punjab Nahi Jaungi \t Hero: Humayun Saeed"<<endl;
        cout<<"5.Bin Roye \t Hero: Humayun Saeed"<<endl;
        int movienuml;
        cin>>movienuml;
        switch(movienuml)
        {
        case 1:
            cout<<"Actor in Law \t Hero: Fahad Mustafa";
            break;
        case 2:
            cout<<"Jawani Phir Nahi Ani \t Hero: Humayun Saeed";
            break;
        case 3:
            cout<<"Teefa in Trouble \t Hero: Ali Zafar";
            break;
        case 4:
            cout<<"Punjab Nahi Jaungi \t Hero: Humayun Saeed";
            break;
        case 5:
            cout<<"Bin Roye \t Hero: Humayun Saeed";
            break;
        default:
            cout<<"Invalid";
            break;

            break;
        }
    default:
        cout<<"Invalid";
        break;
    }

}
void everything() {
issue_date  x;
cout<<"You want to \n1.Purchase \n2.Issue"<<endl;
int y;
cin>>y;
switch(y){
case 1:
    cout<<"The prices of all movies are same i.e is :500$";
    break;


case 2:
cout <<"Enter the Issuing Date in dd/mm/yy: ";
cin >> x.dd >> x.mm >> x.yy;
cout<<endl<< "Issue Date: "<< x.dd<<"/"<<x.mm<<"/"<<x.yy<<endl;
cout<< "Due Date: "<< x.dd+3<<"/"<<x.mm<<"/"<<x.yy<<endl;
int date;
cout<<"Enter recieved date :";
cin>>date;
if(date==x.dd||date==x.dd+1||date==x.dd+2||date==x.dd+3)
{
    cout<<"No penalty: ";
}
else if (date>x.dd+3)
{

    cout<<"You got Penalty : "<<(date-(x.dd+3))*50<<" because you give it late";
}

else
{
    cout<<"Invalid";
}
break;
default:
    cout<<"Invalid";
    break;
}
}

int main()
{
    cout <<"                                          __________________________\n\n";
    cout << "                                             Video rental shop\n";
    cout <<"                                          __________________________\n\n";
    anything();
    everything();
    return 0;
}
