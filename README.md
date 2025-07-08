# Sistema de Folha de Pagamento em Java (POO)

Este projeto implementa um sistema simples de folha de pagamento em Java, utilizando os princípios da Programação Orientada a Objetos (POO) para gerenciar diferentes tipos de funcionários e calcular seus salários.

## 🚀 Conceitos de POO Abordados

* **Herança:** Demonstra a criação de uma hierarquia de classes, onde `Estagiario`, `FuncionarioHorista` e `FuncionarioMensalista` herdam de uma classe base `Funcionarios`.
* **Abstração:** A classe `Funcionarios` é abstrata, definindo um contrato comum para todos os funcionários com métodos abstratos como `calcularSalario()` e `imprimirDados()`.
* **Polimorfismo:** Diferentes tipos de funcionários podem ser tratados de forma genérica pela classe `FolhaPagamento`, e a lógica específica para calcular o salário e imprimir dados é executada de acordo com o tipo de funcionário.
* **Encapsulamento:** Os atributos das classes são privados e acessados através de métodos `getters` e `setters`, garantindo a proteção e o controle sobre os dados.
* **Composição/Agregação:** A classe `FolhaPagamento` "tem uma lista de" `Funcionarios`, mostrando como objetos podem ser combinados para construir sistemas mais complexos.

## 📂 Estrutura do Projeto

O projeto está organizado no pacote `lista04.exercicio01` e contém as seguintes classes:

* `Funcionarios.java`: Classe abstrata base para todos os funcionários, definindo nome, CPF e métodos abstratos para cálculo de salário e impressão de dados.
* `Estagiario.java`: Estende `Funcionarios`, calcula o salário baseado em uma bolsa e carga horária.
* `FuncionarioHorista.java`: Estende `Funcionarios`, calcula o salário baseado em horas trabalhadas e valor por hora.
* `FuncionarioMensalista.java`: Estende `Funcionarios`, calcula o salário baseado em um salário base e benefícios.
* `FolhaPagamento.java`: Gerencia uma lista de funcionários, permitindo adicionar, listar e calcular o valor total da folha de pagamento.
* `Aplicativo.java`: Classe principal com o método `main` para demonstrar a criação de diferentes tipos de funcionários e a funcionalidade da `FolhaPagamento`.

## 🛠️ Como Compilar e Rodar

1.  **Clone o repositório:**
    ```bash
    git clone [https://github.com/SeuUsuario/PayrollSystemJava.git](https://github.com/SeuUsuario/PayrollSystemJava.git)
    ```
2.  **Navegue até o diretório do projeto:**
    ```bash
    cd PayrollSystemJava
    ```
3.  **Compile os arquivos Java:**
    A partir da raiz do projeto (`PayrollSystemJava/`), execute:
    ```bash
    javac src/lista04/exercicio01/*.java -d out
    ```
    (Este comando compila todos os arquivos `.java` dentro do pacote e os coloca no diretório `out`).
4.  **Execute a aplicação:**
    ```bash
    java -cp out lista04.exercicio01.Aplicativo
    ```

## 📄 Exemplo de Saída

Ao executar o `Aplicativo.java`, você verá uma saída similar a esta no console:Funcionário: Gabriela CPF: 12345678998 Carga Horária: 30 Salário: 800,00
Funcionário: Rafaela 
CPF: 12345678998 
Horas trabalhadas: 40.0 
Valor horas: 80.0 
Salário: 3200,00
Funcionário: Isabela 
CPF: 12345678910 
Benefícios: 150.0 
Salário: 1950,00
Funcionário: Manuela
CPF: 12345678998
Carga Horária: 20
Salário: 700,00
Valor total a pagar é: R$ 6650.0

![Java](https://img.shields.io/badge/Java-007396?style=for-the-badge&logo=java&logoColor=white)
