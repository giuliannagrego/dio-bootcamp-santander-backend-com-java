# ANATOMIA DAS CLASSES - JAVA

**Classe executável** -> Classe que tem a capacidade de inicialização do projeto ou de forma idependente, ela precisa conter o método principal >main< 

    ~~~java
    public class MinhaClasse {

        public static void main(String[] args) {
                    
            String primeiroNome = "Giulianna";
            String segundoNome = "Grego";

            String nomeCompleto = nomeCompleto (primeiroNome, segundoNome);

            System.out.println(nomeCompleto);

        }

        public static String nomeCompleto(String primeiroNome, String segundoNome) {
            return primeiroNome.concat(" ").concat(segundoNome);
        }
    }
    ~~~

- **Arquivo.java** -> Todo arquivo .java deve começar com letra *MAIÚSCULA*, se a palavra for composta, a segunda palavra também deve ser maiúscula, ex:
    Calculadora.java -> CalculadoraCientifica.java

- **Nome da classe no arquivo**: A classe deve possuir o mesmo nome do arquivo

- **Nome da variável**: toda variável deve ser escrita com letra *MINÚSCULA*, caso a palavra seja composta, a segunda palavra deverá iniciar com letra *MAIÚSCULA* (prática camelCase), ex:     ano / anoFabricacao
    *Existe uma regra adicional para variáveis quando queremos identificar que a variável não sofrerá alteração de valor, exemplo: queremos determinar que uma variável de nome **br** sempre representará **"Brasil"** e nunca mudará seu valor, logo, determinamos como escrita o código abaixo:*
    ~~~java
    {   
        String BR = "Brasil"
        double PI = 3.14
        int ESTADOS_BRASIL = 27
        int ANO_2000 = 2000

        //como garantia de que os valores não serão alterados, também utilizamos a expressão <final>, antes de declarar a variável 
        
        final String BR = "Brasil"
    }
    ~~~

    Regras de variáveis:

    - Deve conter apenas **letras**, **_ (underline)**, **$** ou os **números** de 0 a 9;
    - Deve obrigatóriamente se iniciar por uma **letra** (preferencialmente), **_** ou **$**, *jamais com números*;
    - Deve iniciar com uma letra minúscula (boa prática);
    - Não pode conter espaços;
    - Não podemos usar palavras-chave na linguagem;
    - O nome deve ser único dentro de um escopo;



## IDENTAÇÃO

Termo utilizado para escrever o código do programa de forma hierárquica, facilitando a visualização e o entendimento do programa