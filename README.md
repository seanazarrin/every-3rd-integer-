# every-3rd-integer-with-initial-2
#include <stdio.h>

int main(void) {
	int i,n;
	int sum=0;
	
  //user input 
  printf("for integers less than\n");
	scanf("%d",&n);
  
	//loop
  for(i=1;i<=n;i++){
	   
	    if(i%2==0){           //why can't we use the condition (i==g*2)
	            printf("%d\n",i);
	    } 
	    //previously had an else statement
	    //but multiples of 5 are also multiples of 2
	    if(i%5==0){
	                sum+=i;
	    }
	}
	 printf("sum of multiples of 5 = %d\n",sum);
	return 0;
}
