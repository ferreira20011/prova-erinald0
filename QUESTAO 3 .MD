3EX:
#include <stdio.h>

int verificarTrianguloValido(int lado1, int lado2, int lado3) {
    
    if ((lado1 + lado2 > lado3) && (lado1 + lado3 > lado2) && (lado2 + lado3 > lado1)) {
        return 1; 
    }
    
}

int main() {
    int lado1, lado2, lado3;

    
    printf("Digite o primeiro lado do triângulo: ");
    scanf("%d", &lado1);
    printf("Digite o segundo lado do triângulo: ");
    scanf("%d", &lado2);
    printf("Digite o terceiro lado do triângulo: ");
    scanf("%d", &lado3);

    
    if (verificarTrianguloValido(lado1, lado2, lado3) == 1) {
        printf("É um triângulo válido.\n");
    } else {
        printf("Não é um triângulo válido.\n");
    }

    return 0;
}
