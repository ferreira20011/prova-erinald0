4EX
#include <stdio.h>


int eh_triangulo_retangulo(int a, int b, int c) {
  
    int temp;
    if (a > b) { temp = a; a = b; b = temp; }
    if (b > c) { temp = b; b = c; c = temp; }
    if (a > b) { temp = a; a = b; b = temp; }

   
    if (c * c == a * a + b * b) {
        return 1; 
    } else {
        return 0;
    }
}

int main() {
    int lado1, lado2, lado3;

   
    printf("Digite os três lados do triângulo: ");
    scanf("%d %d %d", &lado1, &lado2, &lado3);

    if (eh_triangulo_retangulo(lado1, lado2, lado3)) {
        printf("É um triângulo retângulo.\n");
    } else {
        printf("Não é um triângulo retângulo.\n");
    }

    return 0;
}
