# revisao_POO

# Atividade 11
```java

package javaapplication121;

/**
 *
 * @author aluno.saolucas
 */
public class Aluno {
    
     private String nome;
     private String matricula;
     private String curso;
public Aluno(){
}
    public Aluno(String nome, String matricula, String curso) {
        this.nome = nome;
        this.matricula = matricula;
        this.curso = curso;
    }
     
     public void exibirDados(){
         System.out.println("Nome:"+nome);
         System.out.println("Matrícula:"+matricula);
         System.out.println("curso:"+curso);
     }
}
```
# Atividade 12

```java
12. Crie uma classe ContaBancaria com atributos numero, titular e saldo. Adicione
métodos depositar() e sacar(). Obs.: Nos métodos avaliar se existe saldo para
o saque e ao depositar verifique se o valor depositado não é negativo.


package atividade_2poo;

/**
 *
 * @author Henrique 01/09/2025 
 */
public class ContaBancaria {
    
    private String numero;
    private String titulo;
    private double saldo;

public ContaBancaria(){
//consutor padrao
}
    
    public void depositar(double valor){
        if(valor>0){
            saldo= saldo+valor;
            System.out.println("Deposito realizado "+valor);
        }else{
            System.out.println("Valor invalido para Deposito");
        }
    }
    public void sacar(double valor){
        if(valor>0){
            if(saldo>=valor){
                saldo=saldo-valor;
                System.out.println("Saque realizado: "+valor);
            }else{
                System.out.println("Saldo insuficiente");
            }
        }else{
            System.out.println("Valor de saque inválido");
        }
        
    }
}
```
# atividade 13

```java
package atividadepoo13;

/**
 * 13. Implemente uma classe Carro que tenha atributos marca, modelo e ano. Crie
 * um método ligar().
 *
 * @author Henrique 02/09/2025
 */
public class Carro {
    
    private String marca;
    private String modelo;
    private int ano;

public Caroo(){
}
    public void ligar(){
        System.out.println("O carro "+ marca+ " "+ modelo+ "("+ano+") está ligado");
    }
}
```
# atividade 14

```java
package atividadepoo14;

/**
 * 14. Crie uma classe Livro com atributos titulo e autor. Faça uma associação
 * com a classe Biblioteca.
 *
 * @author Henrique 02/09/2025
 */
public class Livro {
    
    private String titulo;
    private String autor;
}
```
```java
package atividadepoo14;

public class Biblioteca {
    private String nome;
    private Arraylist <Livro> Livros; //assossiaçao com a class Livro
    public Biblioteca;
}

}

```
# Atividade 15
```java
package poo15;

/**
 * 15. Implemente uma herança: uma classe Pessoa e duas subclasses Professor e
 * Estudante.
 *
 * @author Henrique 03/09/2025
 */
public class Pessoa { //SUPERCLASSE

    private String nome;
    private int idade;
}

public class Professor extends Pessoa { //SUBCLASSE
    private double Salario;
    public Professor(){
      super();  
}
}

public class Estudante extends Pessoa { //SUBCLASSE
    private double nota;
    public Aluno(){
        super();
}
}

```
# Atividade 16
```java
package poo16;

/**
 * 16. Escreva um exemplo de polimorfismo usando uma classe Animal com métodos
 * sobrescritos em Cachorro e Gato.
 *
 * @author Henrique 03/09/2025
 */
public class Animal {
    private String nome;
public Animal(){
}
    public void fazerSom(){
        System.out.println("O animal não fala");
    }
}

public class Cachorro extends Animal{
    private double racao;
public Cachorro(){
}
    public void fazerSom(){
        System.out.println("AU AU");
    }
}
public class Gato extends Animal{
    private double racao;
public Gato(){
}
    public void fazerSom(){
        System.out.println("MEOW MEOW");
    }
}
```

# atividade 17

```java
package poo17;

/**
 * 17. Crie uma classe Funcionario que possua um método calcularSalario(). Crie
 * uma subclasse Gerente que sobrescreva esse método.
 *
 * @author Henrique 03/09/2025
 */
public class Funcionario {
    protected double hora;
    protected double valorHora;
    public Funcionario(){   
}
    public void calcularSalario(){
        System.out.println("salario "+(hora+valorHora));
    }
}
public class Gerente extends Funcionario{
    private double adicional;
    public Gerente(){
        
    }
    public void calcularSalario(){
        System.out.println("salario gerente "+(hora*valorHora+adicional));
    }
}

```
# atividade 18

```java

package poo18;

/**
 * 18. Faça uma classe Produto com atributos nome e preco. Crie um método que
 * aplique desconto.
 *
 * @author Henrique 
 */
public class Produto {
    private String nome;
    private double preco;
    public Produto(){
}
    public void aplicarDesconto(double desconto){
        System.out.println("o valor com desconto é R$"+(preco-preco+(desconto/100)) );
    }
}

```
# atividade 19
```java
package poo19;

/**
 * 19. Implemente uma classe ContaCorrente que utilize composição com uma classe
 * Cliente.
 *
 * @author henri
 */
public class Cliente {

    private String nome;

    public Cliente() {
    }
    public String to

    String() {
        return "nome:" + nome;

    }
}

public class contaCorrente {

    private int numero;
    private double saldo;
    private Cliente cliente;

    public contaCorrente(int numero, double saldo, Cliente cliente) {
        this.numero = numero;
        this.saldo = saldo;
        this.cliente = cliente;
    }
}
```

# atividade 20

```java
package poo20;

/**
 * 20. Modele um sistema simples de locadora de filmes usando classes Filme,
 * Cliente e Locacao.
 *
 * @author henrique
 */
public class Filme {
    private String nome;
    private int ano;
    public Filme(){
        
    }
}

public class Cliente{
    private String nome;
    private String email;
    private String telefone;
    public Cliente(){
        
    }
}

public class Locacao{
    private String data;
    private Cliente cliente;
    private Filme filme;
    public Locacao(){
        
    }
}
```
