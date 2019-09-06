# Welcome!

This C template lets you get started quickly with a simple one-page playground.

```C runnable
#include <stdio.h>
#include <stdlib.h>

struct node {
    int data;
    struct node* next;
};

void Push(struct node** headRef, int data) {
    struct node* newNode = malloc(sizeof(struct node));
    newNode->data = data;
    newNode->next = *headRef;
    *headRef = newNode;
}

int main() {
    struct node* node1 = NULL;
    Push(&node1,100);
	printf("Hello Node1 : %d", node1->data);
	return 0;   
}


```

# Advanced usage

If you want a more complex example (external libraries, viewers...), see the [official documentation](https://tech.io/playgrounds/408/tech-io-documentation).
