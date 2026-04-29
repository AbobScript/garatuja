# Garatuja Enzo Zinelli
Garatujas são os primeiros rabiscos e expressões gráficas espontâneas de crianças, geralmente entre 0 e 6 anos, representando uma etapa fundamental para o desenvolvimento da coordenação motora fina, criatividade e comunicação pré-verbal. Esses traços, que evoluem com o tempo, permitem que a criança explore o papel, registre emoções e inicie sua representação do mundo. No caso desse arquivo, será utilizado com o objetivo de criar anotações simples para que eu, um iniciante, tenha uma forma simples e rápida de retornar a tópicos caso necessário.

## [HTML]
Linguagem de marcação utilizada em sites web, definindo elementos como texto, links, videos, etc.

## [CSS]

Linguagem de estilo para estilizar o HTML.

# [JS X JAVA X TS]
## JAVASCRIPT
JavaScript é uma linguagem leve e dinâmica, usada principalmente para criar interatividade em páginas web. Roda direto no navegador e também no servidor (com Node.js). É flexível, mas isso também pode gerar mais erros se o código crescer muito.

## Exemplo:

<pre>function somar(a, b) {
  return a + b;
}

console.log(somar(5, 3));</pre>

## TYPESCRIPT
TypeScript é basicamente um “JavaScript melhorado”. Ele adiciona tipagem (ou seja, você define tipos de variáveis, funções, etc.), o que ajuda a evitar erros antes mesmo de rodar o código. No final, o TypeScript é convertido em JavaScript para funcionar no navegador. É muito usado em projetos grandes porque organiza melhor o código.

## Exemplo:
<pre>
  function somar(a: number, b: number): number {
  return a + b;
}

console.log(somar(5, 3));
</pre>

## JAVA
Java já é outra coisa. É uma linguagem mais antiga, forte e totalmente tipada, usada principalmente para sistemas grandes, backend, aplicativos Android e aplicações corporativas. Não roda direto no navegador como JavaScript. Precisa de uma máquina virtual (JVM) para executar.

## Exemplo:

<pre>
  public class Main {
    public static int somar(int a, int b) {
        return a + b;
    }

    public static void main(String[] args) {
  
        System.out.println(somar(5, 3));
    }
}
</pre>

# Programação Orientada ao Objeto

## Classe
Estrutura que define um molde para criar objetos.
Em TypeScript, utiliza a palavra-chave class.

## Objeto
Instância de uma classe.
Representa um elemento com estado (atributos) e comportamento (métodos).

## Atributo
Variável definida dentro de uma classe.
Armazena dados relacionados ao objeto.

## Método
Função definida dentro de uma classe.
Representa ações ou comportamentos do objeto.

## Getters e Setters
Métodos especiais para acessar (get) e modificar (set) atributos.
Permitem controle e validação no acesso aos dados.

## Construtor
Método especial chamado ao criar um objeto.
Usado para inicializar atributos da classe.

## Herança
Permite que uma classe herde propriedades e métodos de outra.
Utiliza a palavra-chave extends no TypeScript.

## Encapsulamento
Restrição de acesso direto aos dados da classe.
Utiliza modificadores como public, private e protected.

## Polimorfismo
Capacidade de métodos terem comportamentos diferentes.
Pode ocorrer via sobrescrita (override) ou interfaces.

# Programação 1 - Programação Orientada a Objetos (POO)

## O que é POO?

A Programação Orientada a Objetos (POO) é um paradigma de programação baseado na abstração do mundo real, utilizando o conceito de objetos, que são instâncias de classes. As classes, por sua vez, representam categorias ou modelos de entidades.

A POO permite organizar o código de forma modular e reutilizável, facilitando a manutenção e a evolução do sistema, além de contribuir para a modelagem de problemas complexos.

## Conceitos fundamentais da POO

- ☑ Classe  
- ☑ Objeto  
- ☑ Atributo  
- ☑ Método  
  - ☐ Sobrescrita (override)    
  - ☐ Sobrecarga (overload)  
