# COMANDO-DE-REPETI-O-EM-C-
O código abaixo mostra como criar um programa em C que utiliza laços (loops) para varrer hosts.

⚠️ Uso exclusivo para fins educacionais • Desenvolvido por M!ss s3c

📝 Guia passo a passo: Criando e executando seu programa

1. Criar o arquivo do programa

No terminal, digite:

nano program.c


Adicione o seguinte código:

#include <stdio.h>

int main(int argc, char *argv[]){
    int i;

    if(argc < 2) {
        printf("Modo de uso: ./program 192.168.0 \n");
    } else {
        for(i = 0; i <= 10; i++){
            printf("Varrendo Host %s.%i  \n", argv[1], i);
        }
    }

    return 0;
}

2. Compilar o programa

No terminal, digite:

gcc program.c -o program


gcc → compilador C.

-o program → nome do executável gerado.

3. Executar o programa
./program 192.168.0

4. Exemplo de saída
Varrendo Host 192.168.0.0
Varrendo Host 192.168.0.1
Varrendo Host 192.168.0.2
Varrendo Host 192.168.0.3
...
Varrendo Host 192.168.0.10

👉 O que você aprendeu aqui

argc e argv → permitem capturar argumentos passados pelo terminal.

if() → permite executar ações condicionais.

for loop → repete um bloco de código várias vezes.

printf() → imprime informações na tela.

Combinar argumentos do terminal com loops permite automatizar tarefas repetitivas, como varredura de hosts.
