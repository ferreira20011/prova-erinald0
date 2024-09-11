EX16
#include <stdio.h>

int main() {
    float nota;
    
   
    printf("Informe a nota final do aluno (0 a 10): ");
    scanf("%f", &nota);

    
    if (nota < 0.0 || nota > 10.0) {
        printf("Erro: Nota fora do intervalo válido.\n");
    } else if (nota >= 9.0) {
        printf("Classificação: A\n");
    } else if (nota >= 7.0) {
        printf("Classificação: B\n");
    } else if (nota >= 5.0) {
        printf("Classificação: C\n");
    } else {
        printf("Classificação: D\n");
    }

    return 0;
}
