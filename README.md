# Design Patterns Study

Projeto de estudo dos padrões descritos pelo [Refactoring.Guru](https://refactoring.guru/design-patterns), usando Java 21 e Maven.

## Estrutura

- `creational`: agregador dos cinco patterns criacionais.
- `structural`: agregador dos sete patterns estruturais.
- `behavioral`: agregador dos dez patterns comportamentais.
- `docs/stories.md`: índice das histórias de domínio, com um exercício dentro de cada submódulo.

Cada pattern é um submódulo Maven independente, com a seguinte forma:

```text
categoria/
	pattern/
		pom.xml
		src/main/java/com/estudo/designpatterns/categoria/pattern/
		src/test/java/
```

	Por exemplo, o Builder fica em `creational/builder` e o Chain of Responsibility em `behavioral/chain-of-responsibility`. O nome do diretório e do artefato usa kebab-case; o pacote Java usa lower-case sem separadores. Cada pattern possui sua própria classe `Main`, seus testes e não depende de outros patterns neste estágio.

## Fluxo sugerido

1. Escolha uma história no índice `docs/stories.md`.
2. Entre no diretório do pattern e leia seu `docs/story.md`.
3. Modele uma primeira versão sem pattern e registre a dor concreta.
4. Implemente o pattern mantendo a mesma regra de negócio.
5. Compare os testes, a quantidade de condicionais e o acoplamento antes e depois.
6. Só mantenha o pattern se ele tornar a mudança descrita na história mais barata ou mais segura.

Execute o reactor completo, incluindo todos os submódulos, com:

```bash
mvn clean test
```

Para executar um pattern individual, entre no diretório dele e rode:

```bash
cd creational/builder
mvn compile exec:java
```

O mesmo formato funciona para qualquer outro submódulo.
