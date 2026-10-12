# Code-for-insertion
The c++ code for insertion  

#include <iostream>
using namespace std;

int main() {
    int a[100], n, x;

    cout << "Enter size: ";
    cin >> n;

    cout << "Enter elements: ";
    for(int i = 0; i < n; i++)
        cin >> a[i];

    cout << "Enter element to insert: ";
    cin >> x;

    for(int i = n; i > 0; i--)
        a[i] = a[i - 1];

    a[0] = x;
    n++;

    cout << "Array: ";
    for(int i = 0; i < n; i++)
        cout << a[i] << " ";

    return 0;
}

# Code-for-insertion At End 

#include <iostream>
using namespace std;

int main() {
    int a[100], n, x;

    cout << "Enter size: ";
    cin >> n;

    cout << "Enter elements: ";
    for(int i = 0; i < n; i++)
        cin >> a[i];

    cout << "Enter element to insert: ";
    cin >> x;

    a[n] = x;
    n++;

    cout << "Array: ";
    for(int i = 0; i < n; i++)
        cout << a[i] << " ";

    return 0;
} 

# Code-for-insertion At Middle 
#include <iostream>
using namespace std;

int main() {
    int a[100], n, x, pos;

    cout << "Enter size: ";
    cin >> n  cout << "Enter elements: ";
    for(int i = 0; i < n; i++)
        cin >> a[i];

    cout << "Enter position: ";
    cin >> pos;

    cout << "Enter el# Code-forement: ";
    cin >> x;

    for(int i = n; i >= pos; i--)
        a[i] = a[i - 1];

    a[pos - 1] = x;
    n++;

    cout << "Array: ";
    for(int i = 0; i < n; i++)
        cout << a[i] << " ";

    return 0;
} 

# Code For Deletion at start 
#include <iostream>
using namespace std;

int main()
{
    int a[100], n;

    cout << "Enter size: ";
    cin >> n;

    cout << "Enter elements: ";
    for (int i = 0; i < n; i++)
    {
        cin >> a[i];
    }

    for (int i = 0; i < n - 1; i++)
    {
        a[i] = a[i + 1];
    }

    n--;

    cout << "Array after deletion: ";
    for (int i = 0; i < n; i++)
    {
        cout << a[i] << " ";
    }

    return 0;
} 
# Code For Deletion at End 
#include <iostream>
using namespace std;

int main()
{
    int a[100], n;

    cout << "Enter size: ";
    cin >> n;

    cout << "Enter elements: ";
    for (int i = 0; i < n; i++)
    {
        cin >> a[i];
    }

    n--;

    cout << "Array after deletion: ";
    for (int i = 0; i < n; i++)
    {
        cout << a[i] << " ";
    }

    return 0;
}
# Code For Deletion at middle 
#include <iostream>
using namespace std;

int main()
{
    int a[100], n;

    cout << "Enter size: ";
    cin >> n;

    cout << "Enter elements: ";
    for (int i = 0; i < n; i++)
    {
        cin >> a[i];
    }

    n--;

    cout << "Array after deletion: ";
    for (int i = 0; i < n; i++)
    {
        cout << a[i] << " ";
    }

    return 0;
} 
# Code-for- Factorial Recursion 
#include <iostream>
using namespace std;

long long int fact(int n);

int main()
{
int n;
long long int factorial = 1;

cout << "Enter value: ";
cin >> n;

factorial = fact(n);

cout << "Factorial of " << n << " is " << factorial;

return 0;

}

long long int fact(int n)
{
if (n == 0 || n == 1)
return 1;
else
return (long long int)n * fact(n - 1);
}
# Code For Push in stack 
#include <iostream>
using namespace std;

int stack[100];
int top = -1;
int size;

void push()
{
int x;

if (top == size - 1)
{
    cout << "Stack Overflow\n";
}
else
{
    cout << "Enter element: ";
    cin >> x;
    top++;
    stack[top] = x;
    cout << "Element pushed successfully\n";
}

}

void pop()
{
if (top == -1)
{
cout << "Stack Underflow\n";
}
else
{
cout << "Popped element: " << stack[top] << endl;
top--;
}
}

void display()
{
if (top == -1)
{
cout << "Stack is empty\n";
}
else
{
cout << "Stack elements: ";
for (int i = top; i >= 0; i--)
{
cout << stack[i] << " ";
}
cout << endl;
}
}

int main()
{
cout << "Enter stack size: ";
cin >> size;

int choice;

do
{
    cout << "\n1. Push";
    cout << "\n2. Pop";
    cout << "\n3. Display";
    cout << "\n4. Exit";
    cout << "\nEnter choice: ";
    cin >> choice;

    switch (choice)
    {
        case 1:
            push();
            break;

        case 2:
            pop();
            break;

        case 3:
            display();
            break;

        case 4:
            cout << "Program ended\n";
            break;

        default:
            cout << "Invalid choice\n";
    }

} while (choice != 4);

return 0;

}
# Code For Pop in Stack 
void pop()
{
    if (top == -1)
    {
        cout << "Stack Underflow\n";
    }
    else
    {
        cout << "Popped element: " << stack[top] << endl;
        top--;
    }
}


