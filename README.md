# Bài 1. Tính toán giá trị của biểu thức
```
#include<stdio.h>
#include<math.h>

int main(){
	int x;
	scanf("%d",&x);
	printf("%lld",1ll*x*x*x+3ll*x*x+x+1);
	return 0;
}
```
# Bài 2. Tính toán giá trị biểu thức 2
```
#include <stdio.h>
#include <string.h>
#include <math.h>
#include <stdlib.h>

int main() {

    /* Enter your code here. Read input from STDIN. Print output to STDOUT */    
    return 0;
}

```
# Bài 3. Đổi nhiệt độ
```
#include<stdio.h>

int main(){
    short c;
    scanf("%d",&c);
    printf("%.2f",((float)c*9/5)+32    );
    return 0;
}
```
# Bài 4. Chu vi và diện tích hình tròn
```
#include<stdio.h>

int main(){
     int r;
    scanf("%d",&r);
    printf("%.4lf %.4lf",r*3.14*2,r*r*3.14);
    return 0;
}
```
# Bài 5. Khoảng cách Euclid
```
#include<stdio.h>
#include<math.h>

int main(){
    int x1,y1,x2,y2;
    scanf("%d %d %d %d",&x1,&y1,&x2,&y2);
    double dis=sqrt(pow(x1-x2,2)+pow(y1-y2,2));
    printf("%.2lf",dis);
    return 0 ;
    
}
```
#  Bài 6. Luyện tập viết câu điều kiện
```
#include<stdio.h>

int main(){
	int n;
	scanf("%d",&n);
	//1
	if(n%2==0){
		printf("YES\n");
	}
	else{
		printf("NO\n");
	}
	//2
	if(n%3==0 && n%5==0){
		printf("YES\n");
	}
	else{
		printf("NO\n");
	}
	//3
	if(n%3==0 && n%7!=0){
		printf("YES\n");
	}
	else{
		printf("NO\n");
	}
	//4
	if(n%3==0 || n%7==0){
		printf("YES\n");
	}
	else{
		printf("NO\n");
	}
	//5
	if(n>30 && n<50){
		printf("YES\n");
	}
	else{
		printf("NO\n");
	}
	//6
	if(n>=30 && (n%2==0 || n%3==0 || n%5==0)){
		printf("YES\n");
	}
	else{
		printf("NO\n");
	}
	//7
	if(n>=10 && n<=99 &&(n%10==2 || n%10==3 || n%10== 5 || n%10== 7)){
		printf("YES\n");
	}
	else{
		printf("NO\n");
	}
	//8
	if(n<=100 && n%23==0){
		printf("YES\n");
	}
	else{
		printf("NO\n");
	}
	//9
	if(n<10 || n>20){
		printf("YES\n");
	}
	else{
		printf("NO\n");
	}
	//10
	int r=n%10;
	if(r%3==0){
		printf("YES\n");
	}
	else{
		printf("NO\n");
	}
	return 0;
}
	
```
# Bài 7. Số lớn nhất và nhỏ nhất
```
#include <stdio.h>
#include <string.h>
#include <math.h>
#include <stdlib.h>

int main(){
    int a,b;
    scanf("%d %d",&a,&b);
    long long s1= a/b*b*1ll;
    long long s2= (a+b-1)/b*b*1ll;
    printf("%lld\n",s1);
    printf("%lld\n",s2);
    return 0;
}
```
# Bài 8. Tổng, hiệu, tích, thương
```
#include <stdio.h>
#include <string.h>
#include <math.h>
#include <stdlib.h>

int main(){
    int a,b;
    scanf("%d %d",&a,&b);
    printf("%lld\n",(long long)a+b);
    printf("%d\n",a-b);
    printf("%lld\n",(long long)a*b);
    if(b>0){
        printf("%.4lf",(double)a/b);
    }
    else{
        printf("INVALID");
    }
    return 0;
}
```
# Bài 9.Kiểm tra năm nhuận
```
#include <stdio.h>
#include <string.h>
#include <math.h>
#include <stdlib.h>

int main() {
    int n;
    scanf("%d",&n);
    if(n%400==0 || (n%4==0 && n%100!=0)){
        printf("YES");
    } 
    else{
        printf("NO");
    }
    return 0;
}
```
# Bài 10. Tam giác hợp lệ
```
#include <stdio.h>
#include <string.h>
#include <math.h>
#include <stdlib.h>

int main() {
    int a,b,c;
    scanf("%d %d %d",&a,&b,&c);
    if(a,b,c>0 && a+b>c&&a+c>b&&c+b>a){
        printf("YES");
    }   
    else{
        printf("NO");
    }
    return 0;
}
```
# Bài 11. Kiểm tra tam giác
```
#include <stdio.h>
#include <string.h>
#include <math.h>
#include <stdlib.h>

int main() {
    int a,b,c;
    scanf("%d %d %d",&a,&b,&c);
    if(a>0 && b>0 && c>0 && a+b>c && a+c>b && b+c>a){
        if(a==b&&b==c){
            printf("1");
        }
        else if(a==b||b==c){
            printf("2");
        }
        else if(a*a==b*b+c*c||b*b==a*a+c*c||c*c==a*a+b*b){
            printf("3");
        }
        else if(a+b>c||a+c>b||b+c>a){
            printf("4");
        }
    }
    else{
        printf("INVALID");
    }

    /* Enter your code here. Read input from STDIN. Print output to STDOUT */    
    return 0;
}
```
# Bài 12. Số ngày của tháng
```
#include <stdio.h>
#include <string.h>
#include <math.h>
#include <stdlib.h>

int main() {
    int t,n;
    scanf("%d %d",&t,&n);
    if(t>0&& t<13  && n>0){
        if(n%400==0||(n%4==0&&n%100!=0)){
            if(t==2){
                printf("29");
            }
            else if(t==1||t==3||t==5||t==7||t==8||t==10||t==12){
            printf("31");
            }
            else{
                printf("30");
            }
        }
        else if(t==1||t==3||t==5||t==7||t==8||t==10||t==12){
            printf("31");
        }
        else if(t==2){
            printf("28");
        }
        else{
            printf("30");
        }
        
    }else{
        printf("INVALID");
    }
    /* Enter your code here. Read input from STDIN. Print output to STDOUT */    
    return 0;
}
```
# Bài 13. Đổi ngày sang năm, tuần, ngày
```
#include <stdio.h>
#include <string.h>
#include <math.h>
#include <stdlib.h>

int main() {
    int n;
    scanf("%d",&n);
    int nam=n/365;
    n=n%365;
    int tuan=n/7;
    int ngay =n%7;
    printf("%d %d %d",nam,tuan,ngay);
    

    /* Enter your code here. Read input from STDIN. Print output to STDOUT */    
    return 0;
}
```
#  Bài 14. Xếp loại học sinh
```
#include <stdio.h>
#include <string.h>
#include <math.h>
#include <stdlib.h>

int main() {
    float a,b,c,d;
    scanf("%f %f %f %f",&a,&b,&c,&d);
    float tb=(a+b+c*2+d*3)/7;
    if( tb>=8){
        printf("GIOI");
    }
    else if(6.5<=tb){
        printf("KHA");
    }
    else if(5<=tb){
        printf("TRUNG BINH");
    }
    else{
        printf("YEU");
    }
    
    /* Enter your code here. Read input from STDIN. Print output to STDOUT */    
    return 0;
}
```
# Bài 15. Mua nước
```
#include <stdio.h>
#include <string.h>
#include <math.h>
#include <stdlib.h>

int main() {
    long long n,a,b;
    scanf("%lld %lld %lld",&n,&a,&b);
    if(a*2<=b){
        printf("%lld",n*a);
    }
    else{
        if(n%2==0){
            printf("%lld",n/2*b);
        }
        else{
            printf("%lld",n/2*b+a);
        }
    }
    

    /* Enter your code here. Read input from STDIN. Print output to STDOUT */    
    return 0;
}
```
# Bài 16. Kí tự kế tiếp
```
#include <stdio.h>
#include <string.h>
#include <math.h>
#include <stdlib.h>

int main() {
    int kitu;
    scanf("%c",&kitu);
    if(kitu=='Z'||kitu=='z'){
        printf("a");
    }
    else if(kitu>='A'&&kitu<'Z'){
        printf("%c",kitu+33);
    }
    else if('a'<=kitu&& kitu<'z'){
        printf("%c",kitu+1);
    }

    /* Enter your code here. Read input from STDIN. Print output to STDOUT */    
    return 0;
}
```
# Bài 17. Kiểm tra chữ cái
```
#include <stdio.h>
#include <string.h>
#include <math.h>
#include <stdlib.h>

int main() {
    int kitu;
    scanf("%c",&kitu);
    if(kitu>='A'&&kitu<='Z'){
        printf("UPPER");
    }
    else if(kitu>='a'&&kitu<='z'){
        printf("LOWER");
    }
    else if(kitu>='0'&&kitu<='9'){
        printf("DIGIT");
    }
    else{
        printf("SPECIAL");
    }

    /* Enter your code here. Read input from STDIN. Print output to STDOUT */    
    return 0;
}
```
# Bài 18. Chuyển đổi in hoa in thường
```
#include <stdio.h>
#include <string.h>
#include <math.h>
#include <stdlib.h>
char swap(char c){
    if(c>='A'&&c<='Z'){
     c=c+32;
    }
    else if(c>='a'&&c<='z'){
    c-=32;
    }
    else c;
    return c;
}

int main() {
    int kitu;
    scanf("%c",&kitu);
    printf("%c",swap(kitu));

    /* Enter your code here. Read input from STDIN. Print output to STDOUT */    
    return 0;
}
```
