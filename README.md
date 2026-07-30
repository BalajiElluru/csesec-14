#include<stdio.h>
void logic(int a[],int n)
{
	int temp,i,j;
	for( i=0;i<n-1;i++)
	{
		for(j=0;j<n-1-i;j++)
		{
			if(a[j]>a[j+1])
			{
			temp=a[i];
			a[i]=a[j+1];
			a[j+1]=temp;
		}
	}
}
}
void display(int a[],int n){
	int i;
for(i=0;i<n;i++){
	printf("%d",a[i]);
}
int main()
	int n;
	scanf("%d",&n);
	printf("enter number of element: ");
	int a[n],i;
	printf("enter elements:");
	for(i=0;i<n;i++){
	scanf("%d",&a[i]);
}
 logic(a,n);
printf("sorted array");
display(a,n);
return 0;
}
 
 

