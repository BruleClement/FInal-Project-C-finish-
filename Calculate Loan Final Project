#include <iostream>
#include <cmath>
#include <time.h>
#include <cstdlib>
#include <stdio.h>
#include <math.h>
#include <stdlib.h>
#include <fstream>
#include <iomanip>
#include <string>





using namespace std;

/*
 *
 */



int Enter_date_starting_month()
{
    int month=0;
    cout<<"\x1b[32;40m Enter the date you want to start the credit : \x1b[0m"<<endl;
    cout<<"\x1b[32;40m                                                                  \x1b[0m"<<endl;
    cout<<"\x1b[32;40m Enter the Month you want to start the credit : (Exemple 8) \x1b[0m";
    cout<<" ";

    while (!(cin >> month))
    {
        cerr << "\x1b[31;40m  Thanks enter a valid number \x1b[0m" << endl;
        cin.clear();
        cin.ignore(1);
    }

    cout<<"\x1b[32;40m                                                                  \x1b[0m"<<endl;

    if((month>12)||(month<1))
    {
        cout<<"\x1b[31;40m The starting Month is not good try again with an other date\x1b[0m"<<endl;
        month=Enter_date_starting_month();
    }

    return month;
}


int Enter_date_starting_year()
{
    int years=0;
    cout<<"\x1b[32;40m Enter the Year you want to start the credit : (Exemple 1964)\x1b[0m";
    cout<<" ";

    while (!(cin >> years))
    {
        cerr << "\x1b[31;40m  Thanks enter a valid number \x1b[0m" << endl;
        cin.clear();
        cin.ignore(1);
    }

    cout<<"\x1b[32;40m                                                                  \x1b[0m"<<endl;

    if(years<0)
    {
        cout<<"\x1b[31;40m The starting Year is not good try again with an other date \x1b[0m"<<endl;
        cout<<"\x1b[32;40m                                                                  \x1b[0m"<<endl;
        years=Enter_date_starting_year();
    }

    return years;
}

int Enter_date_starting_month_of_today()
{
    int month=0;
    cout<<"\x1b[32;40m You will enter the date of today : \x1b[0m"<<endl;
    cout<<"\x1b[32;40m                                                                  \x1b[0m"<<endl;
    cout<<"\x1b[32;40m Enter the month of Today : (Exemple 8) \x1b[0m";
    cout<<" ";

    while (!(cin >> month))
    {
        cerr << "\x1b[31;40m  Thanks enter a valid number \x1b[0m" << endl;
        cin.clear();
        cin.ignore(1);
    }

    cout<<"\x1b[32;40m                                                                  \x1b[0m"<<endl;

    if((month>12)||(month<1))
    {
        cout<<"\x1b[31;40m The Month of today is not good try again with an other date      \x1b[0m"<<endl;
        cout<<"\x1b[32;40m                                                                  \x1b[0m"<<endl;
        month=Enter_date_starting_month_of_today();
    }

    return month;
}

int Enter_date_starting_year_of_today()
{
    int years=0;
    cout<<"\x1b[32;40m Enter the Year of Today : (Exemple 1964) \x1b[0m";
    cout<<" ";

    while (!(cin >> years))
    {
        cerr << "\x1b[31;40m  Thanks enter a valid number \x1b[0m" << endl;
        cin.clear();
        cin.ignore(1);
    }

    cout<<"\x1b[32;40m                                                                  \x1b[0m"<<endl;

    if(years<0)
    {
        cout<<"\x1b[31;40m The Year of today is not good try again with an other date \x1b[0m"<<endl;
        years=Enter_date_starting_year_of_today();
    }

    return years;
}

string enterName()
{
    string Name;
    cout<<"\x1b[32;40m Enter your Name : \x1b[0m";
    cout<<" ";
    cin>>Name;
    cout<<"\x1b[32;40m                                                                  \x1b[0m"<<endl;

    return Name;
}

string enterFirstName()
{
    string FirstName;
    cout<<"\x1b[32;40m Enter your First Name : \x1b[0m";
    cout<<" ";
    cin>>FirstName;
    cout<<"\x1b[32;40m                                                                  \x1b[0m"<<endl;
    return FirstName;
}

double Enter_interestrate()
{
    double InterestRate=0;
    double InterestRateinpourcentage=0;
    cout<<"\x1b[32;40m Enter the Interest rate per year you want (in %)(per year) : \x1b[0m";
    cout<<" ";

    while (!(cin>>InterestRateinpourcentage))
    {
        cerr << "\x1b[31;40m  Thanks enter a valid number \x1b[0m" << endl;
        cin.clear();
        cin.ignore(1);
    }

    cout<<"\x1b[32;40m                                                                  \x1b[0m"<<endl;
    InterestRate=InterestRateinpourcentage/100;

    if((InterestRate>0.1)||(InterestRate<0))
    {
        cout << "\x1b[31;40m The Interest Rate is not legal, try Again With another Interest Rate \x1b[0m" << endl;
        cout<<"\x1b[32;40m                                                                  \x1b[0m"<<endl;
        InterestRate = Enter_interestrate();
    }

    return InterestRate;
}

int Enter_numberofperiod()
{
    int NumberOfperiod=0;

    cout<<"\x1b[32;40m Enter the Number of payment you want to pay your credit : \x1b[0m";
    cout<<" ";

    while (!(cin>>NumberOfperiod))
    {
        cerr << "\x1b[31;40m  Thanks enter a valid number \x1b[0m" << endl;
        cin.clear();
        cin.ignore(1);
    }

    cout<<"\x1b[32;40m                                                                  \x1b[0m"<<endl;

    if((NumberOfperiod>600)||(NumberOfperiod<0))
    {
        cout<<"\x1b[31;40m The Number of payment is not legal, try Again With another Number Of payment \x1b[0m"<<endl;
        cout<<"\x1b[32;40m                                                                  \x1b[0m"<<endl;
        NumberOfperiod=Enter_numberofperiod();
    }

    return NumberOfperiod;
}

double Enter_principal()
{
    double Principal=0;

    cout<<"\x1b[32;40m Enter the principal you want : \x1b[0m";
    cout<<" ";

    while (!(cin>>Principal))
    {
        cerr << "\x1b[31;40m  Thanks enter a valid number \x1b[0m" << endl;
        cin.clear();
        cin.ignore(1);
    }

    cout<<"\x1b[32;40m                                                                  \x1b[0m"<<endl;

    return Principal;
}

double Enter_openingbalance()
{
    double OpeningBalance=0;

    cout<<"\x1b[32;40m Enter the Opening Balance you want : \x1b[0m";
    cout<<" ";

    while (!(cin>>OpeningBalance))
    {
        cerr << "\x1b[31;40m  Thanks enter a valid number \x1b[0m" << endl;
        cin.clear();
        cin.ignore(1);
    }

    cout<<"\x1b[32;40m                                                                  \x1b[0m"<<endl;

    return OpeningBalance;
}

double Enter_instalment()
{
    double Instalment=0;
    cout<<"\x1b[32;40m Enter the instalment you want : \x1b[0m";
    cout<<" ";

    while (!(cin>>Instalment))
    {
        cerr << "\x1b[31;40m  Thanks enter a valid number \x1b[0m" << endl;
        cin.clear();
        cin.ignore(1);
    }

    cout<<"\x1b[32;40m                                                                  \x1b[0m"<<endl;
    return Instalment;

}

double Variable_Interest_Rate_mean()
{
    double IR_mean=0;
    cout<<"\x1b[32;40m Enter the Mean for the Interest Rate you want : \x1b[0m";
    cout<<" ";

    while (!(cin>>IR_mean))
    {
        cerr << "\x1b[31;40m  Thanks enter a valid number \x1b[0m" << endl;
        cin.clear();
        cin.ignore(1);
    }

    cout<<"\x1b[32;40m                                                                  \x1b[0m"<<endl;

    if(IR_mean>5)
    {
        cout<<"\x1b[31;40m The Mean of the Interest Rate is not legal, try again \x1b[0m"<<endl;
        cout<<"\x1b[32;40m                                                                  \x1b[0m"<<endl;
        IR_mean=Variable_Interest_Rate_mean();
    }
    return IR_mean;

}

double Variable_Interest_Rate_StDev()
{
    double IR_stDev=0;
    cout<<"\x1b[32;40m Enter the ST_DEV you want : \x1b[0m";
    cout<<" ";

    while (!(cin>>IR_stDev))
    {
        cerr << "\x1b[31;40m  Thanks enter a valid number \x1b[0m" << endl;
        cin.clear();
        cin.ignore(1);
    }

    cout<<"\x1b[32;40m                                                                  \x1b[0m"<<endl;

    if(IR_stDev>5)
    {
        cout<<"\x1b[31;40m The ST_DEV of the Interest Rate is not legal, try again \x1b[0m"<<endl;
        cout<<"\x1b[32;40m                                                                  \x1b[0m"<<endl;
        IR_stDev=Variable_Interest_Rate_StDev();
    }
    IR_stDev=IR_stDev/100;
    return IR_stDev;

}

double box_muller(double margin_constant, double Variance) {
    float Unif_Value1 , Unif_Value2, Normal_value=0;
    double Benchmark_rate=0;

    do {


        Unif_Value1 = 2.0 * ((float)rand()/RAND_MAX) - 1.0;
        Unif_Value2 = 2.0 * ((float)rand()/RAND_MAX) - 1.0;

        Normal_value = Unif_Value1 * Unif_Value1 + Unif_Value2 * Unif_Value2;
    } while (Normal_value >= 1.0);

    Normal_value = sqrt((-2.0 * log(Normal_value)) / Normal_value);
    Benchmark_rate = Unif_Value2 * Normal_value;
    Benchmark_rate=(double)(margin_constant+Benchmark_rate*Variance);



    return Benchmark_rate;
}