- ☑ Getters e Setters  
- ☑ Encapsulamento  
  - ☑ Modificadores de acesso (`public`, `private`, `protected`)  
  - ☐ Imutabilidade (`readonly`)  
- ☑ Construtor  
- ☑ Métodos e Atributos estáticos (`static`)  
- ☑ Herança  
- ☐ Polimorfismo  
- ☐ Abstração  
  - ☐ Classes abstratas  
  - ☐ Interface  
- ☐ Composição  
  - ☐ Associação  
  - ☐ Agregação

> Conteúdo já abordado nesta versão do texto estão marcados com ☑, enquanto tópicos a serem abordados em versões futuras estão marcados com ☐.

## Conhecimento prévio necessário

- Noções básicas de programação
- Programação estruturada
- Variáveis e tipos de dados
- Funções e procedimentos
- Estruturas de controle (`if`, `for`, `while`, etc.)

## Programação Estruturada (PE) vs Programação Orientada a Objetos (POO)

Na programação estruturada, o foco está na criação de funções e procedimentos que manipulam dados. Já na programação orientada a objetos, o foco está na criação de objetos que combinam dados (atributos) e comportamentos (métodos).

| PE vs POO              | Programação Estruturada                              | Programação Orientada a Objetos                                                             |
| ---------------------- | ---------------------------------------------------- | ------------------------------------------------------------------------------------------- |
| Variáveis vs Atributos | Variáveis são usadas para armazenar dados.           | Atributos armazenam dados dentro de um objeto ou classe.                                    |
| Funções vs Métodos     | Funções são blocos de código que realizam uma tarefa | Métodos são funções associadas a um objeto ou classe e podem acessar seus atributos.        |

A tabela apresenta comparações introdutórias entre programação estruturada e programação orientada a objetos. No entanto, a POO possui conceitos sem equivalentes diretos na programação estruturada, como encapsulamento, herança e polimorfismo.

Além disso, os conceitos de classe e objeto são fundamentais na POO e não possuem correspondência direta na programação estruturada.

## Classe e Objeto

**Classe**: molde ou estrutura que define as características e os comportamentos de um tipo específico de objeto. Ela atua como modelo para criação de instâncias.

**Objeto**: instância de uma classe, isto é, uma materialização da estrutura definida. Cada objeto pode possuir valores diferentes para os atributos da mesma classe.

> [!NOTE]
> Analogia:
> A Programação Estruturada pode ser comparada a uma receita de bolo, com ingredientes (variáveis) e instruções (funções).  
> A Programação Orientada a Objetos pode ser comparada a peças de LEGO, em que cada peça representa um objeto com características (atributos) e comportamentos (métodos), combináveis para formar estruturas mais complexas.

### A referência `this` dentro da classe

A palavra reservada `this` é utilizada dentro de classes para referenciar o objeto atual (instância em execução).

Considere o código: `const minhaReferencia = new MinhaClasse();`.

- O lado esquerdo (`const minhaReferencia`) é a variável que armazenará a referência do objeto.
- O lado direito (`new MinhaClasse()`) cria o objeto e retorna sua referência.

Quando `new MinhaClasse()` é executado, um novo objeto é criado em memória e sua referência é atribuída à variável indicada.

Por esse motivo, dentro da classe, utiliza-se `this` para acessar atributos e métodos da instância atual, independentemente do nome da variável externa que armazenará essa referência.

*Por que usar `this` e não o nome da variável (como `minhaReferencia`)?*

Porque o nome da variável é definido fora da classe e pode variar:

```typescript
const a = new MinhaClasse();
const b = new MinhaClasse();
const c = new MinhaClasse();
```

Dentro da classe, os nomes `a`, `b` e `c` não existem. Portanto, usa-se `this`, que sempre referencia o objeto atual.

