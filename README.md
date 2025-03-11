# Calculadora-UFBRA
Projeto: Calculadora com Classes Aninhadas
Aluno: David Aparecido da Silva Faculdade: Centro Universitário UFBRA Disciplina: [Programação orientada a objeto ] Professor: [ALEXANDRE PEDROSO FERNANDES]

Requisitos do Sistema
Java: Versão 17 ou superior

Inclui suporte a novas funcionalidades como sealed classes e melhorias no Garbage Collector.

IDE Utilizada: IntelliJ IDEA ou Eclipse

Suporte a debugging, análise de código e gerenciamento de pacotes.

Descrição do Projeto
Este projeto utiliza conceitos de Programação Orientada a Objetos (POO) para criar uma calculadora modular baseada em classes aninhadas. A implementação reflete os princípios de encapsulamento e responsabilidade única, tornando o código limpo, reutilizável e fácil de manter. Cada operação matemática foi separada em sua própria classe, localizada dentro de um pacote dedicado.

Esquema de Organização do Projeto
A estrutura do projeto está organizada da seguinte forma:

src/
├── controle/
│   └── Calculadora.java    (Classe principal)
├── operacoes/
    ├── Soma.java           (Classe para somar valores)
    ├── Subtracao.java      (Classe para subtrair valores)
    ├── Multiplicacao.java  (Classe para multiplicar valores)
    └── Divisao.java        (Classe para dividir valores)
Principais Conceitos Utilizados
Programação Orientada a Objetos (POO):

Aplicação dos pilares da POO:

Encapsulamento: Cada operação matemática está isolada em sua própria classe.

Coesão: Cada classe possui uma única responsabilidade.

Uso de pacotes para melhor organização e modularidade.

Tratamento de Exceções:

Evita divisão por zero na classe Divisao utilizando:

java
if (b == 0) {
    throw new IllegalArgumentException("Divisão por zero não é permitida.");
}
Importação e Modularização:

Uso de pacotes (package) e importação (import) para isolar o código e permitir reutilização:

java
package operacoes; // Declaração do pacote
Estrutura de Fluxo:

Utilização do método main para centralizar a execução das operações matemáticas:

java
public static void main(String[] args) {
    Soma soma = new Soma();
    System.out.println(soma.executar(10, 5));
}
Instruções de Configuração e Execução
Configuração do Ambiente:

Baixe e instale o JDK 17 ou superior.

Configure sua IDE favorita (IntelliJ IDEA ou Eclipse).

Passos para Executar o Programa:

Clone o projeto ou baixe os arquivos.

Abra o projeto na sua IDE.

Compile o programa através do menu "Build".

Execute o método main da classe Calculadora.

Compilação e Execução via Linha de Comando:

Compile o código:

bash
javac -d bin src/controle/Calculadora.java
Execute:

bash
java -cp bin controle.Calculadora
Explicação do Funcionamento
Fluxo de Execução
A classe principal (Calculadora) é responsável por instanciar as operações matemáticas de cada classe.

Cada operação (Soma, Subtracao, Multiplicacao, Divisao) executa um cálculo e retorna o resultado para o console.

Divisão por zero é tratada com uma exceção personalizada.


Conclusão
Este projeto exemplifica o uso de boas práticas de desenvolvimento com Java, incluindo organização modular e aplicação de conceitos fundamentais de POO. Foi projetado para ser claro, eficiente e extensível para adição de novas operações no futuro.
