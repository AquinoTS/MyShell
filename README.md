# Mini Shell em C
Este projeto é um shell simplificado escrito em C, que oferece funcionalidades básicas de linha de comando, incluindo execução de comandos internos como cd e path, além de simulações dos comandos Unix cat e ls com suporte a redirecionamento de saída. 

## Funcionalidades
- Comando cd: Muda o diretório atual do shell.
- Comando path: Define os diretórios onde o shell busca por executáveis.
- Comando cat: Exibe o conteúdo de um arquivo. Suporta redirecionamento de saída utilizando >.
- Comando ls: Lista os arquivos no diretório atual. Suporta os flags -a (mostrar todos os arquivos, incluindo ocultos) e -l (mostrar detalhes dos arquivos).
- Redirecionamento de Saída: Permite redirecionar a saída de cat para um arquivo usando o operador >.
- Execução de comandos externos: Permite executar programas e scripts externos que estão nos caminhos definidos pelo comando path.
## Como Compilar
Para compilar o shell, você precisará de um compilador de C, como gcc ou clang. Aqui estão os passos para compilar usando gcc:

```bash
gcc -o shell shell.c
```
Isso compilará o código-fonte myshell.c em um executável chamado myshell.

## Como Usar
Após compilar o programa, você pode executá-lo diretamente do terminal:

```bash
./shell
```
Isso abrirá a interface do shell, onde você pode digitar comandos. Por exemplo:

```bash
myshell> ls -l
myshell> cat myfile.txt > output.txt
myshell> cd /path/to/directory
myshell> path /usr/bin /bin
myshell> exit
```
## Dependências
Este programa não requer bibliotecas externas, mas você deve ter um ambiente Unix-like para que as chamadas de sistema funcionem conforme esperado.
