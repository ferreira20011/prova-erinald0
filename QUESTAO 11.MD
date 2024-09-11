EX 11
#include <stdio.h>

void calcula_desconto_icms(float valor_produto) {
    float desconto;

    if (valor_produto <= 1000.00) {
        desconto = valor_produto * 0.05;
    } else if (valor_produto <= 5000.00) {
        desconto = valor_produto * 0.10;
    } else {
        desconto = valor_produto * 0.15;
    }

    printf("O valor do desconto de ICMS é: R$ %.2f\n", desconto);
}

int main() {
    float valor_produto;


    printf("Digite o valor do produto: ");
    scanf("%f", &valor_produto);

    calcula_desconto_icms(valor_produto);

    return 0;
}
