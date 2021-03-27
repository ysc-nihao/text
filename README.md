#include<iostream>
using namespace std;

int facttail(int n, int a)
{


    if (n < 0)
        return 0;
    else if (n == 0)
        return 1;
    else if (n == 1)
        return a;
    else
        return facttail(n - 1, n * a);
    
}
int main()
{
    int n;
    cout << "请输入要阶乘的n的值：" << endl;
    cin >> n;
    cout<<"您得到的n的阶乘为："<<facttail(n,1);
}
