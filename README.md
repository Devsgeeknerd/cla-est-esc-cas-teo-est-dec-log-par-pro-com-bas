<!-- Título -->
# Estruturas “escolha-caso” — Teoria

***Conteúdo da Aula:***

A estrutura de decisão `escolha-caso` é utilizada quando temos muitas possibilidades para serem avaliadas ao mesmo tempo.

Ela recebe uma expressão de avaliação e verifica em qual dos casos a expressão se encaixa melhor.

Vamos imaginar o seguinte cenário:

* Nós podemos ter 5 categorias de números:
  * Números muito pequenos, que são de 0 até 10;
  * Números pequenos, que são de 11 até 100;
  * Números médios, que são de 101 até 1000;
  * Números grandes, que são de 1001 até 10000;
  * Números não classificados, que não estão em nenhuma destas situações.

Nosso algoritmo irá ler um número que o usuário irá fornecer e, com base neste número, irá informar a qual categoria ele pertence.

Perceba que temos pelo menos cinco categorias nas quais o número pode ser enquadrado de acordo com este valor, o que é uma quantidade de possibilidades considerável.

Poderíamos resolver isso com a estrutura `se-então-senão`; porém, nosso algoritmo ficaria com a codificação muito extensa e confusa, tendo em vista que precisaríamos de 5 estruturas `se-então-senão` encadeadas.

Para esta situação, podemos então utilizar a estrutura `escolha-caso`.

Veja como nosso algoritmo ficaria com uma **pseudo-linguagem**:

```md
escrever "Usuário, digite um número: ";
numeroDigitado : inteiro = ler o número digitado;
escolha (numeroDigitado)
  caso 0 até 10:
    escrever "Número muito pequeno";
  caso 11 até 100:
    escrever "Número pequeno";
  caso 101 até 1000:
    escrever "Número médio";
  caso 1001 até 10000:
    escrever "Número grande";
  outro-caso:
    escrever "Número sem classificação";
```

Veja que a estrutura `escolha-caso` é perfeita para avaliação de variáveis quando as condições onde a variável pode se encaixar são muitas.

Perceba que ainda utilizamos a estrutura `outro-caso`:

* Ela é executada quando a variável analisada não se encaixa em nenhum caso (porém, a estrutura `outro-caso` é opcional).

Esta estrutura fará com que somente o bloco com o caso correspondente à variável analisada seja executado.

Os demais blocos serão ignorados.

<!-- Informações -->
## &#8505; Informações

![Visitors](https://api.visitorbadge.io/api/visitors?path=Devsgeeknerd%2Fcla-est-esc-cas-est-dec-log-par-pro-com-bas&label=Visitantes&labelColor=%23700070&labelStyle=none&countColor=%23000fff&style=plastic&color=%23ffffff "Total de Visitante")
&nbsp;
![Followers](https://img.shields.io/github/followers/Devsgeeknerd?style=p&label=Seguidores&labelColor=800080&color=000fff "Total de Seguidores")
&nbsp;
![Watchers](https://img.shields.io/github/watchers/Devsgeeknerd/cla-est-esc-cas-est-dec-log-par-pro-com-bas?style=p&label=Observadores&labelColor=800080&color=000fff "Total de Observadores")
&nbsp;
![Stars](https://img.shields.io/github/stars/Devsgeeknerd/cla-est-esc-cas-est-dec-log-par-pro-com-bas?style=p&label=Estrelas&labelColor=800080&color=000fff "Total de Estrelas")
&nbsp;
![Forks](https://img.shields.io/github/forks/Devsgeeknerd/cla-est-esc-cas-est-dec-log-par-pro-com-bas?style=p&label=Bifurcações&labelColor=800080&color=000fff "Total de Bifurcações")
&nbsp;
![Repo Size](https://img.shields.io/github/repo-size/Devsgeeknerd/cla-est-esc-cas-est-dec-log-par-pro-com-bas?style=p&label=Tamanho&labelColor=800080&color=000fff "Tamanho do Repositório")
&nbsp;
![License](https://img.shields.io/github/license/Devsgeeknerd/cla-est-esc-cas-est-dec-log-par-pro-com-bas?style=p&label=Licença&labelColor=800080&color=000fff "Licença do Repositório")
