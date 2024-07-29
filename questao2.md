Considere trecho de código em C que implementa uma função para verificar se um número é primo:


#include <stdio.h>
#include <stdbool.h>

bool ehPrimo(int num) {
if (num <= 1) {
return false;
}

    for (int i = 2; i * i <= num; i++) {
        if (num % i == 0) {
            return false;
        }
    }
    
    return true;
}

int main() {
int numero = 29;
if (ehPrimo(numero)) {
printf("%d é primo\n", numero);
} else {
printf("%d não é primo\n", numero);
}
return 0;
}

a) Grafo de Fluxo de Controle: O grafo de fluxo de controle representa as diferentes direções que o programa pode seguir com base nas condições. 
Para o código fornecido, o grafo de fluxo de controle é relativamente simples. 
Ele consiste em um caminho linear com uma bifurcação (condicional) para verificar se o número é primo ou não.

b) Caminhos Independentes: Existem dois caminhos independentes no código:
Caminho quando num é maior que 1 e é primo (entra no bloco if).
Caminho quando num é menor ou igual a 1 ou não é primo (entra no bloco else).

c) Caminhos Identificados:
Caminho: num > 1 e é primo.
Caminho: num <= 1 ou não é primo.

d) Casos de Teste para Cobertura:
Para o caminho 1 (número primo):
Entrada: num = 29 (um número primo maior que 1).
Para o caminho 2 (número não primo):
Entrada: num = 1 (número menor ou igual a 1).
Entrada: num = 4 (número não primo).

e) Condições Lógicas:
num <= 1: Verifica se o número é menor ou igual a 1.
i * i <= num: Verifica se i * i é menor ou igual a num.
num % i == 0: Verifica se num é divisível por i.

f) Conjunto Mínimo de Casos de Teste:

Teste 1: num = 29 (número primo).
Teste 2: num = 1 (número não primo).
Teste 3: num = 4 (número não primo).
g) Análise de Valor Limite:

Teste 1: num = 2 (limite inferior, número primo).
Teste 2: num = 3 (limite inferior, número primo).
Teste 3: num = 1000000 (limite superior, número não primo).