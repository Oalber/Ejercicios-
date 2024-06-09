#include <stdio.h>

int main() {

float num1, num2;

char operador;

printf("Ingrese el primer número: ");

scanf("%f", &num1);

printf("Ingrese el operador (+, -, *, /): ");

scanf(" %c", &operador);

printf("Ingrese el segundo número: ");

scanf("%f", &num2);

float resultado;

switch (operador) {

case '+':

resultado = num1 + num2;

break;

case '-':

resultado = num1 - num2;

break;

case '*':

resultado = num1 * num2;

break;

case '/':

if (num2 == 0) {

printf("Error: división por cero.\n");

return 1;

}

resultado = num1 / num2;

break;

default:

printf("Operador no válido.\n");

return 1;

}

printf("El resultado es: %f\n", resultado);

return 0;
}

