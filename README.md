# lcx
语法入门
一，顺序结构程序设计
1001
#include <stdio.h>
int main()
{
    printf("zhe\n");
    printf("shi\n");
    printf("yi\n");
    printf("dao\n");
    printf("qian\n");
    printf("dao\n");
    printf("ti\n");
}
1002
#include<stdio.h>
int main(){
    printf("4396 = 28 x 157\n");
    printf("5346 = 18 x 297\n");
    printf("5346 = 27 x 198\n");
    printf("5796 = 12 x 483\n");
    printf("5796 = 42 x 138\n");
    printf("6952 = 4 x 1738\n");
    printf("7254 = 39 x 186\n");
    printf("7632 = 48 x 159\n");
    printf("7852 = 4 x 1963\n");
}
1003
#include<stdio.h>
int main(){
    printf("     **     \n");
    printf("     **     \n");
    printf("************\n");
    printf("************\n");
    printf("    *  *    \n");
    printf("    *  *    \n");
}
1004
#include<stdio.h>
int main(){
    printf("Helo word!");
}
1005
#include<stdio.h>
int main(){
    printf("1*1= 1\n");
    printf("1*2= 2 2*2= 4\n");
    printf("1*3= 3 2*3= 6 3*3= 9\n");
    printf("1*4= 4 2*4= 8 3*4=12 4*4=16\n");
    printf("1*5= 5 2*5=10 3*5=15 4*5=20 5*5=25\n");
    printf("1*6= 6 2*6=12 3*6=18 4*6=24 5*6=30 6*6=36\n");
    printf("1*7= 7 2*7=14 3*7=21 4*7=28 5*7=35 6*7=42 7*7=49\n");
    printf("1*8= 8 2*8=16 3*8=24 4*8=32 5*8=40 6*8=48 7*8=56 8*8=64\n");
    printf("1*9= 9 2*9=18 3*9=27 4*9=36 5*9=45 6*9=54 7*9=63 8*9=72 9*9=81\n");
}
二，选择结构程序设计
A比大小
#include<bits/stdc++.h>
using namespace std;
int main(){
    int a,b;
    cin >> a >> b;
    if(a<b) cout <<'<';
    else if (a>b) cout <<'>';
    else cout <<'=';
}
B卡拉兹函数
#include<bits/stdc++.h>
using namespace std;
int f(int n){
    if(n % 2 == 0)return n / 2;
    else return 3 * n + 1;
}
int main(){
    int n;
    cin >> n;
    cout << f(n);
}
C默契
#include<bits/stdc++.h>
using namespace std;
int main(){
    int x, y;
    cin >> x >> y;
    cout << (x == y ? "Tacit！" : "No Tacit!");
}
D整除判断
#include<bits/stdc++.h>
using namespace std;
int main(){
    int m, n;
    cin >> m >>n;
    cout << (m % n == 0 ? "YES" : "NO");
}
E CSimplemathproblem
#include<bits/stdc++.h>
using namespace std;
int main(){
    long long x, y;
    cin >> x >> y;
    cout << (y % x == 0 ? x + y : y - x);
}
三，循环结构程序设计
1001
#include <iostream>
#include <string>
using namespace std;
int main(){
    int n;
    while(cin >> n){
        for(int i = 1;i <= n;i++){
cout <<string(n-i,' ')<<string(2*i-1,'*') << endl;
        }
        for(int i = n -1;i >=1;i--){
            cout << string(n-i,' ')<<string(2*i-1,'*') << endl; 
        }
    }
}
1002
#include<stdio.h>
int main(){
    int n;
    int i,j;
    int num = 1;
    scanf("%d",&n);
    for(i = 1; i <= n; i++){
        for(j =1;j <= i; j++){
            printf("%4d",num);
            num = num + 1;
        }
        printf("\n");
    }
}
1003
#include<stdio.h>
int main(){
    char y;
    scanf("%c",&y);
    int total = y - 'A' + 1;
        int i , j ;
    for(i = 0 ; i < total ; i++){
        for(j = 0 ; j < total - i - 1 ; j++){
            printf(" ");
        }
        for(j = 0 ;j <= i ; j++){
            printf("%c",'A' + j );
        }
        for(j = i- 1 ; j >=0 ; j--){
            printf("%c",'A' + j );
        }
        printf("\n");
    }
}
1004
#include<bits/stdc++.h>
using namespace std;
int main(){
    int t;
    cin >> t;
    while (t--){
        int n;
        cin >> n;
        for (int i = 1; i <= (n-1) / 2; i++){
            for(int j = 1;j <= (n - 1) / 2 - i + 1; j++){
                cout << ' ';
            }
            for(int j =1; j <= 2 * i - 1; j++){
                cout << '*';
            }
            cout << '\n';
        }
        for(int i = 1; i <= n; i++){
            cout << '*';
        }
        cout << '\n';
        for(int i = 1; i <= (n - 1) / 2; i++){
            for(int j =1; j <= i; j++){
                cout << ' ';
            }
            for(int j = 1;j <=n - 2 * i;j++){
                cout << '*';
            }
            cout << '\n';
        }
    }
}
1005
#include <bits/stdc++.h>
using namespace std;
int main(){
    int n,x,q;
    while(cin>>n){
        x=1;q=n;
        for(int j=n*2;j>=0;j-=2){
            cout<<string(j,' ')<<string(x,'*')<<endl;x++;
        }
        for(int p=2;p<=2*n;p+=2){
            cout<<string(p,' ')<<string(q,'*')<<endl;q--;
        }
    }
}
四，数组、字符串及数据批量存储
1001
#include<iostream>
#include<iomanip>
using namespace std;
int main(){
    int T;
    cin >> T;
    while (T--){
        int x;
        cin >> x;
        long long y;
        cin >> y;
        long long maxv = y;
        long long minv = y;
        long long sum = y;
        long long sum2 = y  * y;
        for (int i = 1; i < x; i++){
            cin >> y;
            if (y > maxv){
                maxv = y;
            }
            if (y < minv){
                minv = y;
            }
            sum = sum + y;
            sum2 = sum2 + y * y;
        }
        long long range = maxv - minv;
        double var = ((double)sum2 - (double)sum*sum/x)/x;
        cout << range << " ";
        cout << fixed << setprecision(3) << var << endl;
    }
}
1002
#include<stdio.h>
int main(void){
    int n, x;
    scanf("%d%d",&n,&x);
    long long count = 0;
    for(int i = 1; i <= n;i++){
        int y = i;
        while(y > 0){
            if(y % 10 == x){
                count++;
            }
            y = y / 10;
        }
    }
    printf("%lld\n",count);
}
1003
#include<stdio.h>
int main(void){
    int n, k, m;
    scanf("%d%d%d",&n,&k,&m);
    int ans = 0;
    for(int i = 2;i <= n; i++){
        ans = (ans + m)% i;
    }
    ans = (ans + k) % n;
    printf("%d\n",ans);
}
1004
#include <iostream>
 using namespace std;
 int main(){
     int L, M;
     bool tree[10001] = {false};
     cin >> L >> M;
     for(int i = 1; i <= M; i++){
         int l, r;
         cin >> l >> r;
         for(int pos = l; pos <= r; pos++){
             tree[pos] = true;
         }
     }
     int ans = 0;
     for(int i = 0; i <= L; i++){
         if(tree[i]==false) ans++;
     }
     cout << ans;
 }
 1005
 #include<stdio.h>