string frequency()
{
    string Frequence;
    cout<<"\x1b[32;40m Enter the Frequency you want pay your credit? (yearly/semi-annually/quarterly/monthly) \x1b[0m";
    cout<<" ";
    cin>>Frequence;

    if((Frequence=="yearly")||(Frequence=="Yearly")||(Frequence=="YEARLY"))
    {
        Frequence="yearly";


    }

    if((Frequence=="semi-annually")||(Frequence=="Semi-annually")||(Frequence=="Semi-Annually")||(Frequence=="semi-Annually")||(Frequence=="semi annually")||(Frequence=="Semi Annually")||(Frequence=="Semi annually")||(Frequence=="semi Annually")||(Frequence=="SEMI ANNUALLY")||(Frequence=="SEMI-ANNUALLY"))
    {
        Frequence="semi-annually";


    }

    if((Frequence=="quarterly")||(Frequence=="Quarterly")||(Frequence=="QUARTERLY"))
    {
        Frequence="quarterly";


    }

    if((Frequence=="monthly")||(Frequence=="Monthly")||(Frequence=="MONTHLY"))
    {
        Frequence="monthly";


    }

    if((Frequence!="monthly")&&(Frequence!="Monthly")&&(Frequence!="MONTHLY")&&(Frequence!="quarterly")&&(Frequence!="Quarterly")&&(Frequence!="QUARTERLY")&&(Frequence!="yearly")&&(Frequence!="Yearly")&&(Frequence!="YEARLY")&&(Frequence!="semi-annually")&&(Frequence!="Semi-annually")&&(Frequence!="Semi-Annually")&&(Frequence!="semi-Annually")&&(Frequence!="semi annually")&&(Frequence!="Semi Annually")&&(Frequence!="Semi annually")&&(Frequence!="semi Annually")&&(Frequence!="SEMI ANNUALLY")&&(Frequence!="SEMI-ANNUALLY"))
    {
        cout<<"\x1b[31;40m We can't read what you write you need try again \x1b[0m"<<endl;
        frequency();
    }
    return Frequence;

}


double frequency_Interest_rate(double InterestRate,string Frequence)
{


    if(Frequence=="semi-annually")
    {

        InterestRate=InterestRate/2;

    }
    else if(Frequence=="quarterly")
    {
        InterestRate=InterestRate/4;

    }
    else if(Frequence=="monthly")
    {
        InterestRate=InterestRate/12;

    }
    else
    {
        InterestRate=InterestRate;
    }
    return InterestRate;

}

void Fixed_OpeningBalance_InterestRate_Principal(double OpeningBalance,double InterestRate,double Principal,int Month,int Year,string Frequence)
{


    ofstream outData;
    outData.open("Final Project.csv",ios::app);
    outData<<endl;
    outData<<endl;
    /* First I create all variable I need on the Programm*/

    int NumberOfperiod=0;
    double Interest=0;
    double Instalment=0;
    double ClosingBalance=0;
    double SumPrincipal=0;

    /* I search How many time the person will need to pay*/

    NumberOfperiod=OpeningBalance/Principal;
    /* I Create the array*/

    outData<<";"<<"#"<<";"<<"Date"<<";"<<" Opening Balance "<<";"<<"Principal "<<";"<<" Interest Rate "<<";"<<" Interest "<<";"<<" Instalment "<<";"<<" Closing Balance "<<endl;
    outData<<";"<<"i"<<";"<<"D"<<";"<<"PVi-1"<<";"<<"Pi"<<";"<<"Ri"<<";"<<"INTi"<<";"<<"PMTi"<<";"<<"PVi"<<endl;


    /* I calculate year by year How many the person will need to pay*/

    for(int i=1;i<NumberOfperiod+1;i++)
    {
        Interest=OpeningBalance*InterestRate;
        Instalment=Principal+Interest;
        ClosingBalance=OpeningBalance-Principal;
        SumPrincipal=Principal+SumPrincipal;

        /* I Display the array*/

        outData<<";"<<i<<";"<<Month<<"/"<<Year<<";"<<OpeningBalance<<";"<<Principal<<";"<<InterestRate<<";"<<Interest<<";"<<Instalment<<";"<<ClosingBalance<<endl;
        OpeningBalance=ClosingBalance;
        if(Frequence=="semi-annually")
        {
            if(Month<=6)
            {
                Month=Month+6;
            }
            else
            {
                Month=Month+6-12;
                Year=Year+1;
            }



        }
        else if(Frequence=="quarterly")
        {
            if(Month<=8)
            {
                Month=Month+3;
            }
            else
            {
                Month=Month+3-12;
                Year=Year+1;
            }


        }
        else if(Frequence=="monthly")
        {
            if(Month<12)
            {
                Month=Month+1;
            }
            else
            {
                Month=Month+1-12;
                Year=Year+1;
            }


        }
        else if(Frequence=="yearly")
        {
            Year=Year+1;
        }
    }


    outData<<";;;;"<<SumPrincipal<<endl;
    outData<<endl;
}

void Fixed_OpeningBalance_InterestRate_NumberOfperiod(double OpeningBalance,double InterestRate,int NumberOfperiod,int Month,int Year,string Frequence)
{
    ofstream outData;
    outData.open("Final Project.csv",ios::app);
    outData<<endl;
    outData<<endl;
    /* First I create all variable I need on the Programm*/

    double Instalment=0;
    double Interest=0;
    double Principal=0;
    double ClosingBalance=0;
    double SumPrincipal=0;

    /* I search the Principal*/

    Principal=OpeningBalance/NumberOfperiod;

    /* I Create the array*/

    outData<<";"<<"#"<<";"<<"Date"<<";"<<" Opening Balance "<<";"<<"Principal "<<";"<<" Interest Rate "<<";"<<" Interest "<<";"<<" Instalment "<<";"<<" Closing Balance "<<endl;
    outData<<";"<<"i"<<";"<<"D"<<";"<<"PVi-1"<<";"<<"Pi"<<";"<<"Ri"<<";"<<"INTi"<<";"<<"PMTi"<<";"<<"PVi"<<endl;

    /* I calculate year by year How many the person will need to pay*/

    for(int i=1;i<NumberOfperiod+1;i++)
    {

        Interest=OpeningBalance*InterestRate;
        Instalment=Principal+Interest;
        ClosingBalance=OpeningBalance-Principal;
        SumPrincipal=Principal+SumPrincipal;

        /* I Display the array*/

        outData<<";"<<i<<";"<<Month<<"/"<<Year<<";"<<OpeningBalance<<";"<<Principal<<";"<<InterestRate<<";"<<Interest<<";"<<Instalment<<";"<<ClosingBalance<<endl;
        OpeningBalance=ClosingBalance;
        if(Frequence=="semi-annually")
        {
            if(Month<=6)
            {
                Month=Month+6;
            }
            else
            {
                Month=Month+6-12;
                Year=Year+1;
            }



        }
        else if(Frequence=="quarterly")
        {
            if(Month<=8)
            {
                Month=Month+3;
            }
            else
            {
                Month=Month+3-12;
                Year=Year+1;
            }


        }
        else if(Frequence=="monthly")
        {
            if(Month<12)
            {
                Month=Month+1;
            }
            else
            {
                Month=Month+1-12;
                Year=Year+1;
            }


        }
        else if(Frequence=="yearly")
        {
            Year=Year+1;
        }
    }
    outData<<";;;;"<<SumPrincipal<<endl;
    outData<<endl;
}

void Fixed_Principal_InterestRate_NumberOfperiod(double Principal, double InterestRate, int NumberOfperiod,int Month,int Year,string Frequence)
{
    ofstream outData;
    outData.open("Final Project.csv",ios::app);
    outData<<endl;
    outData<<endl;
    /* First I create all variable I need on the Programm*/

    double Instalment=0;
    double Interest=0;
    double OpeningBalance=0;
    double ClosingBalance=0;
    double SumPrincipal=0;

    /* I search the Principal*/

    OpeningBalance=Principal*NumberOfperiod;

    /* I Create the array*/

    outData<<";"<<"#"<<";"<<"Date"<<" Opening Balance "<<";"<<"Principal "<<";"<<" Interest Rate "<<";"<<" Interest "<<";"<<" Instalment "<<";"<<" Closing Balance "<<endl;
    outData<<";"<<"i"<<";"<<"D"<<";"<<"PVi-1"<<";"<<"Pi"<<";"<<"Ri"<<";"<<"INTi"<<";"<<"PMTi"<<";"<<"PVi"<<endl;

    /* I calculate year by year How many the person will need to pay*/

    for(int i=1;i<NumberOfperiod+1;i++)
    {
        Interest=OpeningBalance*InterestRate;
        Instalment=Principal+Interest;
        ClosingBalance=OpeningBalance-Principal;
        SumPrincipal=Principal+SumPrincipal;

        /* I Display the array*/

        outData<<";"<<i<<";"<<Month<<"/"<<Year<<";"<<OpeningBalance<<";"<<Principal<<";"<<InterestRate<<";"<<Interest<<";"<<Instalment<<";"<<ClosingBalance<<endl;
        OpeningBalance=ClosingBalance;
        if(Frequence=="semi-annually")
        {
            if(Month<=6)
            {
                Month=Month+6;
            }
            else
            {
                Month=Month+6-12;
                Year=Year+1;
            }



        }
        else if(Frequence=="quarterly")
        {
            if(Month<=8)
            {
                Month=Month+3;
            }
            else
            {
                Month=Month+3-12;
                Year=Year+1;
            }


        }
        else if(Frequence=="monthly")
        {
            if(Month<12)
            {
                Month=Month+1;
            }
            else
            {
                Month=Month+1-12;
                Year=Year+1;
            }


        }
        else if(Frequence=="yearly")
        {
            Year=Year+1;
        }
    }
    outData<<";;;;"<<SumPrincipal<<endl;
    outData<<endl;

}

