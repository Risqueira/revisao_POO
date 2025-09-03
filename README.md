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

```
```java
package atividadepoo14;

public class Biblioteca {
    private String nome;
    private Arraylist Livros<Livro>; //assossiaçao com a class Livro
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
public class Pessoa {

    private String nome;
    private int idade;
}

//subclasses abaixo, forma dentro de um arquivo class.
class Professor extends Pessoa {

    private String disciplina;
}

class Estudante extends Pessoa {

    private String curso;
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
    public void fazerSom(){
        System.out.println("O animal faz um som");
    }
}

class Cachorro extends Animal{
    @Override
    public void fazerSom(){
        System.out.println("O cachorro late");
    }
}
class Gato extends Animal{
    @Override
    public void fazerSom(){
        System.out.println("O gato mia");
    }
}
```
```java

package poo16;

public class POO16 {

    public static void main(String[] args) {
        
        //polimorfismo
        Animal a1 = new Cachorro();
        Animal a2 = new Gato();
        
        //Chama cada versao de som que cada animal faz
        a1.fazerSom();
        a2.fazerSom();
    }

}
```
