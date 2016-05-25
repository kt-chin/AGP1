*_AGP 1 Solutions:*_

*C++ Hello World*

#include <iostream>
#include <cstdio>
using namespace std;

int main() {
    printf("Hello, World!");
    return 0;
}

*Input and Output*

#include <cmath>
#include <cstdio>
#include <vector>
#include <iostream>
#include <algorithm>

int main() {
    int a;
    int b;
    int c;
    int sum;
    std::cin >> a >> b >> c;
    sum = a+b+c;
    std::cout << sum << std::endl;
    return 0;
}

*Basic Data Types*

#include <iostream>
#include <cstdio>
using namespace std;

int main() {
    int a;
    long  b;
    long long ch;
    char d;
    float e;
    double f;
    scanf("%d %ld %lld %c %f %lf",&a,&b,&ch,&d,&e,&f);
    printf("%d\n%ld\n%lld\n%c\n%f\n%lf",a,b,ch,d,e,f);
    // Complete the code.
    return 0;
}

*Conditional Statement*

#include <cmath>
#include <cstdio>
#include <vector>
#include <iostream>
#include <algorithm>
using namespace std;

int main() {
string s[] = {
"zero",
"one",
"two",
"three",
"four",
"five",
"six",
"seven",
"eight",
"nine"};
    int a;
    scanf("%d",&a);
    a<=9 ? cout << s[a] : cout<< "Greater than 9";
   return 0;
}

*For Loop*

#include <iostream>
#include <cstdio>
using namespace std;

int main() {
    int a;
    int b;
    string num[]{
        "zero",
        "one",
        "two",
        "three",
        "four",
        "five",
        "six",
        "seven",
        "eight",
        "nine"
    };
    scanf("%d %d",&a,&b);
    for (int i=a;i<= b; i++)
        {
        if (i<=9)
        cout << num[i] << endl;
              else if (i<=9)
                    cout << num[i] << endl;
            if (i>9 && i%2==0)
        {
            cout << "even"<<endl;
        }
            if (i>9 && i%2==1)
                {
                cout <<"odd"<< endl;
            }                
        }
    return 0;
}

*Functions*

#include <iostream>
#include <cstdio>
using namespace std;

int max_of_four(int a, int b, int c, int d)
{
    return((a>b?a:b)>(c>d?c:d)?(a>b?a:b):(c>d?c:d));
}

int main() {
    int a, b, c, d;
    scanf("%d %d %d %d", &a, &b, &c, &d);
    int ans = max_of_four(a, b, c, d);
    printf("%d", ans);
    
    return 0;
}

*Pointer*

#include <stdio.h>
void update(int *a,int *b) {
    int x = *a;
    int y = *b;
    *a<*b? *b = y - x: *b = x-y;
    *a = x+y;
}

int main() {
    int a, b;
    int *pa = &a, *pb = &b;
    scanf("%d %d", &a, &b);
    update(pa, pb);
    printf("%d\n%d", a, b);
    return 0;
}

*Array Introductions*

#include <cmath>
#include <cstdio>
#include <vector>
#include <iostream>
#include <algorithm>
using namespace std;

int main() {
    int n;
    cin>>n;
    int arr[n];
    if(n<1 || n > 1000) return -1;
    for (int i = 0;i<n;i++)
        cin>>arr[i];
    for (int i=n-1;i>=0;i--)
        cout << arr[i] << " ";  
    return 0;
}

*Simple Array Sum*

#include <cmath>
#include <cstdio>
#include <vector>
#include <iostream>
#include <algorithm>
using namespace std;

int main(){
    int n, sum = 0;
    cin >> n;
    vector<int> arr(n);
    for(int arr_i = 0;arr_i < n;arr_i++){
       cin >> arr[arr_i];
        sum += arr[arr_i];
       
    }
    cout << sum;
    
    return 0;
}

*Arrays - DS*

#include <map>
#include <set>
#include <list>
#include <cmath>
#include <ctime>
#include <deque>
#include <queue>
#include <stack>
#include <string>
#include <bitset>
#include <cstdio>
#include <limits>
#include <vector>
#include <climits>
#include <cstring>
#include <cstdlib>
#include <fstream>
#include <numeric>
#include <sstream>
#include <iostream>
#include <algorithm>
#include <unordered_map>

using namespace std;

int main(){
    int n;
    cin >> n;
    vector<int> arr(n);
    for(int arr_i = 0;arr_i < n;arr_i++){
       cin >> arr[arr_i];  
    }
          for (int arr_i=n-1; arr_i>=0; arr_i--)
      {
        cout  <<arr[arr_i]<< " ";    
      }
 
    return 0;
}

*Operator Overloading*

class Matrix{
public:
vector<vector<int> > a;

Matrix & operator + (const Matrix &y) {

    for (int i=0; i<y.a.size(); ++i) {
        for (int j=0; j<y.a[0].size(); ++j) {
            this->a[i][j] = this->a[i][j] + y.a[i][j];
        }
    }

    return *this;
}
};

