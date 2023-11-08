# Calculator-with-login-er modifications
#include <stdio.h>
#include <stdlib.h>
#include <string.h>
int main() {
char username[20];
char password[20];
// Create a simple login system
printf("Welcome to the Calculator Program!\n");
printf("Enter your username: ");
scanf("%s", username);
printf("Enter your password: ");
scanf("%s", password);
// Simple check for username and password
if (strcmp(username, "user") == 0 && strcmp(password, "pass") == 0) {
printf("Login successful!\n");
float a, b;
char ch;
printf("Enter a: \n");
scanf("%f", &a);
printf("Enter b: \n");
scanf("%f", &b);
printf("Enter an operator (+, -, *, /)\n");
scanf(" %c", &ch);
if (ch == '+') {
printf("%f", a + b);
} else if (ch == '-') {
printf("%f", a - b);
} else if (ch == '*') {
printf("%f", a * b);
} else if (ch == '/') {
if (b != 0) {
printf("%f", a / b);
}
} else {
printf("Invalid operator\n");
}
} else {
printf("Login failed. Incorrect username or password.\n");
}
return 0;
}
