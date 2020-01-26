# matrix
finding the (diagonal ,upper diagonal ,lower diagonal) of the matrix and adding and subtracting the rows of the matrix 
#include<stdio.h>
int sum,diff;
int main(){
int i,j,a,b,c[10][10];
printf("\nenter number of rows:");
scanf("%d",&a);
printf("enter number of columns:");
scanf("%d",&b);
printf("\nenter matrix elements:\n");
for(i=1;i<=a;i++){
for(j=1;j<=b;j++){
printf("enter element [%d,%d]:",i,j);
scanf("%d",&c[i][j]);}}
printf("\nmatrix elements are:\n");
for(i=1;i<=a;i++){
for(j=1;j<=b;j++){
printf("%d\t",c[i][j]);}
printf("%d\n");}
printf("\n");
printf("diagonal of matrix:");
printf("\n");
for(i=1;i<=a;i++){
for(j=1;j<=b;j++){
if(i==j){
printf("%d\t",c[i][j]);}
else{
printf("\t");}}
printf("\n");}
printf("\n");
printf("upper diagonal of matrix:");
printf("\n");
 for(i=1;i<=a;i++){
for(j=1;j<=b;j++){
if(i<=j){
printf("%d\t",c[i][j]);}
else{
printf("\t");}}
printf("\n");}
printf("\n");
printf("lower diagonal of matrix:");
printf("\n");
for(i=1;i<=a;i++){
for(j=1;j<=b;j++){
if(i>=j){
printf("%d\t",c[i][j]);}
else{
printf("\t");}}
printf("\n");}
printf("\n");
printf("transpose of matrix:");
printf("\n");
for(i=1;i<=b;i++){
for(j=1;j<=a;j++){
printf("%d\t",c[j][i]);}
printf("%d\n");}
printf("\n");
printf("summing the rows of matrix:");
printf("\n");
for(i=1;i<=a;i++){
for(j=1;j<=b;j++){
sum+=c[i][j];}
printf("sum of %d row of matrix is %d\n",i,sum);
sum=0;}
printf("\n");
printf("subtracting the rows of matrix:");
printf("\n");
for(i=1;i<=a;i++){
for(j=1;j<=b;j++){
diff=c[i][j]-diff;}
printf("difference of %d row of matrix is %d\n",i,diff);
diff=0;}
return 0;}



 
