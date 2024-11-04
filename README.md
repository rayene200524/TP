#include <stdio.h>
#include <stdlib.h>
int main(){
	int A[4][4]={{1,2,3,4},{5,6,7,8},{9,10,11,12},{13,14,15,16}};  
	int T;
	int i,j;
   printf("tableau inital:\n");
    for(i=0;i<4;i++){
    	for(j=0;j<4;j++){
    		printf("%d\t\t",A[i][j]);
		}
		printf("\n");
	}
	    for(i=0;i<3;i++){
	    	for(j=i+1;j<4;j++){
	    		T=A[i][j];
	    		A[i][j]=A[j] [i];
	    		A[j][i]=T;
			}
			}
			printf("tableau echange :\n");
			for(i=0;i<4;i++){
				for(j=0;j<4;j++){
					printf("%d\t\t",A[i][j]);
				}
				printf("\n");
			}
			return 0;
}