*Plus Minus*

#include <cmath>
#include <cstdio>
#include <vector>
#include <iostream>
#include <algorithm>
using namespace std;

int main(){
    int n, m;
    float pos=0,neg=0,zero = 0;
    cin >> n;
    vector<int> arr(n);
    for(int arr_i = 0;arr_i < n;arr_i++){
       cin >> arr[arr_i];
        if(arr[arr_i] > 0) pos++;
        else if(arr[arr_i] <0) neg++;
        else if(arr[arr_i] ==0) zero++;
    }
    cout << (pos/n)<< endl;
    cout << (neg/n)<< endl;
    cout << (zero/n) << endl;
    return 0;
}

*Strings*

#include <iostream>
#include <string>
using namespace std;

int main() {
   // Complete the program
    string x, y;
    cin >> x >> y;  
    cout << x.length() << ' ' << y.length() << endl;
    cout << x + y << endl;
    swap( x[0], y[0] );
    cout << x << ' ' <<  y << endl;

    return 0;
}


*StringStream*

#include <sstream>
#include <vector>
#include <iostream>
using namespace std;

vector<int> parseInts(string str) {
    stringstream ss(str); 
    vector<int> result;
    char ch;
    int tmp;
    while(ss >> tmp) {      
    result.push_back(tmp);
    ss >> ch;         
        
}
return result;

}
int main() {
    string str;
    cin >> str;
    vector<int> integers = parseInts(str);
    for(int i = 0; i < integers.size(); i++) {
        cout << integers[i] << "\n";
    }
    
    return 0;
}

*Vector Sort*

#include <cmath>
#include <cstdio>
#include <vector>
#include <iostream>
#include <algorithm>
using namespace std;


int main() {
    vector <int> v;
    int size,a;
    cin >> size;
    for(int i = 0;i<size;i++)
    {
        cin >> a;
        v.push_back(a);
    }
    sort(v.begin(),v.end());
    for(int i =0; i<size;i++)
    {
        cout << v[i] << ' ';
    }
    return 0;
}

*Inheritance Introduction*

#include <cmath>
#include <cstdio>
#include <vector>
#include <iostream>
#include <algorithm>
using namespace std;


class Triangle{
    public:
       void triangle(){
           cout<<"I am a triangle\n";
       }
};
class Isosceles : public Triangle{
    public:
       void isosceles(){
          cout<<"I am an isosceles triangle\n";
       }
        void description()
        {
            cout<<"In an isosceles triangle two sides are equal\n";
        }
        //Write your code here.
};
int main(){
    Isosceles isc;
    isc.isosceles();
     isc.description();
    isc.triangle();
    return 0;
}

*Structs*
#include <cmath>
#include <cstdio>
#include <vector>
#include <iostream>
#include <algorithm>
using namespace std;

struct Student{
    int age;
    string first_name;
    string last_name;
    int standard;
};


int main() {
    Student st;
    
    cin >> st.age >> st.first_name >> st.last_name >> st.standard;
    cout << st.age << " " << st.first_name << " " << st.last_name << " " << st.standard;
    
    return 0;
}

*Classes and Objects*

class Student{
    private:
    vector<int> scores;

    public:
    void input(){
        scores.resize(5);
        for(int i=0; i<5; i++){
            cin >> scores[i];
        }
    }

    int calculateTotalScore (){
        return std::accumulate(scores.begin(), scores.end(), 0);
    }
};

*Overload Operators*

//Overload operators + and << for the class complex
//+ should add two complex numbers as (a+ib) + (c+id) = (a+c) + i(b+d)
//<< should print a complex number in the format "a+ib"
ostream& operator<<(ostream& os, const Complex& c) {
    return os << c.a << (c.b > 0 ? '+' : '-') << 'i' << c.b;
}

Complex operator+(const Complex& a, const Complex& b) { 
    return { a.a + b.a, a.b + b.b };
}

*Rectangle Area*

class Rectangle{
   public:
   int width;
   int height;
    const void Display() {
   cout << width << " " << height << endl;
}
};
class RectangleArea : public Rectangle {
    public:
    void Input()
    {
        cin >> width >> height;
    }
    void Display()
    {
        cout << width*height << endl;
    }
};

*Find Digits*

#include <cmath>
#include <cstdio>
#include <vector>
#include <iostream>
#include <algorithm>
using namespace std;

int main() {
int t; 
scanf("%d",&t);
for(int i = 0; i < t; i++)
{
    int n;
    int m;
    int count=0;
    scanf("%d",&n);
    int temp =n;
    while(n>0)
    {
        m=n%10;
        if(m!=0 && temp%m==0)
        {
            count++;
        }
        n=n/10;
    }
    printf("%d\n",count);
}
return 0;
}

*Multi Level Inheritance*

