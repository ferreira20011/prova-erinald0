EX 15
#include <stdio.h>


void converte_moeda(char origem, char destino, float valor) {
    float convertido;

    if (origem == 'B' && destino == 'U') {
        convertido = valor * 0.19;
        printf("Valor convertido: %.2f USD\n", convertido);
    } else if (origem == 'B' && destino == 'E') {
        convertido = valor * 0.16;
        printf("Valor convertido: %.2f EUR\n", convertido);
    } else if (origem == 'U' && destino == 'B') {
        convertido = valor * 5.30;
        printf("Valor convertido: %.2f BRL\n", convertido);
    } else if (origem == 'E' && destino == 'B') {
        convertido = valor * 6.20;
        printf("Valor convertido: %.2f BRL\n", convertido);
    } else if (origem == 'U' && destino == 'E') {
        convertido = valor * (5.30 / 6.20);
        printf("Valor convertido: %.2f EUR\n", convertido);
    } else if (origem == 'E' && destino == 'U') {
        convertido = valor * (6.20 / 5.30);
        printf("Valor convertido: %.2f USD\n", convertido);
    } else {
        printf("Erro: Moeda não reconhecida.\n");
    }
}

int main() {
    char origem, destino;
    float valor;


    printf("Informe a moeda de origem (B para BRL, U para USD, E para EUR): ");
    scanf(" %c", &origem);

    printf("Informe a moeda de destino (B para BRL, U para USD, E para EUR): ");
    scanf(" %c", &destino);

    printf("Informe o valor a ser convertido: ");
    scanf("%f", &valor);

    converte_moeda(origem, destino, valor);

    return 0;
}
