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
    cin >> n;

    cout << "Enter elements: ";
    for(int i = 0; i < n; i++)
        cin >> a[i];

    cout << "Enter position: ";
    cin >> pos;

    cout << "Enter element: ";
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