> [!TIP]
> Recapitulando:
>
> |                                              `const minhaReferencia` | `=` | `new MinhaClasse()`                                                                                                                     |
> | -------------------------------------------------------------------: | :-: | :-------------------------------------------------------------------------------------------------------------------------------------- |
> | Variável (ou constante) à qual a referência do objeto será atribuída |  ←  | Criação de um objeto a partir da classe `MinhaClasse`. A expressão retorna a referência do objeto criado, atribuída à variável. Como o nome externo ainda não é conhecido dentro da classe, utiliza-se `this`. |

## Prática: exemplo de classe e objetos em TypeScript

Considere uma classe para representar quadriláteros, com atributos de lados e métodos para cálculo de área, perímetro e verificação de quadrado:

```typescript
class Quadrilatero {
  lado1: number;
  lado2: number;

  calcularArea(): number {
    return this.lado1 * this.lado2;
  }

  calcularPerimetro(): number {
    return 2 * (this.lado1 + this.lado2);
  }

  eQuadrado(): boolean {
    return this.lado1 === this.lado2;
  }
}
```

Para criar objetos, utiliza-se `new`, associando o resultado a uma variável ou constante:

```typescript
const q1 = new Quadrilatero();
q1.lado1 = 5;
q1.lado2 = 10;

const q2 = new Quadrilatero();
q2.lado1 = 7;
q2.lado2 = 7;

console.log(q1.calcularArea()); // Saída: 50
console.log(q1.eQuadrado()); // Saída: false

console.log(q2.calcularArea()); // Saída: 49
console.log(q2.eQuadrado()); // Saída: true
```

Nesse exemplo, os objetos `q1` e `q2` pertencem à mesma classe, mas possuem estados diferentes. Isso evidencia que cada objeto é uma instância única.

> [!NOTE]
> O exemplo é intencionalmente simples, com foco didático.

> [!NOTE]
> O acesso a atributos e métodos é realizado por notação de ponto (`.`), por exemplo: `q1.lado1` e `q1.calcularArea()`.

> [!TIP]
> Recapitulação:
>
> | Termo      | Descrição |
> | ---------- | --------- |
> | `classe`   | Molde que define características e comportamentos. |
> | `objeto`   | Instância de uma classe. |
> | `atributo` | Variável pertencente ao objeto/classe. |
> | `método`   | Função pertencente ao objeto/classe. |

## Construtor

O construtor é um método especial chamado automaticamente na criação do objeto. Seu objetivo principal é inicializar atributos e garantir estado inicial válido.

```typescript
class Pessoa {
  nome: string;
  idade: number;

  constructor(paramNome: string, paramIdade: number) {
    this.nome = paramNome;
    this.idade = paramIdade;
  }
}
```

Uso:

```typescript
const pessoa1 = new Pessoa("Alice", 30);
console.log(pessoa1.nome); // Saída: Alice
console.log(pessoa1.idade); // Saída: 30
```

Sem construtor explícito, valores essenciais podem ficar ausentes, aumentando risco de inconsistência.

Exemplo com `Quadrilatero`:

```typescript
class Quadrilatero {
  lado1: number;
  lado2: number;

  constructor(paramLado1: number, paramLado2: number) {
    this.lado1 = paramLado1;
    this.lado2 = paramLado2;
  }

  calcularArea(): number {
    return this.lado1 * this.lado2;
  }

  calcularPerimetro(): number {
    return 2 * (this.lado1 + this.lado2);
  }

  eQuadrado(): boolean {
    return this.lado1 === this.lado2;
  }
}
```

```typescript
const q1 = new Quadrilatero(5, 10);
console.log(q1.calcularArea()); // Saída: 50
console.log(q1.calcularPerimetro()); // Saída: 30
console.log(q1.eQuadrado()); // Saída: false
```

## Herança

A herança promove reutilização de código e organização hierárquica entre classes.

```typescript
class Quadrado extends Quadrilatero {
  constructor(paramLado: number) {
    super(paramLado, paramLado);
  }

  eQuadrado(): boolean {
    return true;
  }
}
```

A subclasse `Quadrado` herda atributos e métodos de `Quadrilatero`, mas redefine comportamento específico quando necessário.

