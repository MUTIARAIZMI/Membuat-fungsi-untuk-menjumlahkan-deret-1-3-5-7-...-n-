# Membuat fungsi untuk menjumlahkan deret: 1+3+5+7+...+n 

Coding program lengkap

    #include <stdio.h>
    #include <conio.h>

    int jumlah (int x,int bil2);
    int ganjil (int bil1);

    int main (void)
    {
    int n,bil1,bil2,jum,x,i;
    printf("Masukan bilangan (n) = ");
    scanf ("%d",&n);
    bil1=1;
    x=1;
    printf("%d+",bil1);
    for (i=1;i<=n -2;i++)
    {
        bil2=ganjil(bil1);
        x=jumlah (x,bil2);
        bil1=bil2;
        printf("%d+",bil2);
    }
    bil2=ganjil (bil1);
    x=jumlah (x,bil2);
    printf("%d=%d",bil2,x);
    getch ();
    }
    int ganjil (int bil1)
    {
    int bil2;
    bil2=bil1+2;
    return (bil2);
    }
    int jumlah (int x,int bil2)
    {
    x=x+bil2;
    return (x);
    }


Hasil program

![img](https://raw.githubusercontent.com/MUTIARAIZMI/Membuat-fungsi-untuk-menjumlahkan-deret-1-3-5-7-...-n-/master/menjumlahkan%20deret%201%2B3%2B5%2B7.jpg)
