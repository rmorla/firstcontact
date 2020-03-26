# Reverse Engineering 
Nesta sessão iremos explorar Reverse Engineering, uma técnica de análise de executáveis muito utilizada em cibersegurança. Vamos começar por um crackme, avançando depois para assembly e manipulação de binários. Durante estes exercicios serão utilizadas ferramentas de reverse engineering de programas linux/C e assembly.

## Nota prévia -- IMPORTANTE

Existem questões éticas relacionadas com a cibersegurança e o penetration testing, por exemplo sobre a exploração ilegítima de vulnerabilidades e informação encontrada através destas atividades. Pode ser encontrada em vários sites da Internet uma ampla discussão sobre estas questões éticas (um exemplo é https://cert.eccouncil.org/code-of-ethics.html). Chamamos a atenção para a necessidade de estar consciente destas questões éticas e de que não deve ser utilizada informação e conhecimento adquiridos para ciber-ataques ou outras atividades ilegais.

## Requisitos, ferramentas, apontadores:  

**Computador com Kali instalado numa VM** 
- Ver em [Metaploit](metasploit.md); não é preciso interface em modo bridge só acesso Internet normal por NAT.

**Ghidra** Ferramenta de reverse engineering, https://ghidra-sre.org. 
- 1/Java) sudo apt update ; sudo apt install openjdk-11-jdk 
- 2/Ghidra) download do zip do site Ghidra, unzip, e correr ./GhidraRun
- 3/Run) abrir um projeto novo e carregar o binário para análise.

**Outras ferramentas, incluídas no Kali** 
- file para ver características do ficheiro
- strings para identificar ASCII no meio do código executável
- objdump para ver estrutura do ficheiro binário
- r2 para re linha de comando
- hexeditor para editar binário
- python para programação rápida :)

**Análise dinâmica, debugging**
- ltrace e strace, instrumentação dinâmica, sudo apt install ltrace strace
- edb, debugger, sudo apt install edb-debugger

**Apontadores**

https://www.codementor.io/@packt/reverse-engineering-a-linux-executable-hello-world-rjceryk5d

<!--Software a instalar:
%- IDA -> https://en.wikipedia.org/wiki/Interactive_Disassembler <br/> Tutorial https://www.youtube.com/watch?v=3FnyzJ6bTEs
-->

<!--
## IMPORTANTE LER - APRESENTAÇÃO DE CONCEITOS FUNDAMENTAIS E FERRAMENTAS USADAS NOS EXERCÍCIOS
- http://www.cs.virginia.edu/~evans/cs216/guides/x86.html   X86 Assembly Guide
- https://lospi.net/developing/software/software%20engineering/reverse%20engineering/assembly/2015/03/06/reversing-with-ida.html Getting started with Reverse Engineering 
-->




## 4 Exercícios


### Exercício 1 -- CrackMe 1

**Objectivo:** Descobrir a password para encontrar a flag <br/>
**Ficheiros:** [ex1_1](content/bin/ex1.64) [ex1_2](content/bin/ex1_2.64)<br/>
**Dicas:** correr o comando chmod +x para tornar o ficheiro executavel, strings 

### Exercício 2 -- Skills

**Objectivo:** Descobrir o login para encontrar a flag <br/>
**Ficheiros:** [skills](content/bin/skills) <br/>
**Dicas:** strings, ltrace
 
### Exercício 3 -- CrackMe 2

**Objectivo:** Descobrir a password para encontrar a flag <br/>
**Ficheiros:** [ex3_1](content/bin/ex3.64) [ex3_2](content/bin/ex3_2.64)<br/>
**Dicas:** strings, ltrace, objdump, radare2

### Exercício 4 -- LastOne

**Objectivo:** Encontrar a flag <br/>
**Ficheiros:** [last_exercise](content/bin/last_exercise)<br/>
**Dicas:** radare2, ghidra, gdb



## Desenrolar do workshop

**Discord**
- discordapp.com , link de acesso enviado para o endereço de mail
- canal de dúvidas para instalação do Kali etc antes do workshop (apoio limitado)
- canais gerais de voz e de texto para acompanhamento durante o workshop
- canais por exercícios para dúvidas e discussão entre participantes

**Best effort**
- somos muitos inscritos e poucos a dar apoio, precisamos de bom senso e paciência
- os exercícios ficarão disponíveis após o workshop, e tentaremos dar apoio (limitado) também depois do workshop

