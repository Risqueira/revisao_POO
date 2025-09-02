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


package atividadepoo14;

import java.util.ArrayList;

public class Biblioteca {
    
    public ArrayList<Livro> Livro = new ArrayList<>();
    
}

}

```
