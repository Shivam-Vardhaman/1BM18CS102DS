#include <stdio.h>
#include<stdlib.h>
#define MAX 50
void insert();
void delete();
void display();
int queue_array[MAX];
int rear = - 1;
int front = 0;
int main()
{
int choice;
while (1)
{
printf("Enter Choice : \n ");
printf("1.Insert  \n");
printf("2.Delete \n");
printf("3.Display \n");
printf("4.Quit \n");
scanf("%d", &choice);
switch(choice)
{
case 1:
insert();
break;
case 2:
delete();
break;
case 3:
display();
break;
case 4:
exit(1);
default:
printf("Choice is wrong \n");
}
}
}
void insert()
{
int item;
if(rear == MAX - 1)
printf("Queue Overflow \n");
else
{
if(front>rear)
front = 0;
printf("Insert the element in queue :\n ");
scanf("%d", &item);
 rear ++;
queue_array[rear] = item;
}
}
void delete()
{
if(front>rear)
{
printf("Queue Underflow \n");
return;
}
else
{
printf("Element removed from queue is : %d \n", queue_array[front]);
 front ++;
}
}
void display()
{
int i;
if(front == - 1)
printf("Queue does not contain any element \n");
else
{
printf("Queue is : \n");
for(i = front; i <= rear; i++)
printf("%d \n ", queue_array[i]);
printf("\n");
}
}
