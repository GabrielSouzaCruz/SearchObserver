# Search and Sort Observer

Este projeto em Java oferece uma rica implementação de diversos algoritmos de ordenação e busca, com um diferencial: o uso do padrão de projeto *Observer* para monitorar e notificar as operações internas dos algoritmos, como comparações e trocas de elementos.

## 📝 Sobre o Projeto

O objetivo principal é fornecer uma ferramenta didática e prática para o estudo e visualização do comportamento de algoritmos clássicos. Através do padrão *Observer*, é possível acompanhar em tempo real cada passo da execução de um algoritmo de ordenação, obtendo *insights* sobre sua eficiência e funcionamento.

## ✨ Funcionalidades

  * **Padrão Observer**: Acompanhe as etapas de ordenação e busca através das classes `SortObserver` e `SearchObserver`.
  * **Implementação Genérica**: Os algoritmos são implementados com Generics (`<T>`), permitindo que sejam utilizados com qualquer tipo de objeto que implemente a interface `Comparable` ou através de um `Comparator` customizado.
  * **Exemplos Práticos**: A classe `App` demonstra como utilizar os algoritmos com uma classe `Pessoa`, ordenando e buscando por diferentes critérios (nome e data de nascimento).
  * **Leitura de Arquivos**: Carrega dados de arquivos de texto para serem utilizados com os algoritmos.

## 🚀 Algoritmos Implementados

### Algoritmos de Ordenação (`ObservableSort`)

Todos os algoritmos de ordenação estendem a classe `ObservableSort`, que notifica um `SortObserver` sobre comparações, trocas e a conclusão do processo.

  * **Bubble Sort**: Implementação do algoritmo Bubble Sort, incluindo uma versão otimizada.
  * **Insertion Sort**: Implementação do algoritmo Insertion Sort.
  * **Selection Sort**: Implementação do algoritmo Selection Sort.
  * **Quick Sort**: Implementação do algoritmo Quick Sort.

### Algoritmos de Busca (`SearchObserver`)

A classe `Busca` implementa algoritmos de busca que notificam um `SearchObserver` sobre as comparações e o resultado da busca.

  * **Busca Linear**: Implementação da busca linear.
  * **Busca Binária**: Implementação da busca binária.

## 📂 Estrutura do Projeto

```
.
├── src/
│   ├── App.java
│   ├── BubbleSort.java
│   ├── Busca.java
│   ├── InsertionSort.java
│   ├── ObservableSort.java
│   ├── Pessoa.java
│   ├── QuickSort.java
│   ├── SearchObserver.java
│   ├── SelectionSort.java
│   └── SortObserver.java
├── bin/
│   └── (arquivos .class compilados)
└── numeros.txt
└── numeros_aleatorios.txt
```

## ⚙️ Como Executar

1.  **Pré-requisitos**:

      * Java Development Kit (JDK) instalado.
      * Git (opcional, para clonar o repositório).

2.  **Clone o repositório (opcional)**:

    ```bash
    git clone https://github.com/GabrielSouzaCruz/SearchObserver.git
    cd SearchObserver
    ```

3.  **Compile o projeto**:
    Navegue até o diretório raiz do projeto e execute o comando de compilação do Java. Isso irá gerar os arquivos `.class` no diretório `bin/`.

    ```bash
    javac -d bin src/*.java
    ```

4.  **Execute a aplicação**:
    A classe `App.java` contém o método `main` para demonstrar o funcionamento dos algoritmos.

    ```bash
    java -cp bin App
    ```

    O programa irá ordenar uma lista de pessoas e depois solicitar dados para realizar uma busca.

## 🤝 Como Contribuir

Contribuições são sempre bem-vindas\! Se você tem alguma sugestão para melhorar este projeto, sinta-se à vontade para criar um *fork* e submeter um *pull request*.

1.  Faça um *fork* do projeto.
2.  Crie uma nova *branch* para sua funcionalidade (`git checkout -b feature/AmazingFeature`).
3.  Faça o *commit* de suas alterações (`git commit -m 'Add some AmazingFeature'`).
4.  Faça o *push* para a *branch* (`git push origin feature/AmazingFeature`).
5.  Abra um *Pull Request*.