> [!NOTE]
> Herança não significa cópia física de código, e sim reutilização por relação entre classes. A superclasse permanece como origem dos comportamentos herdados.

## Encapsulamento

O encapsulamento protege o estado interno da classe, controlando acesso por modificadores (`public`, `private`, `protected`).

| Modificador | Descrição | Acesso |
| ----------- | --------- | ------ |
| `public`    | Acessível de qualquer lugar. | Dentro e fora da classe. |
| `private`   | Acessível apenas na classe. | Apenas dentro da classe. |
| `protected` | Acessível na classe e em subclasses. | Classe e subclasses. |

Sem encapsulamento, estados inválidos podem ser introduzidos em objetos.

```typescript
class Quadrilatero {
  private lado1: number;
  private lado2: number;

  constructor(paramLado1: number, paramLado2: number) {
    this.lado1 = paramLado1;
    this.lado2 = paramLado2;
  }

  calcularArea(): number {
    return this.lado1 * this.lado2;
  }

  calcularPerimetro(): number {
    return 2 * (this.lado1 + this.lado2);
  }

  eQuadrado(): boolean {
    return this.lado1 === this.lado2;
  }
}
```

Com `private`, o TypeScript impede acesso externo direto e reforça consistência do objeto.

## Getters e Setters

Getters e setters permitem leitura e escrita controladas de atributos privados.

- **Getter**: retorna valor.
- **Setter**: altera valor com validação.

```typescript
class Quadrilatero {
  private lado1: number;
  private lado2: number;

  constructor(paramLado1: number, paramLado2: number) {
    this.setLado1(paramLado1);
    this.setLado2(paramLado2);
  }

  getLado1(): number {
    return this.lado1;
  }

  getLado2(): number {
    return this.lado2;
  }

  setLado1(novoLado1: number): void {
    if (novoLado1 <= 0) throw new Error("lado1 deve ser maior que zero.");
    this.lado1 = novoLado1;
  }

  setLado2(novoLado2: number): void {
    if (novoLado2 <= 0) throw new Error("lado2 deve ser maior que zero.");
    this.lado2 = novoLado2;
  }

  calcularArea(): number {
    return this.lado1 * this.lado2;
  }
}
```

### Getters e Setters em JavaScript/TypeScript

Também é possível utilizar sintaxe de propriedades com `get` e `set`:

```typescript
class Quadrilatero {
  private _lado1: number;
  private _lado2: number;

  constructor(paramLado1: number, paramLado2: number) {
    this.lado1 = paramLado1;
    this.lado2 = paramLado2;
  }

  get lado1(): number {
    return this._lado1;
  }

  set lado1(novoLado1: number) {
    if (novoLado1 <= 0) throw new Error("lado1 deve ser maior que zero.");
    this._lado1 = novoLado1;
  }

  get lado2(): number {
    return this._lado2;
  }

  set lado2(novoLado2: number) {
    if (novoLado2 <= 0) throw new Error("lado2 deve ser maior que zero.");
    this._lado2 = novoLado2;
  }

  get area(): number {
    return this.lado1 * this.lado2;
  }
}
```

## Métodos e atributos estáticos

Métodos e atributos estáticos pertencem à classe, não às instâncias. Seu acesso ocorre diretamente pelo nome da classe e é indicado para comportamentos que não dependem do estado de um objeto específico.

```typescript
class Quadrado {
  private _lado: number;

  constructor(paramLado: number) {
    this.lado = paramLado;
  }

  get lado(): number {
    return this._lado;
  }

  set lado(novoLado: number) {
    if (novoLado <= 0) throw new Error("lado deve ser maior que zero.");
    this._lado = novoLado;
  }

  get area(): number {
    return this.lado * this.lado;
  }

  static maiorArea(q1: Quadrado, q2: Quadrado, ..qn: Quadrado[]): Quadrado {
    let maior = q1;
    const quadrados = [q1, q2, ...n];
    for (const q of quadrados) {
      if (q.area > maior.area) {
        maior = q;
      }
    }
    return maior;
  }
}
```