void Fixed_OpeningBalance_InterestRate_Instalment(double OpeningBalance,double InterestRate,double Instalment,int Month,int Year,string Frequence)
{
    ofstream outData;
    outData.open("Final Project.csv",ios::app);
    outData<<endl;
    outData<<endl;
    /* First I create all variable I need on the Programm*/

    double Principal=0;
    double Interest=0;
    double ClosingBalance=0;
    double i=1;
    double SumPrincipal=0;

    outData<<";"<<"#"<<";"<<"Date"<<";"<<" Opening Balance "<<";"<<"Principal "<<";"<<" Interest Rate "<<";"<<" Interest "<<";"<<" Instalment "<<";"<<" Closing Balance "<<endl;
    outData<<";"<<"i"<<";"<<"D"<<";"<<"PVi-1"<<";"<<"Pi"<<";"<<"Ri"<<";"<<"INTi"<<";"<<"PMTi"<<";"<<"PVi"<<endl;

    /* I calculate year by year How many the person will need to pay*/

    for(OpeningBalance=OpeningBalance;OpeningBalance>Instalment*0.80;OpeningBalance=OpeningBalance-Principal)
    {
        Interest=OpeningBalance*InterestRate;
        Principal=Instalment-Interest;
        ClosingBalance=OpeningBalance-Principal;
        SumPrincipal=Principal+SumPrincipal;
        outData<<";"<<i<<";"<<Month<<"/"<<Year<<";"<<OpeningBalance<<";"<<Principal<<";"<<InterestRate<<";"<<Interest<<";"<<Instalment<<";"<<ClosingBalance<<endl;
        i=i+1;
        if(Frequence=="semi-annually")
        {
            if(Month<=6)
            {
                Month=Month+6;
            }
            else
            {
                Month=Month+6-12;
                Year=Year+1;
            }



        }
        else if(Frequence=="quarterly")
        {
            if(Month<=8)
            {
                Month=Month+3;
            }
            else
            {
                Month=Month+3-12;
                Year=Year+1;
            }


        }
        else if(Frequence=="monthly")
        {
            if(Month<12)
            {
                Month=Month+1;
            }
            else
            {
                Month=Month+1-12;
                Year=Year+1;
            }


        }
        else if(Frequence=="yearly")
        {
            Year=Year+1;
        }


    }
    outData<<";;;;"<<SumPrincipal<<endl;
    outData<<endl;



}

void Fixed_NumberOfperiod_InterestRate_Instalment(double NumberOfperiod,double InterestRate,double Instalment,int Month,int Year,string Frequence)
{
    ofstream outData;
    outData.open("Final Project.csv",ios::app);
    outData<<endl;
    outData<<endl;
    /* First I create all variable I need on the Programm*/


    double Principal=0;
    double Interest=0;
    double ClosingBalance=0;
    double SumPrincipal=0;

    outData<<";"<<"#"<<";"<<"Date"<<" Opening Balance "<<";"<<"Principal "<<";"<<" Interest Rate "<<";"<<" Interest "<<";"<<" Instalment "<<";"<<" Closing Balance "<<endl;
    outData<<";"<<"i"<<";"<<"D"<<";"<<"PVi-1"<<";"<<"Pi"<<";"<<"Ri"<<";"<<"INTi"<<";"<<"PMTi"<<";"<<"PVi"<<endl;

    /* I calculate the Opening Balance */

    double OpeningBalance=Instalment/(InterestRate*(1+(1/(pow(1+InterestRate,NumberOfperiod)-1))));


    /* I calculate year by year How many the person will need to pay*/

    for(int i=1;i<NumberOfperiod+1;i++)
    {
        Interest=OpeningBalance*InterestRate;
        Principal=Instalment-Interest;
        ClosingBalance=OpeningBalance-Principal;
        SumPrincipal=Principal+SumPrincipal;
        outData<<";"<<i<<";"<<Month<<"/"<<Year<<";"<<OpeningBalance<<";"<<Principal<<";"<<InterestRate<<";"<<Interest<<";"<<Instalment<<";"<<ClosingBalance<<endl;
        OpeningBalance=ClosingBalance;
        if(Frequence=="semi-annually")
        {
            if(Month<=6)
            {
                Month=Month+6;
            }
            else
            {
                Month=Month+6-12;
                Year=Year+1;
            }



        }
        else if(Frequence=="quarterly")
        {
            if(Month<=8)
            {
                Month=Month+3;
            }
            else
            {
                Month=Month+3-12;
                Year=Year+1;
            }


        }
        else if(Frequence=="monthly")
        {
            if(Month<12)
            {
                Month=Month+1;
            }
            else
            {
                Month=Month+1-12;
                Year=Year+1;
            }


        }
        else if(Frequence=="yearly")
        {
            Year=Year+1;
        }
    }
    outData<<";;;;"<<SumPrincipal<<endl;
    outData<<endl;

}

void Fixed_OpeningBalance_NumberOfperiod_Instalment(double OpeningBalance,double NumberOfperiod,double Instalment,int Month,int Year,string Frequence)
{


    ofstream outData;
    outData.open("Final Project.csv",ios::app);
    outData<<endl;
    outData<<endl;

    double InterestRate=0;
    double Interest=0;
    double Principal=0;
    double ClosingBalance=0;
    double SumPrincipal=0;



    InterestRate=(Instalment-(OpeningBalance/NumberOfperiod))/OpeningBalance;


    outData<<";"<<"#"<<";"<<"Date"<<";"<<" Opening Balance "<<";"<<"Principal "<<";"<<" Interest Rate "<<";"<<" Interest "<<";"<<" Instalment "<<";"<<" Closing Balance "<<endl;
    outData<<";"<<"i"<<";"<<"D"<<";"<<"PVi-1"<<";"<<"Pi"<<";"<<"Ri"<<";"<<"INTi"<<";"<<"PMTi"<<";"<<"PVi"<<endl;


    for(int i=1;i<NumberOfperiod+1;i++)
    {
        Interest=OpeningBalance*InterestRate;
        Principal=Instalment-Interest;
        ClosingBalance=OpeningBalance-Principal;
        SumPrincipal=Principal+SumPrincipal;

        /* I Display the array*/

        outData<<";"<<i<<";"<<Month<<"/"<<Year<<";"<<OpeningBalance<<";"<<Principal<<";"<<InterestRate<<";"<<Interest<<";"<<Instalment<<";"<<ClosingBalance<<endl;
        OpeningBalance=ClosingBalance;
        if(Frequence=="semi-annually")
        {
            if(Month<=6)
            {
                Month=Month+6;
            }
            else
            {
                Month=Month+6-12;
                Year=Year+1;
            }



        }
        else if(Frequence=="quarterly")
        {
            if(Month<=8)
            {
                Month=Month+3;
            }
            else
            {
                Month=Month+3-12;
                Year=Year+1;
            }


        }
        else if(Frequence=="monthly")
        {
            if(Month<12)
            {
                Month=Month+1;
            }
            else
            {
                Month=Month+1-12;
                Year=Year+1;
            }


        }
        else if(Frequence=="yearly")
        {
            Year=Year+1;
        }
    }


    outData<<";;;;"<<SumPrincipal<<endl;
    outData<<endl;
}


/* floating rate */
void Fixed_OpeningBalance_FloatInterestRate_Principal(double OpeningBalance,double MEAN,double ST_DEV,double Principal,int Month,int Year,string Frequence)
{


    ofstream outData;
    outData.open("Final Project.csv",ios::app);
    outData<<endl;
    outData<<endl;
    /* First I create all variable I need on the Programm*/

    int NumberOfperiod=0;
    double Interest=0;
    double Instalment=0;
    double ClosingBalance=0;
    double SumPrincipal=0;
    double FloatingRate=0;
    double InterestRate=0;
    srand(time(NULL));

    /* I search How many time the person will need to pay*/

    NumberOfperiod=OpeningBalance/Principal;

    /* I Create the array*/

    outData<<";"<<"#"<<";"<<"Date"<<";"<<" Opening Balance "<<";"<<"Principal "<<";"<<"Floating Rate"<<";"<<" Interest Rate "<<";"<<" Interest "<<";"<<" Instalment "<<";"<<" Closing Balance "<<endl;
    outData<<";"<<"i"<<";"<<"D"<<";"<<"PVi-1"<<";"<<"Pi"<<";"<<"Ri"<<";"<<"Fi"<<";"<<"INTi"<<";"<<"PMTi"<<";"<<"PVi"<<endl;


    /* I calculate year by year How many the person will need to pay*/

    for(int i=1;i<NumberOfperiod+1;i++)
    {

        FloatingRate=box_muller(MEAN,ST_DEV);
        InterestRate=FloatingRate+MEAN;
        Interest=OpeningBalance*InterestRate;
        Instalment=Principal+Interest;
        ClosingBalance=OpeningBalance-Principal;
        SumPrincipal=Principal+SumPrincipal;

        /* I Display the array*/

        outData<<";"<<i<<";"<<Month<<"/"<<Year<<";"<<OpeningBalance<<";"<<Principal<<";"<<FloatingRate<<";"<<InterestRate<<";"<<Interest<<";"<<Instalment<<";"<<ClosingBalance<<endl;
        OpeningBalance=ClosingBalance;
        if(Frequence=="semi-annually")
        {
            if(Month<=6)
            {
                Month=Month+6;
            }
            else
            {
                Month=Month+6-12;
                Year=Year+1;
            }



        }
        else if(Frequence=="quarterly")
        {
            if(Month<=8)
            {
                Month=Month+3;
            }
            else
            {
                Month=Month+3-12;
                Year=Year+1;
            }


        }
        else if(Frequence=="monthly")
        {
            if(Month<12)
            {
                Month=Month+1;
            }
            else
            {
                Month=Month+1-12;
                Year=Year+1;
            }


        }
        else if(Frequence=="yearly")
        {
            Year=Year+1;
        }
    }


    outData<<";;;;"<<SumPrincipal<<endl;
    outData<<endl;
}

