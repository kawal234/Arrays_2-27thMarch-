# Arrays_2-27thMarch-
#include<stdio.h>
------------------------------------------------------------------------------------------------------------------------------------------------------------------------
/*
int main(){
	int a[100];
	int i,loc=-1,key,n;
	printf("Enter value of n: ");
	scanf("%d",&n);
	printf("Enter the Elements: ");
	for(i=0;i<n;i++){
		scanf("%d",&a[i]);
	}
	printf("Enter integer value to search in array: ");
	scanf("%d",&key);
	for(i=0;i<n;i++){
		if(a[i]==key){
			loc=i;
			break;
		}
	}
	if(loc!=-1){
		printf("Element is found at %d",loc+1);
	}
	else{
		printf("Element is not found.");
	}
	return 0;
}
*/
------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

//for ascending order array
/*
int main(){
	int a[100];
	int i,loc=-1,key,n,mid,beg,last;
	printf("Enter value of n: ");
	scanf("%d",&n);
	printf("Enter the Elements: ");
	for(i=0;i<n;i++){
		scanf("%d",&a[i]);
	}
	beg=0;
	last=n-1;
	printf("Enter integer value to search: ");
	scanf("%d",&key);
	while(beg<=last){
		mid=(beg+last)/2;
		if(a[mid]==key){
			loc=mid;
			break;
		}
		else if(a[mid]>key){
			last=mid-1;
		}
		else if(a[mid]<key){
			beg=mid+1;
		}
		
	}
	if(loc!=-1){
		printf("element found at %d",loc+1);
	}
	else{
		printf("Element not found");
	}
	return 0;
}
*/
--------------------------------------------------------------------------------------------------------------------------------------------------------------------

//for descending order
/*
int main(){
	int a[100];
	int i,loc=-1,key,n,mid,beg,last;
	printf("Enter value of n: ");
	scanf("%d",&n);
	printf("Enter the Elements: ");
	for(i=0;i<n;i++){
		scanf("%d",&a[i]);
	}
	beg=0;
	last=n-1;
	printf("Enter integer value to search: ");
	scanf("%d",&key);
	while(beg<=last){
		mid=(beg+last)/2;
		if(a[mid]==key){
			loc=mid;
			break;
		}
		else if(a[mid]>key){
			beg=mid+1;
		}
		else if(a[mid]<key){
			last=mid-1;
		}
		
	}
	if(loc!=-1){
		printf("element found at %d",loc+1);
	}
	else{
		printf("Element not found");
	}
	return 0;
}
*/
---------------------------------------------------------------------------------------------------------------------------------------------------------------------
int main(){
	int a[100];
	int hold,i,j,n;
	printf("Enter value of n: ");
	scanf("%d",&n);
	printf("Enter the Elements: ");
	for(i=0;i<n;i++){
		scanf("%d",&a[i]);
	}
	printf("Data in Original Form");
	for(i=0;i<n;i++){
		printf("%d",a[i])
	}
	for(i=0;i<n-1;i++){
		for(j=0;j<n-1;j++){
			if(a[j]<a[j+1]){
				hold=a[j];
				a[j]=a[j+1];
				a[j+1]=hold;
			}
		}
	}
}
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
