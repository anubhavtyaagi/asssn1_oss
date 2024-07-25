# asssn1_oss
Create a C program that reads an array of integers from the user, calculates the average of the integers, and prints the result. Initialize a new Git repository for this project, commit the code, and upload it to your GitHub account. Provide the URL of the repository.
Write a C program that takes a string input from the user and reverses the string. Initialize a Git repository, commit your changes, and push the repository to GitHub. Share the repository link.
#include <stdio.h> #include <stdlib.h>

void reverse(int i, int j, char a[]) { if (i < j) { char t = a[i]; a[i] = a[j]; a[j] = t; reverse(i + 1, j - 1, a); } }

int main() { printf("Average of Array\n"); int n; printf("Enter the number of characters: "); scanf("%d",&n); char a[n]; printf("Enter %d characters: \n", n); for (int i = 0; i < n; i++) { printf("Enter character %d: ", i + 1); scanf(" %c", &a[i]); // Read each character into array a }

reverse(0,n-1,a);

for(int i=0;i<n;i++)
{
    printf("%c \t",a[i]);
}

return 0;
}

#include <stdio.h> #include <stdlib.h>

int main() { printf("Average of Array\n"); int n; printf("Enter the number of elements: "); scanf("%d",&n); int a[n]; printf("Enter the elements: \n"); for(int i=0;i<n;i++){ printf("Enter %d ",i); scanf("%d",&a[i]); }

float avg = 0;
for(int i=0;i<n;i++){
    avg += a[i];
}

avg = avg/n;
printf("The average of this array is: %f",avg);

return 0;
}
