# dizideki-küçük-ve-büyük-sayiyi-bulma

#include<stdio.h>
#include<stdlib.h>
//dizideki en küçük ve en büyük sayiyi bulma
int main(void)
{
	int dizi[50],adet,kucuk,buyuk,i,j;
	printf("girilecek sayi adedi");
	scanf("%d",&adet);
	
	for(i=0;i<adet;i++)
	{
		printf("%d) sayi giriniz",i+1);
		scanf("%d",&dizi[i]);
		if(i==0)
		{
			kucuk=dizi[i];
			buyuk=dizi[i];
		}
		else
		{
			if(dizi[i]<kucuk)
			{
				kucuk=dizi[i];
			}
			else if(dizi[i]>buyuk)
			{
				buyuk=dizi[i];
			}
		}
	}
	printf("%d kucuk sayi %d buyuk sayi",kucuk,buyuk);
	printf("\n");
	return 0;
}
