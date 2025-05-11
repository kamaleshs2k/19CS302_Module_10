# EX 46 C function to traverse the linked list and display it in the following format.
## DATE: 11/05/2025
## AIM:
To write a C function to traverse the linked list and display it in the following format.

## Algorithm
1.Start the program and define a linked list node structure with data and next pointer.

2.Create a function display() that takes the head of the list as argument.

3.Traverse the list using a loop until the current node is NULL.

4.Print each node's data in the format data ->.

5.After the last node, print NULL and end the program.

## Program:
```
/*
C function to traverse the linked list and display it in the following format.

Developed by: Kamalesh S
RegisterNumber:  212223060108
*/
#include <stdio.h>
#include <stdlib.h>

struct Node
{
    int data;
    struct Node* next;
};

void display(struct Node* head)
{
    struct Node* current = head;
    while(current != NULL)
    {
        printf("%d -> ", current->data);
        current = current->next;
    }
    printf("NULL\n");
}

int main()
{
    struct Node* head = (struct Node*)malloc(sizeof(struct Node));
    struct Node* second = (struct Node*)malloc(sizeof(struct Node));
    struct Node* third = (struct Node*)malloc(sizeof(struct Node));

    head->data = 10;
    head->next = second;

    second->data = 20;
    second->next = third;

    third->data = 30;
    third->next = NULL;

    display(head);

    return 0;
}


```

## Output:

![image](https://github.com/user-attachments/assets/d089e533-d8cf-4f6e-8c00-0c2ea766872e)


## Result:
Thus the program was executed and the output was verified successfully.
