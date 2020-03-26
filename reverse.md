# Reverse Engineering 
Nesta sessão iremos explorar Reverse Engineering, uma técnica de análise de executáveis muito utilizada em cibersegurança. Vamos começar por um crackme, avançando depois para assembly e manipulação de binários. Durante estes exercicios serão utilizadas ferramentas de reverse engineering de programas linux/C e assembly.

## Nota prévia -- IMPORTANTE

Existem questões éticas relacionadas com a cibersegurança e o penetration testing, por exemplo sobre a exploração ilegítima de vulnerabilidades e informação encontrada através destas atividades. Pode ser encontrada em vários sites da Internet uma ampla discussão sobre estas questões éticas (um exemplo é https://cert.eccouncil.org/code-of-ethics.html). Chamamos a atenção para a necessidade de estar consciente destas questões éticas e de que não deve ser utilizada informação e conhecimento adquiridos para ciber-ataques ou outras atividades ilegais.

## Requisitos, ferramentas, apontadores:  

**Computador com Kali instalado numa VM** Ver em [Metaploit](metasploit.md), não é preciso modo bridge só acesso Internet por NAT.

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







## Exercício 1 -- CrackMe 1

## Exercício 2 -- Gatekeeper

### Manipulação de Binários

O ficheiro que vamos usar para o exercício de manipulação de binário pode ser obtido na respectiva pasta deste projeto.
O nome do ficheiro é Gatekeeper. Este é um ficheiro do tipo ELF: https://en.wikipedia.org/wiki/Executable_and_Linkable_Format.
<br/> O objetivo deste exercício é obter uma Flag, como num CTF. Assim que conseguirem, comuniquem a Flag encontrada a um dos monitores. 

## Exercício 3 -- CrackMe 2

## Exercício 4 -- LastOne