void Fixed_OpeningBalance_FloatInterestRate_NumberOfperiod(double OpeningBalance,double MEAN,double ST_DEV,int NumberOfperiod,int Month,int Year,string Frequence)
{
    ofstream outData;
    outData.open("Final Project.csv",ios::app);
    outData<<endl;
    outData<<endl;
    /* First I create all variable I need on the Programm*/

    double Instalment=0;
    double Interest=0;
    double Principal=0;
    double ClosingBalance=0;
    double SumPrincipal=0;
    double FloatingRate=0;
    double InterestRate=0;
    srand(time(NULL));
    /* I search the Principal*/

    Principal=OpeningBalance/NumberOfperiod;

    /* I Create the array*/
    outData<<";"<<"#"<<";"<<"Date"<<";"<<" Opening Balance "<<";"<<"Principal "<<";"<<"Floating Rate"<<";"<<" Interest Rate "<<";"<<" Interest "<<";"<<" Instalment "<<";"<<" Closing Balance "<<endl;
    outData<<";"<<"i"<<";"<<"D"<<";"<<"PVi-1"<<";"<<"Pi"<<";"<<"Ri"<<";"<<"Fi"<<";"<<"INTi"<<";"<<"PMTi"<<";"<<"PVi"<<endl;


    /* I calculate year by year How many the person will need to pay*/

    for(int i=1;i<NumberOfperiod+1;i++)
    {
        FloatingRate=box_muller(MEAN,ST_DEV);
        InterestRate=FloatingRate+MEAN;
        Interest=OpeningBalance*InterestRate;
        Instalment=Principal+Interest;
        ClosingBalance=OpeningBalance-Principal;
        SumPrincipal=Principal+SumPrincipal;

        /* I Display the array*/

        outData<<";"<<i<<";"<<Month<<"/"<<Year<<";"<<OpeningBalance<<";"<<Principal<<";"<<InterestRate<<";"<<FloatingRate<<";"<<Interest<<";"<<Instalment<<";"<<ClosingBalance<<endl;
        OpeningBalance=ClosingBalance;
        if(Frequence=="semi-annually")
        {
            if(Month<=6)
            {
                Month=Month+6;
            }
            else
            {
                Month=Month+6-12;
                Year=Year+1;
            }



        }
        else if(Frequence=="quarterly")
        {
            if(Month<=8)
            {
                Month=Month+3;
            }
            else
            {
                Month=Month+3-12;
                Year=Year+1;
            }


        }
        else if(Frequence=="monthly")
        {
            if(Month<12)
            {
                Month=Month+1;
            }
            else
            {
                Month=Month+1-12;
                Year=Year+1;
            }


        }
        else if(Frequence=="yearly")
        {
            Year=Year+1;
        }
    }
    outData<<";;;;"<<SumPrincipal<<endl;
    outData<<endl;
}

void Fixed_Principal_FloatInterestRate_NumberOfperiod(double Principal, double MEAN,double ST_DEV, int NumberOfperiod,int Month,int Year,string Frequence)
{
    ofstream outData;
    outData.open("Final Project.csv",ios::app);
    outData<<endl;
    outData<<endl;
    /* First I create all variable I need on the Programm*/

    double Instalment=0;
    double Interest=0;
    double OpeningBalance=0;
    double ClosingBalance=0;
    double SumPrincipal=0;
    double FloatingRate=0;
    double InterestRate=0;
    srand(time(NULL));
    /* I search the Principal*/

    OpeningBalance=Principal*NumberOfperiod;

    /* I Create the array*/
    outData<<";"<<"#"<<";"<<"Date"<<";"<<" Opening Balance "<<";"<<"Principal "<<";"<<"Floating Rate"<<";"<<" Interest Rate "<<";"<<" Interest "<<";"<<" Instalment "<<";"<<" Closing Balance "<<endl;
    outData<<";"<<"i"<<";"<<"D"<<";"<<"PVi-1"<<";"<<"Pi"<<";"<<"Ri"<<";"<<"Fi"<<";"<<"INTi"<<";"<<"PMTi"<<";"<<"PVi"<<endl;


    /* I calculate year by year How many the person will need to pay*/

    for(int i=1;i<NumberOfperiod+1;i++)
    {
        FloatingRate=box_muller(MEAN,ST_DEV);
        InterestRate=FloatingRate+MEAN;
        Interest=OpeningBalance*InterestRate;
        Instalment=Principal+Interest;
        ClosingBalance=OpeningBalance-Principal;
        SumPrincipal=Principal+SumPrincipal;

        /* I Display the array*/

        outData<<";"<<i<<";"<<Month<<"/"<<Year<<";"<<OpeningBalance<<";"<<Principal<<";"<<FloatingRate<<";"<<InterestRate<<";"<<Interest<<";"<<Instalment<<";"<<ClosingBalance<<endl;
        OpeningBalance=ClosingBalance;
        if(Frequence=="semi-annually")
        {
            if(Month<=6)
            {
                Month=Month+6;
            }
            else
            {
                Month=Month+6-12;
                Year=Year+1;
            }



        }
        else if(Frequence=="quarterly")
        {
            if(Month<=8)
            {
                Month=Month+3;
            }
            else
            {
                Month=Month+3-12;
                Year=Year+1;
            }


        }
        else if(Frequence=="monthly")
        {
            if(Month<12)
            {
                Month=Month+1;
            }
            else
            {
                Month=Month+1-12;
                Year=Year+1;
            }


        }
        else if(Frequence=="yearly")
        {
            Year=Year+1;
        }
    }
    outData<<";;;;"<<SumPrincipal<<endl;
    outData<<endl;

}

void Fixed_OpeningBalance_FloatInterestRate_Instalment(double OpeningBalance,double MEAN,double ST_DEV,double Instalment,int Month,int Year,string Frequence)
{
    ofstream outData;
    outData.open("Final Project.csv",ios::app);
    outData<<endl;
    outData<<endl;
    /* First I create all variable I need on the Programm*/

    double Principal=0;
    double Interest=0;
    double ClosingBalance=0;
    double i=1;
    double SumPrincipal=0;
    double FloatingRate=0;
    double InterestRate=0;
    srand(time(NULL));
    outData<<";"<<"#"<<";"<<"Date"<<";"<<" Opening Balance "<<";"<<"Principal "<<";"<<"Floating Rate"<<";"<<" Interest Rate "<<";"<<" Interest "<<";"<<" Instalment "<<";"<<" Closing Balance "<<endl;
    outData<<";"<<"i"<<";"<<"D"<<";"<<"PVi-1"<<";"<<"Pi"<<";"<<"Ri"<<";"<<"Fi"<<";"<<"INTi"<<";"<<"PMTi"<<";"<<"PVi"<<endl;

    /* I calculate year by year How many the person will need to pay*/

    for(OpeningBalance=OpeningBalance;OpeningBalance>Instalment;OpeningBalance=OpeningBalance-Principal)
    {
        FloatingRate=box_muller(MEAN,ST_DEV);
        InterestRate=FloatingRate+MEAN;
        Interest=OpeningBalance*InterestRate;
        Principal=Instalment-Interest;
        ClosingBalance=OpeningBalance-Principal;
        SumPrincipal=Principal+SumPrincipal;

        outData<<";"<<i<<";"<<Month<<"/"<<Year<<";"<<OpeningBalance<<";"<<Principal<<";"<<FloatingRate<<";"<<InterestRate<<";"<<Interest<<";"<<Instalment<<";"<<ClosingBalance<<endl;

        i=i+1;
        if(Frequence=="semi-annually")
        {
            if(Month<=6)
            {
                Month=Month+6;
            }
            else
            {
                Month=Month+6-12;
                Year=Year+1;
            }



        }
        else if(Frequence=="quarterly")
        {
            if(Month<=8)
            {
                Month=Month+3;
            }
            else
            {
                Month=Month+3-12;
                Year=Year+1;
            }


        }
        else if(Frequence=="monthly")
        {
            if(Month<12)
            {
                Month=Month+1;
            }
            else
            {
                Month=Month+1-12;
                Year=Year+1;
            }


        }
        else if(Frequence=="yearly")
        {
            Year=Year+1;
        }


    }
    outData<<";;;;"<<SumPrincipal<<endl;
    outData<<endl;



}


void Introduction()
{
    cout<<"\x1b[92;100m    Hello my name is JARVIS I am a program helping you to calculate your bank loan. \x1b[0m"<<endl;
    cout<< "\x1b[32;40m                     I will do my best to guide you through the process             \x1b[0m"<<endl;
    cout<<endl;
    cout<<"                  ";

}


