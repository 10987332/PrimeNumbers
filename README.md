#include<iostream>

using namespace std;

void prime(int m);

int main()
{

    int number = 0;

    // Take input from user
    cout << "Enter a number : " << endl;
    cin >> number;

        prime(number);
    }

    void prime (int m)
    {
        int sum = 0;
        for(int i = m; i > 0 ; i = i - 1)
        {
 bool not_prime = false;
            for(int j = 2; j < i; j++)
            {

            if(i%j == 0)
            {
                 not_prime = true;
                j = i;
            }
        }
         // If the number is prime then add it
           if (not_prime == false)
           {
                 sum = sum + i;
            }
        }

    cout << endl << "The Sum of prime numbers is " << sum;
}


