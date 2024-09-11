EX 6 
#include <stdio.h>


void verifica_aprovacao(float nota) {
    if (nota >= 7.0) {
        printf("Aprovado.\n");
    } else {
        printf("Reprovado.\n");
    }
}

int main() {
    float nota;

   
    printf("Digite a nota do aluno (0 a 10): ");
    scanf("%f", &nota);

    verifica_aprovacao(nota);

    return 0;
}
