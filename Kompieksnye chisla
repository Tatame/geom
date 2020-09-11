#include <stdio.h>
#include <math.h>
int main (){
    int n=0, s=0;
    double vesh=0, mn=0, r=0, f=0;
    printf("Введите вещественную часть числа\n");
    scanf("%lf",&vesh);
    printf("Введите мнимую часть числа\n");
    scanf("%lf",&mn);
    printf("Введите степень (натуральное число)\n");
    scanf("%d",&n);
    r=sqrt(vesh*vesh+mn*mn);
    f=atan(mn/vesh);
    now:printf("Какое действие хотите произвести?\n0-Тригонометрическая запись числа\n1-Обратное число\n2-Возведение в степень\n3-Все корни n-ой степени\n4-Закончить программу\n");
    scanf("%d",&s);
    if (s==0){
         printf("Z=%lf*(cos(%lf)+i*sin(%lf))\n",r,f,f); //В тригонометрическом представлении
         goto now;
    }
    if (s==1){
         printf("Z^-1=%lf-i*%lf\n",vesh/r,mn/r); //В минус первой
         goto now;
    }
    if (s==2){
         printf("Z^n=%lf*(cos(%lf)+i*sin(%lf))\n",pow(r,n),f*n,f*n);//В степени n
         goto now;
    }
    if (s==3){
         printf("n/Z=%lf*(cos(%lf+2pk)+i*sin(%lf+2pk))\n",pow(r,1/n),f/n,f/n);//Корень энной степени
         goto now;
    }
    if (s==4) goto end;
    else {
        printf("Нет такого варианта");
        goto now;
    }
    end: return 0;
}
