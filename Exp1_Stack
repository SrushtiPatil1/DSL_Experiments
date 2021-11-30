
// NAME:- SRUSHTI B. PATIL
// CLASS:- IT - 43
// Program to implement stack using array in C.

#include<stdio.h>
int stack[], top=-1;
void push();
int pop();
int isFull();
int isEmpty();
void traverse();
void atTop();
void main(){


    int choice, stackItem;

    while(1){

        printf("Stack Operation \n");
        printf("Enter `1` for  Push Operation \n");
        printf("Enter `2` for  Pop Operation \n");
        printf("Enter `3` for  atTop Operation \n");
        printf("Enter `4` for  Traverse Operation \n");
        printf("Enter `5` for  Quit Operation \n");
        printf("Enter your choice : ");
        scanf("%d",&choice);

        switch(choice){
            case 1:
                    printf("Enter a integer value : ");
                    scanf("%d",&stackItem);
                    push(stackItem);
                    break;
            case 2:
                    stackItem = pop();
                    if(stackItem == 0){
                        printf("Your stack is underflow \n");
                    }else{
                        printf("Last popped item : %d\n", stackItem);
                    }
                    break;
            case 3:
                    atTop();
                    break;
            case 4:
                    traverse();
                    break;
            case 5:
                    return;
                    break;
            default: printf("Please enter correct choice : ");
        }
    }
}




void push(int stackElement)
{
    if(isFull()){
        printf("Stack is full.It can't be overflowed. \n");
    }else{
        top++;
        stack[top] = stackElement;
        printf("%d has been pushed \n", stackElement);
    }
}


int isFull(){
    if(top == 50-1){
        return 1;
    }else{
        return 0;
    }
}



int isEmpty(){
    if(top == -1){
        return 1;
    }else{
        return 0;
    }
}


int pop(){
    if(isEmpty()){
        return 0;
    }else{
        return stack[top--];
    }
}


void atTop()
{
    if(isEmpty())
    {
        printf("Your Stack is empty \n");
    }else{
        printf("Element at top is : %d \n", stack[top]);
    }
}


void traverse(){
    if(isEmpty())
    {
        printf("Your Stack is empty \n");
    }else{
        int i;
        printf("Stack Elements are : \n");
        for(i=0; i <= top; i++){
            printf("%d \n", stack[i]);
        }
    }
}