int All_Step() {

    /* First Step */



    string Name, FirstName, Sure;
    int monthofcredit, yearofcredit, monthoftoday, yearoftoday, NotunderstandSure = 0;

    cout << "\x1b[37;44m                  First step you have to answer some question  :) \x1b[0m" << endl;
    cout << "\x1b[32;40m                                                                  \x1b[0m" << endl;

    Name = enterName();
    FirstName = enterFirstName();
    monthoftoday = Enter_date_starting_month_of_today();
    yearoftoday = Enter_date_starting_year_of_today();
    monthofcredit = Enter_date_starting_month();
    yearofcredit = Enter_date_starting_year();

    if (yearoftoday > yearofcredit)
    {
        cout << "\x1b[31;40m it's impossible to do the credit enter an other year for starting the credit \x1b[0m"<< endl;
        yearofcredit = Enter_date_starting_year();
    }
    else if ((yearoftoday == yearofcredit) && (monthoftoday > monthofcredit))
    {
        cout << "\x1b[31;40m it's impossible to do the credit enter an other month for starting the credit \x1b[0m"<< endl;
        monthofcredit = Enter_date_starting_month();
    }

    cout << "\x1b[32;40m The information you have entered is : \x1b[0m" << endl;
    cout << "\x1b[37;40m Name                         : " << Name << "\x1b[0m" << endl;
    cout << "\x1b[37;40m FirstName                    : " << FirstName << "\x1b[0m" << endl;
    cout << "\x1b[37;40m Date of Today                : " << monthoftoday << "/" << yearoftoday << "\x1b[0m" << endl;
    cout << "\x1b[37;40m Date You want Start The Loan : " << monthofcredit << "/" << yearofcredit << "\x1b[0m" << endl;
    cout << "\x1b[32;40m                                                                  \x1b[0m" << endl;

    while (NotunderstandSure == 0)
    {
        cout << "\x1b[32;40m Do you agree with the information you have given us  (Yes/No) : \x1b[0m" << " ";
        cin >> Sure;
        if ((Sure == "Yes") || (Sure == "yes") || (Sure == "YES"))
        {
            NotunderstandSure = 1;

        }
        else if ((Sure == "No") || (Sure == "no") || (Sure == "NO"))
        {
            int Wichinformation = 0;

            cout << "\x1b[32;40m  Let's Start Again :)  \x1b[0m" << endl;
            cout << "\x1b[32;40m                                                                  \x1b[0m" << endl;
            cout << "\x1b[32;40m  what information do you want to change (Enter 1, 2, 3 or 4) \x1b[0m" << endl;
            cout << "\x1b[37;40m 1) Name                         : \x1b[0m" << endl;
            cout << "\x1b[37;40m 2) FirstName                    : \x1b[0m" << endl;
            cout << "\x1b[37;40m 3) Date of Today                : \x1b[0m" << endl;
            cout << "\x1b[37;40m 4) Date You want Start The Loan : \x1b[0m" << endl;
            cout << "\x1b[32;40m Enter : \x1b[0m";
            cout << " ";

            while (!(cin >> Wichinformation))
            {
                cerr << "\x1b[31;40m  Thanks enter a valid number \x1b[0m" << endl;
                cin.clear();
                cin.ignore(1);
            }

            cout << "\x1b[32;40m                                                                  \x1b[0m" << endl;


            if (Wichinformation == 1)
            {
                Name = enterName();
            }
            else if (Wichinformation == 2)
            {
                FirstName = enterFirstName();
            }
            else if (Wichinformation == 3)
            {
                monthoftoday = Enter_date_starting_month_of_today();
                yearoftoday = Enter_date_starting_year_of_today();

            }
            else if (Wichinformation == 4)
            {
                monthofcredit = Enter_date_starting_month();
                yearofcredit = Enter_date_starting_year();
            }


        }
        else
            {

            cout << "\x1b[32;40m Can you repeat please?  \x1b[0m" << endl;

            }
    }

    cout << "\x1b[32;40m                                                                  \x1b[0m" << endl;
    cout << "\x1b[32;40m The information The information you have entered are : \x1b[0m" << endl;
    cout << "\x1b[37;40m Name                         : " << Name << "\x1b[0m" << endl;
    cout << "\x1b[37;40m FirstName                    : " << FirstName << "\x1b[0m" << endl;
    cout << "\x1b[37;40m Date of Today                : " << monthoftoday << "/" << yearoftoday << "\x1b[0m" << endl;
    cout << "\x1b[37;40m Date You want Start The Loan : " << monthofcredit << "/" << yearofcredit << "\x1b[0m" << endl;
    cout << "\x1b[32;40m                                                                  \x1b[0m" << endl;

    ofstream outData;
    outData.open("Final Project.csv", ios::app);

    outData << endl;
    outData << ";" << "Name" << ";" << Name << endl;
    outData << ";" << "First Name" << ";" << FirstName << endl;
    outData << ";" << "Today" << ";" << monthoftoday << "/" << yearoftoday << endl;
    outData << ";" << "Start Month" << ";" << monthofcredit << "/" << yearofcredit << endl;



    /* Second Step */
    cout << "\x1b[32;40m                                                                  \x1b[0m" << endl;
    cout << "\x1b[37;44m                   Second Step                   \x1b[0m" << endl;
    cout << "\x1b[32;40m                                                                  \x1b[0m" << endl;

    int FloatingorFixedrate = 0;
    double ST_DEV = 0;
    double MEAN = 0;


    cout << "\x1b[32;40m You will have the choice between the different variable : \x1b[0m" << endl;
    cout << "       " << "\x1b[37;40m Interest Rate. \x1b[0m" << "       " << "\x1b[37;40m Number Of Payment. \x1b[0m"<< endl;
    cout << "       " << "\x1b[37;40m Principal      \x1b[0m" << "       " << "\x1b[37;40m Instalment.      \x1b[0m"<< endl;
    cout << "       " << "\x1b[37;40m             Opening Balance             \x1b[0m" << endl;
    cout << "\x1b[32;40m                                                                  \x1b[0m" << endl;
    cout << "\x1b[32;40m                                                                  \x1b[0m" << endl;

    while ((FloatingorFixedrate > 2) || (FloatingorFixedrate < 1)) {
        cout << "\x1b[32;40m  You have the choice between a floating Rate and a Fixed Rate \x1b[0m" << endl;
        cout << "\x1b[32;40m  (Enter the number corresponding to the Rate you choose) \x1b[0m" << endl;
        cout << "\x1b[32;40m  1) Fixed Rate \x1b[0m" << endl;
        cout << "\x1b[32;40m  2) Floating Rate \x1b[0m" << endl;
        while (!(cin >> FloatingorFixedrate))
        {
            cerr << "\x1b[31;40m  Thanks enter a valid number \x1b[0m" << endl;
            cin.clear();
            cin.ignore(1);
        }
        if (FloatingorFixedrate == 1)
        {
            int ChoiceFunction1 = 0;
            while ((ChoiceFunction1 > 6) || (ChoiceFunction1 < 1))
            {
                cout
                        << "\x1b[32;40m  You have the choice between Different Fixed Variable for calculate your loan  : \x1b[0m"<< endl;
                cout << "\x1b[32;40m  (Enter the number corresponding to the Rate you choose) \x1b[0m" << endl;
                cout << "\x1b[32;40m  1) Fixed OpeningBalance InterestRate Principal\x1b[0m" << endl;
                cout << "\x1b[32;40m  2) Fixed OpeningBalance InterestRate Number Of payment \x1b[0m" << endl;
                cout << "\x1b[32;40m  3) Fixed Principal InterestRate Number Of payment \x1b[0m" << endl;
                cout << "\x1b[32;40m  4) Fixed OpeningBalance InterestRate Instalment \x1b[0m" << endl;
                cout << "\x1b[32;40m  5) Fixed Number Of payment InterestRate Instalment \x1b[0m" << endl;
                cout << "\x1b[32;40m  6) Fixed OpeningBalance Number Of payment Instalment \x1b[0m" << endl;
                while (!(cin >> ChoiceFunction1))
                {
                    cerr << "\x1b[31;40m  Thanks enter a valid number \x1b[0m" << endl;
                    cin.clear();
                    cin.ignore(1);
                }
                cout << "\x1b[32;40m                                                                  \x1b[0m" << endl;

                if (ChoiceFunction1 == 1)
                {

                    cout << "\x1b[32;40m  You will now Enter the Value of the Different Variable : \x1b[0m" << endl;

                    double OpeningBalance = Enter_openingbalance();
                    double InterestRate = Enter_interestrate();
                    double Principal = Enter_principal();
                    double NotunderstandSure2 = 0;

                    cout << "\x1b[32;40m                                                                  \x1b[0m"<< endl;
                    cout << "\x1b[32;40m The information The information you have entered are : \x1b[0m" << endl;
                    cout << "\x1b[37;40m Opening Balance              : " << OpeningBalance << "\x1b[0m" << endl;
                    cout << "\x1b[37;40m Interest Rate                : " << InterestRate << "\x1b[0m" << endl;
                    cout << "\x1b[37;40m Principal               : " << Principal << "\x1b[0m" << endl;
                    cout << "\x1b[32;40m                                                                  \x1b[0m"<< endl;

                    while (NotunderstandSure2 == 0)
                    {
                        cout << "\x1b[32;40m Do you agree with the information you have given us  (Yes/No) : \x1b[0m"<< " ";
                        cin >> Sure;
                        if ((Sure == "Yes") || (Sure == "yes") || (Sure == "YES"))
                        {
                            NotunderstandSure2 = 1;

                        }
                        else if ((Sure == "No") || (Sure == "no") || (Sure == "NO"))
                        {
                            OpeningBalance = Enter_openingbalance();
                            InterestRate = Enter_interestrate();
                            Principal = Enter_principal();

                            cout
                                    << "\x1b[32;40m                                                                  \x1b[0m"<< endl;
                            cout << "\x1b[32;40m The information The information you have entered are : \x1b[0m"<< endl;
                            cout << "\x1b[37;40m Opening Balance              : " << OpeningBalance << "\x1b[0m"<< endl;
                            cout << "\x1b[37;40m Interest Rate                : " << InterestRate << "\x1b[0m" << endl;
                            cout << "\x1b[37;40m Principal               : " << Principal << "\x1b[0m" << endl;
                            cout<< "\x1b[32;40m                                                                  \x1b[0m"<< endl;

                        }
                        else
                            {

                            cout << "\x1b[32;40m Can you repeat please?  \x1b[0m" << endl;

                            }
                    }


                    outData << endl;
                    outData << ";" << "Opening Balance" << ";" << OpeningBalance << endl;
                    outData << ";" << "Interest Rate" << ";" << InterestRate << endl;
                    outData << ";" << "Principal" << ";" << Principal << endl;


                    string Frequence = frequency();
                    InterestRate = frequency_Interest_rate(InterestRate, Frequence);

                    outData << ";" << "Frequency" << ";" << Frequence << endl;
                    outData << endl;

                    Fixed_OpeningBalance_InterestRate_Principal(OpeningBalance, InterestRate, Principal, monthofcredit,yearofcredit, Frequence);


                }
                else if (ChoiceFunction1 == 2)
                {

                    cout << "\x1b[32;40m  You will now Enter the Value of the Different Variable : \x1b[0m" << endl;
                    double OpeningBalance = Enter_openingbalance();
                    double InterestRate = Enter_interestrate();
                    double NumberOfPayment = Enter_numberofperiod();
                    double NotunderstandSure2 = 0;

                    cout << "\x1b[32;40m                                                                  \x1b[0m"
                         << endl;
                    cout << "\x1b[32;40m The information The information you have entered are : \x1b[0m" << endl;
                    cout << "\x1b[37;40m Opening Balance              : " << OpeningBalance << "\x1b[0m" << endl;
                    cout << "\x1b[37;40m Interest Rate                : " << InterestRate << "\x1b[0m" << endl;
                    cout << "\x1b[37;40m Number Of Payment               : " << NumberOfPayment << "\x1b[0m" << endl;
                    cout << "\x1b[32;40m                                                                  \x1b[0m"
                         << endl;

                    while (NotunderstandSure2 == 0)
                    {
                        cout << "\x1b[32;40m Do you agree with the information you have given us  (Yes/No) : \x1b[0m"
                             << " ";
                        cin >> Sure;
                        if ((Sure == "Yes") || (Sure == "yes") || (Sure == "YES"))
                        {
                            NotunderstandSure2 = 1;

                        }
                        else if ((Sure == "No") || (Sure == "no") || (Sure == "NO"))
                        {
                            OpeningBalance = Enter_openingbalance();
                            InterestRate = Enter_interestrate();
                            NumberOfPayment = Enter_numberofperiod();
                            cout
                                    << "\x1b[32;40m                                                                  \x1b[0m"
                                    << endl;
                            cout << "\x1b[32;40m The information The information you have entered are : \x1b[0m"
                                 << endl;
                            cout << "\x1b[37;40m Opening Balance              : " << OpeningBalance << "\x1b[0m"
                                 << endl;
                            cout << "\x1b[37;40m Interest Rate                : " << InterestRate << "\x1b[0m" << endl;
                            cout << "\x1b[37;40m Number Of Payment              : " << NumberOfPayment << "\x1b[0m"
                                 << endl;
                            cout
                                    << "\x1b[32;40m                                                                  \x1b[0m"
                                    << endl;

                        }
                        else
                            {

                            cout << "\x1b[32;40m Can you repeat please?  \x1b[0m" << endl;

                            }
                    }


                    outData << endl;
                    outData << ";" << "Opening Balance" << ";" << OpeningBalance << endl;
                    outData << ";" << "Interest Rate" << ";" << InterestRate << endl;
                    outData << ";" << "Number Of Payment" << ";" << NumberOfPayment << endl;


                    string Frequence = frequency();
                    InterestRate = frequency_Interest_rate(InterestRate, Frequence);

                    outData << ";" << "Frequency" << ";" << Frequence << endl;
                    outData << endl;
                    Fixed_OpeningBalance_InterestRate_NumberOfperiod(OpeningBalance, InterestRate, NumberOfPayment,monthofcredit, yearofcredit, Frequence);


                }
                else if (ChoiceFunction1 == 3)
                {
                    cout << "\x1b[32;40m  You will now Enter the Value of the Different Variable : \x1b[0m" << endl;
                    double Principal = Enter_principal();
                    double InterestRate = Enter_interestrate();
                    double NumberOfPayment = Enter_numberofperiod();
                    double NotunderstandSure2 = 0;
                    cout << "\x1b[32;40m                                                                  \x1b[0m"
                         << endl;
                    cout << "\x1b[32;40m The information The information you have entered are : \x1b[0m" << endl;
                    cout << "\x1b[37;40m Number Of Payment             : " << NumberOfPayment << "\x1b[0m" << endl;
                    cout << "\x1b[37;40m Interest Rate                : " << InterestRate << "\x1b[0m" << endl;
                    cout << "\x1b[37;40m Principal              : " << Principal << "\x1b[0m" << endl;
                    cout << "\x1b[32;40m                                                                  \x1b[0m"
                         << endl;
                    while (NotunderstandSure2 == 0)
                    {
                        cout << "\x1b[32;40m Do you agree with the information you have given us  (Yes/No) : \x1b[0m"
                             << " ";
                        cin >> Sure;
                        if ((Sure == "Yes") || (Sure == "yes") || (Sure == "YES"))
                        {
                            NotunderstandSure2 = 1;

                        }
                        else if ((Sure == "No") || (Sure == "no") || (Sure == "NO"))
                        {
                            Principal = Enter_principal();
                            InterestRate = Enter_interestrate();
                            NumberOfPayment = Enter_numberofperiod();
                            cout
                                    << "\x1b[32;40m                                                                  \x1b[0m"
                                    << endl;
                            cout << "\x1b[32;40m The information The information you have entered are : \x1b[0m"
                                 << endl;
                            cout << "\x1b[37;40m Principal              : " << Principal << "\x1b[0m" << endl;
                            cout << "\x1b[37;40m Interest Rate                : " << InterestRate << "\x1b[0m" << endl;
                            cout << "\x1b[37;40m Number Of Payment              : " << NumberOfPayment << "\x1b[0m"
                                 << endl;
                            cout
                                    << "\x1b[32;40m                                                                  \x1b[0m"
                                    << endl;

                        }
                        else
                            {

                            cout << "\x1b[32;40m Can you repeat please?  \x1b[0m" << endl;

                        }
                    }


                    outData << endl;
                    outData << ";" << "Principal" << ";" << Principal << endl;
                    outData << ";" << "Interest Rate" << ";" << InterestRate << endl;
                    outData << ";" << "Number Of Payment" << ";" << NumberOfPayment << endl;


                    string Frequence = frequency();
                    InterestRate = frequency_Interest_rate(InterestRate, Frequence);

                    outData << ";" << "Frequency" << ";" << Frequence << endl;
                    outData << endl;
                    Fixed_Principal_InterestRate_NumberOfperiod(Principal, InterestRate, NumberOfPayment,monthofcredit, yearofcredit, Frequence);


                }
                else if (ChoiceFunction1 == 4)
                {

                    cout << "\x1b[32;40m  You will now Enter the Value of the Different Variable : \x1b[0m" << endl;
                    double OpeningBalance = Enter_openingbalance();
                    double InterestRate = Enter_interestrate();
                    double Instalment = Enter_instalment();
                    double NotunderstandSure2 = 0;

                    cout << "\x1b[32;40m                                                                  \x1b[0m"
                         << endl;
                    cout << "\x1b[32;40m The information The information you have entered are : \x1b[0m" << endl;
                    cout << "\x1b[37;40m Opening Balance              : " << OpeningBalance << "\x1b[0m" << endl;
                    cout << "\x1b[37;40m Interest Rate                : " << InterestRate << "\x1b[0m" << endl;
                    cout << "\x1b[37;40m Instalment               : " << Instalment << "\x1b[0m" << endl;
                    cout << "\x1b[32;40m                                                                  \x1b[0m"<< endl;

                    while (NotunderstandSure2 == 0) {
                        cout << "\x1b[32;40m Do you agree with the information you have given us  (Yes/No) : \x1b[0m"
                             << " ";
                        cin >> Sure;
                        if ((Sure == "Yes") || (Sure == "yes") || (Sure == "YES")) {
                            NotunderstandSure2 = 1;

                        } else if ((Sure == "No") || (Sure == "no") || (Sure == "NO")) {
                            OpeningBalance = Enter_openingbalance();
                            InterestRate = Enter_interestrate();
                            Instalment = Enter_instalment();
                            cout
                                    << "\x1b[32;40m                                                                  \x1b[0m"
                                    << endl;
                            cout << "\x1b[32;40m The information The information you have entered are : \x1b[0m"
                                 << endl;
                            cout << "\x1b[37;40m Opening Balance              : " << OpeningBalance << "\x1b[0m"
                                 << endl;
                            cout << "\x1b[37;40m Interest Rate                : " << InterestRate << "\x1b[0m" << endl;
                            cout << "\x1b[37;40m Instalment              : " << Instalment << "\x1b[0m" << endl;
                            cout
                                    << "\x1b[32;40m                                                                  \x1b[0m"
                                    << endl;

                        } else {

                            cout << "\x1b[32;40m Can you repeat please?  \x1b[0m" << endl;

                        }
                    }


                    outData << endl;
                    outData << ";" << "Opening Balance" << ";" << OpeningBalance << endl;
                    outData << ";" << "Interest Rate" << ";" << InterestRate << endl;
                    outData << ";" << "Instalment" << ";" << Instalment<< endl;


                    string Frequence = frequency();
                    InterestRate = frequency_Interest_rate(InterestRate, Frequence);

                    outData << ";" << "Frequency" << ";" << Frequence << endl;
                    outData << endl;
                    Fixed_OpeningBalance_InterestRate_Instalment(OpeningBalance, InterestRate, Instalment,monthofcredit, yearofcredit, Frequence);


                } else if (ChoiceFunction1 == 5) {
                    cout << "\x1b[32;40m  You will now Enter the Value of the Different Variable : \x1b[0m" << endl;

                    double NumberOfPayment = Enter_numberofperiod();
                    double InterestRate = Enter_interestrate();
                    double Instalment = Enter_instalment();
                    double NotunderstandSure2 = 0;

                    cout << "\x1b[32;40m                                                                  \x1b[0m"
                         << endl;
                    cout << "\x1b[32;40m The information The information you have entered are : \x1b[0m" << endl;
                    cout << "\x1b[37;40m Number Of Payment              : " << NumberOfPayment << "\x1b[0m" << endl;
                    cout << "\x1b[37;40m Interest Rate                : " << InterestRate << "\x1b[0m" << endl;
                    cout << "\x1b[37;40m Instalment              : " << Instalment << "\x1b[0m" << endl;
                    cout << "\x1b[32;40m                                                                  \x1b[0m"
                         << endl;

                    while (NotunderstandSure2 == 0)
                    {
                        cout << "\x1b[32;40m Do you agree with the information you have given us  (Yes/No) : \x1b[0m"
                             << " ";
                        cin >> Sure;
                        if ((Sure == "Yes") || (Sure == "yes") || (Sure == "YES"))
                        {
                            NotunderstandSure2 = 1;

                        }
                        else if ((Sure == "No") || (Sure == "no") || (Sure == "NO"))
                        {
                            NumberOfPayment = Enter_numberofperiod();
                            InterestRate = Enter_interestrate();
                            Instalment = Enter_instalment();
                            cout<< "\x1b[32;40m                                                                  \x1b[0m"<< endl;
                            cout << "\x1b[32;40m The information The information you have entered are : \x1b[0m"<< endl;
                            cout << "\x1b[37;40m Number Of Payment             : " << NumberOfPayment << "\x1b[0m"<< endl;
                            cout << "\x1b[37;40m Interest Rate                : " << InterestRate << "\x1b[0m" << endl;
                            cout << "\x1b[37;40m Instalment              : " << Instalment << "\x1b[0m" << endl;
                            cout<< "\x1b[32;40m                                                                  \x1b[0m"<< endl;

                        }
                        else
                            {

                            cout << "\x1b[32;40m Can you repeat please?  \x1b[0m" << endl;

                            }
                    }


                    outData << endl;
                    outData << ";" << "Number Of Payment" << ";" << NumberOfPayment << endl;
                    outData << ";" << "Interest Rate" << ";" << InterestRate << endl;
                    outData << ";" << "Instalment" << ";" << Instalment << endl;


                    string Frequence = frequency();
                    InterestRate = frequency_Interest_rate(InterestRate, Frequence);

                    outData << ";" << "Frequency" << ";" << Frequence << endl;
                    outData << endl;
                    Fixed_NumberOfperiod_InterestRate_Instalment(NumberOfPayment, InterestRate, Instalment,monthofcredit, yearofcredit, Frequence);


                }
                else if (ChoiceFunction1 == 6)
                {
                    cout << "\x1b[32;40m  You will now Enter the Value of the Different Variable : \x1b[0m" << endl;
                    double NumberOfPayment = Enter_numberofperiod();
                    double Instalment = Enter_instalment();
                    double OpeningBalance = Enter_openingbalance();
                    double NotunderstandSure2 = 0;

                    cout << "\x1b[32;40m                                                                  \x1b[0m"
                         << endl;
                    cout << "\x1b[32;40m The information The information you have entered are : \x1b[0m" << endl;
                    cout << "\x1b[37;40m Opening Balance              : " << OpeningBalance << "\x1b[0m" << endl;
                    cout << "\x1b[37;40m Instalment               : " << Instalment << "\x1b[0m" << endl;
                    cout << "\x1b[37;40m Number Of Payment               : " << NumberOfPayment << "\x1b[0m" << endl;
                    cout << "\x1b[32;40m                                                                  \x1b[0m"
                         << endl;

                    while (NotunderstandSure2 == 0)
                    {
                        cout << "\x1b[32;40m Do you agree with the information you have given us  (Yes/No) : \x1b[0m"
                             << " ";
                        cin >> Sure;
                        if ((Sure == "Yes") || (Sure == "yes") || (Sure == "YES"))
                        {
                            NotunderstandSure2 = 1;

                        }
                        else if ((Sure == "No") || (Sure == "no") || (Sure == "NO")) {
                            NumberOfPayment = Enter_numberofperiod();
                            OpeningBalance = Enter_openingbalance();
                            Instalment = Enter_instalment();
                            cout
                                    << "\x1b[32;40m                                                                  \x1b[0m"
                                    << endl;
                            cout << "\x1b[32;40m The information The information you have entered are : \x1b[0m"
                                 << endl;
                            cout << "\x1b[37;40m Number Of Payment             : " << NumberOfPayment << "\x1b[0m"
                                 << endl;
                            cout << "\x1b[37;40m Opening Balance              : " << OpeningBalance << "\x1b[0m"
                                 << endl;
                            cout << "\x1b[37;40m Instalment              : " << Instalment << "\x1b[0m" << endl;
                            cout
                                    << "\x1b[32;40m                                                                  \x1b[0m"
                                    << endl;

                        }
                        else
                            {

                            cout << "\x1b[32;40m Can you repeat please?  \x1b[0m" << endl;

                            }
                    }


                    outData << endl;
                    outData << ";" << "Number Of Payment" << ";" << NumberOfPayment << endl;
                    outData << ";" << "Opening Balance" << ";" << OpeningBalance << endl;
                    outData << ";" << "Instalment" << ";" << Instalment<< endl;


                    string Frequence = frequency();
                    outData << ";" << "Frequency" << ";" << Frequence << endl;
                    outData << endl;
                    Fixed_OpeningBalance_NumberOfperiod_Instalment(OpeningBalance, NumberOfPayment, Instalment,monthofcredit, yearofcredit, Frequence);


                }
            }


        }
        else if (FloatingorFixedrate == 2)
        {
            int ChoiceFunction2 = 0;

            cout << "\x1b[32;40m  For all the Choice you will have a Floating Interest Rate : \x1b[0m" << endl;
            cout << "\x1b[32;40m  Define the Floating Interest Rate : \x1b[0m" << endl;

            double MEAN = Variable_Interest_Rate_mean();
            double ST_DV = Variable_Interest_Rate_StDev();

            while ((ChoiceFunction2 > 4) || (ChoiceFunction2 < 1))
            {
                cout<< "\x1b[32;40m  You have the choice between Different Fixed Variable for calculate your loan  : \x1b[0m"<< endl;
                cout << "\x1b[32;40m  (Enter the number corresponding to the Rate you choose) \x1b[0m" << endl;
                cout << "\x1b[32;40m  1) Fixed OpeningBalance InterestRate Principal\x1b[0m" << endl;
                cout << "\x1b[32;40m  2) Fixed OpeningBalance InterestRate Number Of payment \x1b[0m" << endl;
                cout << "\x1b[32;40m  3) Fixed Principal InterestRate Number Of payment \x1b[0m" << endl;
                cout << "\x1b[32;40m  4) Fixed OpeningBalance InterestRate Instalment \x1b[0m" << endl;

                while (!(cin >> ChoiceFunction2))
                {
                    cerr << "\x1b[31;40m  Thanks enter a valid number \x1b[0m" << endl;
                    cin.clear();
                    cin.ignore(1);
                }
                if (ChoiceFunction2 == 1)
                {
                    cout << "\x1b[32;40m  You will now Enter the Value of the Different Variable : \x1b[0m" << endl;
                    double OpeningBalance = Enter_openingbalance();
                    double Principal = Enter_principal();
                    double NotunderstandSure2 = 0;
                    cout << "\x1b[32;40m                                                                  \x1b[0m"<< endl;
                    cout << "\x1b[32;40m The information The information you have entered are : \x1b[0m" << endl;
                    cout << "\x1b[37;40m Opening Balance              : " << OpeningBalance << "\x1b[0m" << endl;
                    cout << "\x1b[37;40m Principal               : " << Principal << "\x1b[0m" << endl;
                    cout << "\x1b[32;40m                                                                  \x1b[0m"<< endl;

                    while (NotunderstandSure2 == 0)
                    {
                        cout << "\x1b[32;40m Do you agree with the information you have given us  (Yes/No) : \x1b[0m"<< " ";
                        cin >> Sure;
                        if ((Sure == "Yes") || (Sure == "yes") || (Sure == "YES"))
                        {
                            NotunderstandSure2 = 1;

                        }
                        else if ((Sure == "No") || (Sure == "no") || (Sure == "NO"))
                        {
                            OpeningBalance = Enter_openingbalance();
                            Principal = Enter_principal();
                            cout
                                    << "\x1b[32;40m                                                                  \x1b[0m"
                                    << endl;
                            cout << "\x1b[32;40m The information The information you have entered are : \x1b[0m"
                                 << endl;
                            cout << "\x1b[37;40m Opening Balance              : " << OpeningBalance << "\x1b[0m"
                                 << endl;
                            cout << "\x1b[37;40m Principal               : " << Principal << "\x1b[0m" << endl;
                            cout
                                    << "\x1b[32;40m                                                                  \x1b[0m"
                                    << endl;

                        }
                        else
                            {

                            cout << "\x1b[32;40m Can you repeat please?  \x1b[0m" << endl;

                            }
                    }


                    outData << endl;
                    outData << ";" << "Opening Balance" << ";" << OpeningBalance << endl;
                    outData << ";" << "Mean" << ";" << MEAN << endl;
                    outData << ";" << "ST_DEV" << ";" << ST_DEV << endl;
                    outData << ";" << "Principal" << ";" << Principal << endl;


                    string Frequence = frequency();


                    outData << ";" << "Frequency" << ";" << Frequence << endl;
                    outData << endl;

                    Fixed_OpeningBalance_FloatInterestRate_Principal(OpeningBalance, MEAN, ST_DEV, Principal,monthofcredit, yearofcredit, Frequence);

                }
                else if (ChoiceFunction2 == 2)
                {

                    cout << "\x1b[32;40m  You will now Enter the Value of the Different Variable : \x1b[0m" << endl;
                    double OpeningBalance = Enter_openingbalance();
                    double NumberOfPayment = Enter_numberofperiod();
                    double NotunderstandSure2 = 0;
                    cout << "\x1b[32;40m                                                                  \x1b[0m"<< endl;
                    cout << "\x1b[32;40m The information The information you have entered are : \x1b[0m" << endl;
                    cout << "\x1b[37;40m Opening Balance              : " << OpeningBalance << "\x1b[0m" << endl;
                    cout << "\x1b[37;40m Number Of Payment               : " << NumberOfPayment << "\x1b[0m" << endl;
                    cout << "\x1b[32;40m                                                                  \x1b[0m"<< endl;

                    while (NotunderstandSure2 == 0)
                    {
                        cout << "\x1b[32;40m Do you agree with the information you have given us  (Yes/No) : \x1b[0m"
                             << " ";
                        cin >> Sure;
                        if ((Sure == "Yes") || (Sure == "yes") || (Sure == "YES"))
                        {
                            NotunderstandSure2 = 1;

                        }
                        else if ((Sure == "No") || (Sure == "no") || (Sure == "NO"))
                        {
                            OpeningBalance = Enter_openingbalance();
                            NumberOfPayment = Enter_numberofperiod();
                            cout
                                    << "\x1b[32;40m                                                                  \x1b[0m"
                                    << endl;
                            cout << "\x1b[32;40m The information The information you have entered are : \x1b[0m"
                                 << endl;
                            cout << "\x1b[37;40m Opening Balance              : " << OpeningBalance << "\x1b[0m"
                                 << endl;
                            cout << "\x1b[37;40m Number Of Payment              : " << NumberOfPayment << "\x1b[0m"
                                 << endl;
                            cout
                                    << "\x1b[32;40m                                                                  \x1b[0m"
                                    << endl;

                        }
                        else
                            {

                            cout << "\x1b[32;40m Can you repeat please?  \x1b[0m" << endl;

                            }
                    }


                    outData << endl;
                    outData << ";" << "Opening Balance" << ";" << OpeningBalance << endl;
                    outData << ";" << "Mean" << ";" << MEAN << endl;
                    outData << ";" << "ST_DEV" << ";" << ST_DEV << endl;
                    outData << ";" << "Number Of Payment" << ";" << NumberOfPayment << endl;


                    string Frequence = frequency();

                    outData << ";" << "Frequency" << ";" << Frequence << endl;
                    outData << endl;
                    Fixed_OpeningBalance_FloatInterestRate_NumberOfperiod(OpeningBalance,MEAN,ST_DEV,NumberOfPayment,monthofcredit,yearofcredit,Frequence);


                }
                else if(ChoiceFunction2 == 3)
                {
                    cout << "\x1b[32;40m  You will now Enter the Value of the Different Variable : \x1b[0m" << endl;
                    double Principal = Enter_principal();
                    double NumberOfPayment = Enter_numberofperiod();
                    double NotunderstandSure2 = 0;
                    cout << "\x1b[32;40m                                                                  \x1b[0m"
                         << endl;
                    cout << "\x1b[32;40m The information The information you have entered are : \x1b[0m" << endl;
                    cout << "\x1b[37;40m Number Of Payment             : " << NumberOfPayment << "\x1b[0m" << endl;
                    cout << "\x1b[37;40m Principal              : " << Principal << "\x1b[0m" << endl;
                    cout << "\x1b[32;40m                                                                  \x1b[0m"
                         << endl;
                    while (NotunderstandSure2 == 0)
                    {
                        cout << "\x1b[32;40m Do you agree with the information you have given us  (Yes/No) : \x1b[0m"
                             << " ";
                        cin >> Sure;
                        if ((Sure == "Yes") || (Sure == "yes") || (Sure == "YES"))
                        {
                            NotunderstandSure2 = 1;

                        }
                        else if ((Sure == "No") || (Sure == "no") || (Sure == "NO"))
                        {
                            Principal = Enter_principal();
                            NumberOfPayment = Enter_numberofperiod();
                            cout
                                    << "\x1b[32;40m                                                                  \x1b[0m"
                                    << endl;
                            cout << "\x1b[32;40m The information The information you have entered are : \x1b[0m"
                                 << endl;
                            cout << "\x1b[37;40m Principal              : " << Principal << "\x1b[0m" << endl;
                            cout << "\x1b[37;40m Number Of Payment              : " << NumberOfPayment << "\x1b[0m"
                                 << endl;
                            cout
                                    << "\x1b[32;40m                                                                  \x1b[0m"
                                    << endl;

                        }
                        else
                            {

                            cout << "\x1b[32;40m Can you repeat please?  \x1b[0m" << endl;

                            }
                    }


                    outData << endl;
                    outData << ";" << "Principal" << ";" << Principal << endl;
                    outData << ";" << "Mean" << ";" << MEAN << endl;
                    outData << ";" << "ST_DEV" << ";" << ST_DEV << endl;
                    outData << ";" << "Number Of Payment" << ";" << NumberOfPayment << endl;


                    string Frequence = frequency();

                    outData << ";" << "Frequency" << ";" << Frequence << endl;
                    outData << endl;

                    Fixed_Principal_FloatInterestRate_NumberOfperiod(Principal,MEAN,ST_DEV,NumberOfPayment,monthofcredit,yearofcredit,Frequence);



                }
                else if(ChoiceFunction2 == 4)
                {

                        cout << "\x1b[32;40m  You will now Enter the Value of the Different Variable : \x1b[0m" << endl;
                        double OpeningBalance = Enter_openingbalance();
                        double Instalment = Enter_instalment();
                        double NotunderstandSure2 = 0;

                        cout << "\x1b[32;40m                                                                  \x1b[0m"
                             << endl;
                        cout << "\x1b[32;40m The information The information you have entered are : \x1b[0m" << endl;
                        cout << "\x1b[37;40m Opening Balance              : " << OpeningBalance << "\x1b[0m" << endl;
                        cout << "\x1b[37;40m Instalment               : " << Instalment << "\x1b[0m" << endl;
                        cout << "\x1b[32;40m                                                                  \x1b[0m"
                             << endl;

                        while (NotunderstandSure2 == 0)
                        {
                            cout << "\x1b[32;40m Do you agree with the information you have given us  (Yes/No) : \x1b[0m"
                                 << " ";
                            cin >> Sure;
                            if ((Sure == "Yes") || (Sure == "yes") || (Sure == "YES"))
                            {
                                NotunderstandSure2 = 1;

                            }
                            else if ((Sure == "No") || (Sure == "no") || (Sure == "NO"))
                            {
                                OpeningBalance = Enter_openingbalance();
                                Instalment = Enter_instalment();

                                cout
                                        << "\x1b[32;40m                                                                  \x1b[0m"
                                        << endl;
                                cout << "\x1b[32;40m The information The information you have entered are : \x1b[0m"
                                     << endl;
                                cout << "\x1b[37;40m Opening Balance              : " << OpeningBalance << "\x1b[0m"
                                     << endl;
                                cout << "\x1b[37;40m Instalment              : " << Instalment << "\x1b[0m" << endl;
                                cout
                                        << "\x1b[32;40m                                                                  \x1b[0m"
                                        << endl;

                            }
                            else
                                {

                                cout << "\x1b[32;40m Can you repeat please?  \x1b[0m" << endl;

                                }
                        }


                        outData << endl;
                        outData << ";" << "Opening Balance" << ";" << OpeningBalance << endl;
                    outData << ";" << "Mean" << ";" << MEAN << endl;
                    outData << ";" << "ST_DEV" << ";" << ST_DEV << endl;
                        outData << ";" << "Instalment" << ";" << Instalment << "/" << yearoftoday << endl;


                        string Frequence = frequency();

                        outData << ";" << "Frequency" << ";" << Frequence << endl;
                        outData << endl;

                    Fixed_OpeningBalance_FloatInterestRate_Instalment(OpeningBalance,MEAN,ST_DEV,
                            Instalment,monthofcredit,yearofcredit,Frequence);



                    }
            }


        }
        else
            {
            cout << "\x1b[32;40m Can you repeat please?  \x1b[0m" << endl;

            }

    }
    outData << ";;;;;;;;;;;;;;;;;;;;;;;;;;" << endl;
    cout << endl;


}

int main(int argc, char** argv)
{
    Introduction();
    All_Step();

}
