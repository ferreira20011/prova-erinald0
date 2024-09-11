EX 12
#include <stdio.h>


void calcula_iptu(float valor_venal) {
    float iptu;

    if (valor_venal <= 100000.00) {
        iptu = valor_venal * 0.01;
    } else if (valor_venal <= 300000.00) {
        iptu = valor_venal * 0.015;
    } else if (valor_venal <= 500000.00) {
        iptu = valor_venal * 0.02;
    } else {
        iptu = valor_venal * 0.025;
    }

    printf("O valor do IPTU a ser pago é: R$ %.2f\n", iptu);
}

int main() {
    float valor_venal;


    printf("Digite o valor venal do imóvel: ");
    scanf("%f", &valor_venal);

    calcula_iptu(valor_venal);

    return 0;
}

