julien@ubuntu:~/0x0d. structures, typedef$ 
Repo:

GitHub repository: alx-low_level_programming
Directory: 0x0E-structures_typedef
File: dog.h
   
1. A dog is the only thing on earth that loves you more than you love yourself
mandatory
Score: 0.0% (Checks completed: 0.0%)
Write a function that initialize a variable of type struct dog

Prototype: void init_dog(struct dog *d, char *name, float age, char *owner);
julien@ubuntu:~/0x0d. structures, typedef$ cat 1-main.c
#include <stdio.h>
#include "dog.h"

/**
 * main - check the code
 *
 * Return: Always 0.
 */
int main(void)
{
    struct dog my_dog;

    init_dog(&my_dog, "Poppy", 3.5, "Bob");
    printf("My name is %s, and I am %.1f :) - Woof!\n", my_dog.name, my_dog.age);
    return (0);
}
julien@ubuntu:~/0x0d. structures, typedef$ gcc -Wall -pedantic -Werror -Wextra -std=gnu89 1-main.c 1-init_dog.c -o b
julien@ubuntu:~/0x0d. structures, typedef$ ./b 
My name is Poppy, and I am 3.5 :) - Woof!
julien@ubuntu:~/0x0d. structures, typedef$ 
Repo:

GitHub repository: alx-low_level_programming
Directory: 0x0E-structures_typedef
File: 1-init_dog.c
