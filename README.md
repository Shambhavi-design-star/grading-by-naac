#include<stdio.h>
int main()
{
    int a,b,c,e,d,f,g,p,i,sum,pre=1000 ;
  float x;
    // take user input
  

    // printing the input value
for(i=1; i<=p; i++)
    {
          printf("Hello! Let's understand how the NAAC (National Assessment & Accreditation Council) grading system works.\n Enter number of colleges you want to search the NAAC ranking for: ");
    // use scanf to take input
    scanf("%d", &p);
    printf("First you have to fill the following details which are necessary to determine the NAAC ranking of the college: \n");
    printf("Enter the respective marks of the following elegibility criteria for NAAC:\n");
     printf("\n1. CURRICULAR ASPECTS: ");
        scanf("%d",&a);
 printf("\n2. TEACHING, LEARNING & EVALUATION: ");
        scanf("%d",&b);
         printf("\n3. RESEARCH, INNOVATION & EXTENSION: ");
        scanf("%d",&c);
          printf("\n4. INFRASTRUCTURE & LEARNING RESOURCES: ");
        scanf("%d",&d);
         printf("\n5. STUDENT SUPPORT & PROGRESSIONS: ");
        scanf("%d",&e);
        printf("6.LEADERSHIP AND MANAGEMENT:");
        scanf("%d",&f);
printf("\n7. INSTITUTIONAL VALUES & BEST PRACTICES: ");
        scanf("%d",&g);
         sum= (a+b+c+d+e+f+g);
        printf("\nSum of the seven CrW GP: %d\n", sum);
        if (a>=100 && b>=350 && c>=110 && d>=100 && e>=140 && f>=100 && g>=100)
       {
           printf("eligible for grading....\n");
      x=sum/pre;
        printf("Now comes the CGPA (Cumulative Grade Point Average).The formula for the same is as follows:\nThe sum of the seven CrW GP divided by the sum of the pre assigned Weightages of the seven Criteria.\nThus thecollege CGPA is:\n ");
        if(x<4 && x>3.51){
           printf("IT IS AN 'A++' GRADED COLLEGE. \n");
        }
         if(x<3.50 && x>3.26){
           printf("IT IS AN 'A+' GRADED COLLEGE. \n");
        }
         if(x<3.25 && x>3.01){
           printf("IT IS AN 'A' GRADED COLLEGE. \n");
        }
         if(x<3.00 && x>2.76){
           printf("IT IS A 'B++' GRADED COLLEGE. \n");
        }
         if(x<2.75 && x>2.51){
           printf("IT IS A 'B+' GRADED COLLEGE. \n");
        }
         if(x<2.50 && x>2.01){
           printf("IT IS A 'B' GRADED COLLEGE. \n");
        }
         if(x<2.00 && x>1.51){
           printf("IT IS A 'C' GRADED COLLEGE. \n");
        }
         if(x<=1.50){
           printf("IT IS A 'D' GRADED COLLEGE, which is not accredited. \n");
        }
       }
    else
    {
   printf("not eligible....\n");
}
    return 0;}
}
