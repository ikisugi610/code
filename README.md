#include <stdio.h>
void one(int a, int b)
{  
    if(a==b)
    {
        printf("Chu Vi Hình Vuông: %dx4(4 cạnh)=%d\n", a, b*4);
    }
    else
    {
        printf("Chu Vi Hình Vuông: 2 cạnh không bằng nhau nên đây không phải là hình vuông\n");
    }
}
void two(int a, int b)
{
    if(a==b)
    {
        printf("Diện Tích Hình Vuông: %dx%d=%d\n", a, a, a*a);
    }
    else
    {
        printf("Diện Tích Hình Vuông: 2 cạnh không bằng nhau nên đây không phải hình vuông\n");
    }
}
void there(int a, int b)
{
    printf("Chu Vi Hình Chữ Nhật: 2x(%d+%d)=%d\n", a, b, 2*(a+b));
}
void four(int a, int b)
{
    printf("Diện Tích Hình Chữ Nhật: %dx%d=%d\n", a, b, a*b);
}
int main ()
{
    int a, b;
    printf("Hay nhap so a: ");
    scanf("%d", &a);
    printf("Hay nhap so b: ");
    scanf("%d", &b);
    one(a,b);
    two(a,b);
    there(a,b);
    four(a,b);
    while(a!=b)
    {
        printf("Lưu Ý: Hình Vuông Có 2 Cạnh Bằng Nhau\n");
        printf("Bạn Hãy Nhập Một Số a Khác Để TÍnh Hình Vuông: ");
        scanf("%d",&a);
        printf("Lưu Ý: Hình Vuông Có 2 Cạnh Bằng Nhau\n");
        printf("Bạn Hãy Nhập Một Số b Khác Để Tính Hình Vuông: ");
        scanf("%d",&b);
        if(a==b)
        {
            printf("Chu Vi Hình Vuông: %dx4(4 cạnh)=%d\n", a, b*4);
            printf("Diện Tích Hình Vuông: %dx%d=%d\n", a, a, a*a);
        }
        else
        {
            printf("Chu Vi Hình Vuông: 2 cạnh không bằng nhau nên đây không phải là hình vuông\n");
            printf("Diện Tích Hình Vuông: 2 cạnh không bằng nhau nên đây không phải hình vuông\n");
        }
    }
}
