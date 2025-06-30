# A - Estrutura Fundamental

---

## Código A0 - Hello World

```java
public class A0_HelloWorld {
    public static void main(String[] args) {
        System.out.println("Hello World!");
    }
}
```

**Explicações:**

- `public`: Torna o método e a variável acessíveis fora da classe, permitindo que outras classes os chamem diretamente.
- `class`: Define uma classe.
- `static`: Indica que o método `main` pode ser usado sem criar uma instância da classe.
- `void`: O método não retorna nenhum valor.
- `String[] args`: Parâmetro do método `main` que recebe argumentos da linha de comando.

---

## Código A1_0 - Tipos primitivos (`int`, `double`)

```java
public class A1_0Teste {
    public static void main(String[] args) {
        // Declaração de variáveis inteiras e reais
        int numeroInteiro = 10;      // Tipo inteiro (int)
        double numeroReal = 5.75;    // Tipo real (double)
        
        // Exibindo os valores das variáveis
        System.out.println("Número inteiro: " + numeroInteiro);
        System.out.println("Número real: " + numeroReal);
    }
}
```

---

## Código A1_1 - Outros tipos primitivos (`byte`, `short`, `long`, `float`)

### Tipos Inteiros

- **byte**: Quando você precisa de um número pequeno e deseja economizar espaço (ex: contadores, datas).
  - Tamanho: 8 bits (1 byte)
  - Intervalo: -128 até 127
- **short**: Para números um pouco maiores que `byte`, mas ainda economizando memória (ex: pontuação em jogos).
  - Tamanho: 16 bits (2 bytes)
  - Intervalo: -32.768 até 32.767
- **int**: Usado para intervalos maiores.
  - Tamanho: 32 bits (4 bytes)
  - Intervalo: -2³¹ até 2³¹-1 (aprox. -2 bilhões até 2 bilhões)
- **long**: Para números muito grandes (ex: cálculos financeiros).
  - Tamanho: 64 bits (8 bytes)
  - Intervalo: -2⁶³ até 2⁶³-1

```java
public class A1_1Teste {
    public static void main(String[] args) {
        // Tipos inteiros
        byte numeroByte = 120;          // Tipo byte
        short numeroShort = 30000;      // Tipo short
        int numeroInt = 30000;          // Tipo int
        long numeroLong = 1000000000L;  // Tipo long (necessita do sufixo 'L')

        // Exibindo os valores das variáveis inteiras
        System.out.println("Número byte: " + numeroByte);
        System.out.println("Número short: " + numeroShort);
        System.out.println("Número int: " + numeroInt);
        System.out.println("Número long: " + numeroLong);
    }
}
```

### Tipos Reais

- **float**: Para números decimais com precisão moderada (ex: temperatura, pequenas distâncias).
  - Tamanho: 32 bits (4 bytes)
  - Precisão: ~6 a 7 dígitos decimais
- **double**: Para maior precisão em cálculos decimais (ex: cálculos científicos, financeiros).
  - Tamanho: 64 bits (8 bytes)
  - Precisão: ~15 dígitos decimais

```java
public class A1_2Teste {
    public static void main(String[] args) {
        // Tipos reais
        float numeroFloat = 5.75f;      // Tipo float (necessita do sufixo 'f')
        double numeroDouble = 19.99;    // Tipo double

        // Exibindo os valores das variáveis reais
        System.out.println("Número float: " + numeroFloat);
        System.out.println("Número double: " + numeroDouble);
    }
}
```

---

## Código A1_3 - Constante

- `static`: A constante pertence à classe, não à instância.
- `final`: Indica que a variável não pode ser alterada após ser definida.

```java
public class A1_3Teste {
   public static final double PI = 3.1416;

   public static void main(String[] args) {
       float valor = 12.123456789f;
      
       System.out.printf("Float com 6 casas decimais: %.6f\n", valor);
       System.out.printf("Float em notação científica: %e\n", valor);
       System.out.printf("Valor da constante PI: %.4f\n", PI);
   }
}
```

---

## Código A1_4 - Tipo primitivo `char`

```java
public class A1_4Teste {
    public static void main(String[] args) {
        // Tipo caractere
        char letraA = 'A'; // Tipo char, representa um único caractere

        // Exibindo o valor da variável char
        System.out.println("Caractere letra A: " + letraA);
    }
}
```

---

## Código A1_5 - Tipo primitivo `boolean`

```java
public class A1_5Teste {
    public static void main(String[] args) {
        // Tipo booleano, valores true ou false
        boolean ligado = true;   // Tipo boolean, valor true
        boolean desligado = false;  // Tipo boolean, valor false

        // Usando os valores booleanos
        System.out.println("O dispositivo está ligado? " + ligado);
        System.out.println("O dispositivo está desligado? " + desligado);
    }
}
```

---

## Código A1_6 - String básica

> **Nota:** `String` não é um tipo primitivo.

```java
public class A1_6Teste {
   public static void main(String[] args) {
       // String (não é um tipo primitivo)
       String texto = "Exemplo de texto";

       // Exibindo os valores
       System.out.println("String: " + texto);
   }
}
```
