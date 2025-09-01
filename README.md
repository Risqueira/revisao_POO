# revisao_POO

# Atividade 1
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
# Atividade 2

```java
12. Crie uma classe ContaBancaria com atributos numero, titular e saldo. Adicione
métodos depositar() e sacar(). Obs.: Nos métodos avaliar se existe saldo para
o saque e ao depositar verifique se o valor depositado não é negativo.
```