int main(){
    int n;
    int a[100];
    scanf("%d", &n);
    for(int i = 0; i < n; i++){
        scanf("%d", &a[i]);
    }
    if(n >= 2){
        if(a[n-2] < a[n-1]){
            printf("UP\n");
        }
        else{
            printf("DOWN\n");
        }
    }
    else{
        if(a[0]==15)
            printf("DOWN\n");
        else if(a[0]==0)
            printf("UP\n");
        else
            printf("-1\n");
    }
}
五，函数与递归
A,
#include<iostream>
using namespace std;
int main(){
    int L,R;
    cin >> L >> R;
    int  cnt = 0;
    for(int i=L;i<=R;i++){
        int x = i;
        while(x>0){
            if(x%10 == 2) cnt++;
            x /=10;
        }
    }
    cout << cnt;
}
B,
#include <iostream>
using namespace std;
int cnt(int num, int x, bool isTwo){
    int res = 0;
    if(isTwo){
        if(num/10 == x) res++;
        if(num%10 == x) res++;
    }
    else{
        for(int t=num;t>0;t/=10)
            if(t%10 == x) res++;
    }
    return res;
}

int main(){
    int y,m,x;
    while(cin >> y >> m >> x){
        int days;
        if(m==1||m==3||m==5||m==7||m==8||m==10||m==12) days=31;
        else if(m==4||m==6||m==9||m==11) days=30;
        else days = ((y%4==0 && y%100!=0)||y%400==0) ? 29 : 28;int ans = 0;
        for(int d=1;d<=days;d++)
            ans += cnt(y,x,false)+cnt(m,x,true)+cnt(d,x,true);
        cout << ans << endl;
    }
}
C,
#include<iostream>
#include<string>
#include<cmath>
using namespace std;
bool isPrime(long long n){
    if(n <= 1)return false;
    for(long long i = 2; i <= sqrt(n); i++){
        if(n % i == 0){
            return false;
        }
    }
    return true;
}
int main(){
    string s;
    cin >> s;
    string newStr = s;
    for(int i = s.size()-2; i >= 0; i--){
        newStr += s[i];
    }
    long long num =stoll(newStr);
    if(isPrime(num)){
        cout << "prime" << endl;
    }
    else{
        cout << "noprime" << endl;
    }
}
D，
#include <iostream>
using namespace std;
int main() {
    int x, y;
    cin >> x >> y;
    if (x > y) {
        int temp = x;
        x = y;
        y = temp;
    }
    int count = 0;
    for (int i = x; i <= y; i++) {
        int temp = i;
        int sum = 0;
        while (temp > 0) {
            sum += temp % 10;
            temp /= 10;
        }
        if (sum % 5 == 0) {
            count++;
        }
    }
    cout << count << endl;
}
E，
#include <iostream>
#include <string>
#include <vector>
using namespace std;
int main(){
    int t;
    cin>>t;
    while(t--){
        string n,m;
        cin>>n>>m;
        int a1=n.size();
        int a2=m.size();
        vector<int> result(a1+a2);
        for(int i=a1-1;i>=0;i--){
            for(int j=a2-1;j>=0;j--){
                int b=(n[i]-'0')*(m[j]-'0');
                int sum=b+result[i+j+1];
                result[i+j+1]=sum%10;
                result[i+j]+=sum/10;
            }
        }
        for(int i=1;i<=a1+a2-1;i++){
            cout<<result[i];
        }
        cout<<endl;
    }
}
六，栈、队列和stl
A，
#include<iostream>
#include<algorithm>
using namespace std;
int main(){
    int a[8] = {1,2,3,4,5,6,7,8};
    do{
        cout << a[0];
        for(int i = 1; i < 8; i++){
            cout << " " << a[i];
        }
        cout << endl;
    }
    while(next_permutation(a, a + 8));
}
B，
#include <iostream>
#include <algorithm>
using namespace std;
const int MAXN = 100001;
int A[MAXN];
int B[MAXN];
int diff[MAXN];
int main(){
    int n, K;
    cin >> n >> K;
    for(int i = 0; i < n; i++){
        cin >> A[i];
    }
    for(int i = 0; i < n; i++){
        cin >> B[i];
    }
    long long sum = 0;
    for(int i = 0; i < n; i++){
        sum = sum + B[i];
        diff[i] = A[i] - B[i];
    }
    sort(diff, diff + n, greater<int>());
    for(int i = 0; i < K; i++){
        sum = sum + diff[i];
    }
 
    cout << sum << endl;
}
C，
#include<iostream>
#include<algorithm>
using namespace std;
const int MAXN = 101;
long long a[MAXN];
int main(){
    int n;
    cin >> n;
    for(int i= 0; i < n; i++){
        cin >> a[i];
    }
    sort(a, a + n);
    bool find = false;
    int pos;
    for(int i = 2; i < n; i++){
        if(a[i-2] + a[i-1] > a[i]){
            find = true;
            pos = i;
            break;
        }
    }
    if(find == true){
        cout << a[pos-2] << " " << a[pos-1] << " " << a[pos] << endl;
    }
    else{
        cout << "No solution" << endl;
    }
}
D，
#include<iostream>
#include<string>
#include<algorithm>
using namespace std;
const int MAXN = 25;
string s[MAXN];
bool cmp(string a, string b){
    return a + b > b + a;
}
int main(){
    int n;
    cin >> n;
    for(int i = 0; i < n; i++){
        cin >> s[i];
    }
    sort(s, s + n, cmp);
    for(int i = 0; i < n; i++){
        cout << s[i];
    }
}
E，
#include<iostream>
#include<string>
using namespace std;
int main(){
    string s;
    cin >> s;
    int cnta = 0, cntb = 0;
    bool ok = true;
    for(int i = 0; i < s.size(); i++){
        if(s[i] =='a'){
            cnta++;
        }
        else if(s[i] == 'b'){
            cntb++;
        }
        else{
            ok = false;
            break;
        }
        if(cntb > cnta){
            ok = false;
            break;
        }
    }
    if(ok && cnta == cntb){
        cout << "Good" << endl;
    }
    else{
        cout << "Bad" << endl;
    }
}
七，模拟、枚举与贪心
