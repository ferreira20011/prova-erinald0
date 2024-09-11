 1EX.
 #include <stdio.h>


int verificar_primo(int numero) {
    
    if (numero == 2 || numero == 3 || numero == 5 || numero == 7) {
        return 1;
    }
   
    return 0;
}

int main() {
    
    int numeros[] = {1, 2, 3, 4, 5, 6, 7, 8, 9, 10};
    for (int i = 0; i < 10; i++) {
        int resultado = verificar_primo(numeros[i]);
        if (resultado) {
            printf("O número %d é primo.\n", numeros[i]);
        } else {
            printf("O número %d não é primo.\n", numeros[i]);
        }
    }
    return 0;
}