#include <cmath>
#include <cstdio>
#include <vector>
#include <iostream>
#include <algorithm>
using namespace std;

class Triangle{
   public:
      void triangle(){
         cout<<"I am a triangle\n";
      }
};

class Isosceles : public Triangle{
     public:
        void isosceles(){
          cout<<"I am an isosceles triangle\n";
        }
};
class Equilateral : public Isosceles{
     public:
        void equilateral(){
          cout<<"I am an equilateral triangle\n";
        }
};
   
//Write your code here.
int main(){
  
    Equilateral eqr;
    eqr.equilateral();
    eqr.isosceles();
    eqr.triangle();
    return 0;
}

*Class*

#include<iostream>
using namespace std;

class Student
{
public:
   void setage(int a)
{
    age=a;
}
int getage()
{
    return age;
}
void setstd(int b)
{
    standard=b;
}
int getstd()
{
    return standard;
}
void setfn(string c)
{
    first_name=c;
}
string getfn()
{
    return first_name;
}

void setln(string d)
{

    last_name=d;

}
string getln()
{
    return last_name;
}

   void totald()
    {
    cout<<age<<","<<first_name<<","<<last_name<<","<<standard;

}

private:
int age, standard;
string first_name, last_name;
string total;

};

int main()
{
int x,y;
string m;
string n;

cin>>x>>n>>m>>y;
Student myObject;
myObject.setage(x);
cout<<myObject.getage()<<endl;
myObject.setln(m);
cout<<myObject.getln()<<", ";
myObject.setfn(n);
cout<<myObject.getfn()<<endl;
myObject.setstd(y);
cout<<myObject.getstd()<<"\n"<<endl;
myObject.totald();

return 0;
}

*Sherlock and Squares*

#include <cmath>
#include <cstdio>
#include <vector>
#include <iostream>
#include <algorithm>
using namespace std;


int main() {

int t;
cin >> t;

for(int i = 0; i < t; i++){
    int a;
    int b;
    int count = 0;
    cin >> a >> b;
    int range;

    for(range = a; range <=b; ++range){

       int temp = sqrt(range);
        if(temp*temp == range)
        {
            count++;
            range += temp*2 ;
        }
    }
    cout<<count<<"\n";
}
return 0;
}

*Sherlock and the Beast*

#include <cmath>
#include <cstdio>
#include <vector>
#include <iostream>
#include <algorithm>
using namespace std;


int main(){
int t;
cin >> t;
for(int i = 0; i < t; i++)
{
int n, m, flag = -1;
 cin >> n;
m = n;
 if(m <= 0)
cout<<"-1\n";
else
{
if(m%3 == 0)
{
cout<< string(m,'5')<<"\n";
}
while(m%3 != 0)
{
m -= 5;
if(m<0)
{
 cout<<"-1\n";
        break;
    }
    else
        {
        if(m%3==0)
             cout<<string(m,'5')<<string((n-m),'3')<<"\n";
    }
}

}
}
return 0;
}

*A Very Big Sum*

#include <cmath>
#include <cstdio>
#include <vector>
#include <iostream>
#include <algorithm>
using namespace std;

int main(){ 
    int n; 
    long sum=0; 
    cin >> n; 
    vector<int> arr(n); 
    for(int arr_i = 0;arr_i < n;arr_i++)
        { 
        cin >> arr[arr_i];
    }
for(int i=0; i<n; i++)
    sum+=arr[i];
cout<<sum;

return 0;
}


*Angry Professor*

#include <cmath>
#include <cstdio>
#include <vector>
#include <iostream>
#include <algorithm>
using namespace std;
int main(){
    int t;
    cin >> t;
    for(int a0 = 0; a0 < t; a0++){
        int n;
        int k;
        int count = 0;
        cin >> n >> k;
        vector<int> a(n);
        for(int a_i = 0;a_i < n;a_i++){
           cin >> a[a_i];
            if (a[a_i] <= 0) {
                ++count;
            }
        }
        if (count < k) {
            cout <<"YES" << endl;
        } else {
            cout <<"NO" << endl;
        }
     }

    return 0;
}

*Utopian Tree*

#include <cmath>
#include <cstdio>
#include <vector>
#include <iostream>
#include <algorithm>
#include <cmath>
using namespace std;
int main(){
    int t;
    cin >> t;
    for(int a0 = 0; a0 < t; a0++){
        int n;
        cin >> n;    
        int exp = (n+1)/2 + 1;
        int val = pow(2,exp) - 1;
        if (n%2!=0) {
            val--;
        }
        cout<<val<<endl;
    }
    return 0;
}

*Staircase*

#include <cmath>
#include <cstdio>
#include <vector>
#include <iostream>
#include <algorithm>


int main(){
    int n;
    std::cin >>n;
    std::string s(n,' ');
    while(n){
    s[n-1]='#';
    std::cout << s << std::endl;
    --n;
}
    
    return 0;
}

