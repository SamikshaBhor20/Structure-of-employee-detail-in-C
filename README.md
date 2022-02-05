//# Structure-of-employee-detail-in-C
//Program that defines a structure employee containing the details such as empno, empname, department name and salary. The structure has to store 20 employees in an organization.

#include<stdio.h>
#include<stdlib.h>
typedef struct
{
  char name[30];
  int id;
  double salary;
}
Employee;
int main()
{
  int n=2;
  Employee employees[n];
  printf("Enter %d Employee details \n \n",n);
  for(int i=0;i<n;i++)
  {
    printf("Employee %d;- \n",i+1);
    printf("Name: ");
    scanf("%[^\n]s",employees[i].id);
    printf("Salary: ");
    scanf("%lf",&employees[i].salary);
    char ch=getchar();
    printf("\n");
    
  }
  printf("-------------All Employees Deatails------------\n");
  for(int i=0;i<n;i++)
  {
    printf"Name\t: ");
    printf("%s \n",employees[i].name);
    
    printf("ID \t: ");
    printf("%d \n",employees[i].id);
    
    printf("Salary \t: ");
    printf("%.2lf \n",employees[i].salary);
    
    printf("\n");
  }
  return 0;
}
