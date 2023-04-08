# Clean Architecture - Use Cases para Product

- A aplicação deste módulo incorpora a _Clean Architecture_ na aplicação de um módulo anterior: _DDD_ - Modelagem Tática. Isso quer dizer que a aplicação aproveita, como base, a estrutura de um projeto em que se trabalham os _patterns_ de _Domain-Driven Design_.

- O Contexto Limitado da aplicação corresponde a uma área responsável pela Conclusão de Vendas;
- Inicialmente, o Contexto Limitado foi subdividido em módulos: 1. Gerenciamento de pedidos (_checkout_); 2. Gerenciamento de clientes (_customer_); 3. Gerenciamento de produtos (_product_);

- O coração da aplicação, ou seja, as Entidades ou _Enterprise Business Rules_ da _Clean Architecture_ corresponde aos módulos do _DDD_, sendo que cada módulo concentra regras de negócio próprias.

- A _Clean Architecture_ adiciona uma camada nova à aplicação: _usecase_. Ela vai ser responsável por definir as intenções no sistema. Sob o diretório de _usecase_, é definido um novo diretório correspondente a cada uma das Entidades: _checkout_, _customer_, _product_. E sob cada diretório das Entidades, são definidos diretórios para cada um dos casos de uso, porque cada caso de uso tem um propósito ou intenção diferente no sistema.

- Por exemplo, com relação a _customer_, vamos imaginar um caso de uso em que a intenção seja a de buscar um cliente - aí, cria-se um diretório _find_.

- É nesse contexto que este desafio propõe-se a:

- Criar casos de uso que correspondam às operações de criar, buscar, listar e atualizar produtos no sistema;

- Implementar os testes unitários e de integração de cada caso de uso.

> N.T. 1: Linguagem de programação para este desafio: _TypeScript_.
> N.T. 2: A solução para este desafio envolve criar a seguinte árvore de diretórios:
>
> > /src/usecase/product/create
> > /src/usecase/product/find
> > /src/usecase/product/list
> > /src/usecase/product/update
