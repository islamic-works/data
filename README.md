## Dados para uso Offline no projeto de APP

## Sponsors

Apoiadores e patrocinadores do projeto

## Team

Equipe que está colaborando no projeto

## Glossary

Este arquivo possui os termos usados no glossário, inicialmente obtidos no link: http://muslimeislam.blogspot.com/p/glossario-islamico.html

## Glossary Link

Esta base de dados, informa os termos na aplicação que devem ser linkados com outros módulos, por exemplo estando no módulo chat, alguém digita um termo que está no glossário, este pode ser automáticamente lincado com o glossario, ou posso definir que determinados termos tenham um comportamento especifico conforme o módulo que ele foi identificado, assim informo o nome do módulo de origem `term.way.from` e qual o destino a ser dado a ele caso o usuário clique nele "term.way.to.module" se for apenas abrir outro módulo ou "term.way.to.url" com ou sem parâmetros para roteador por exemplo para uma definição especifica do termo.

O Agrande desafio (@TODO) é como programar no nativescript uma monitoração constante do chat para tal construção de links, e como varrer o código conforme o parametro "term.way.from" identificando o termo nos módulos e construindo atuomáticamente os links.

``` JSON
[
   {
      "term": "farj",
      "way": [
         {
            "from": "glossary",
            "to": {"module":"praytimes"}
         },
         {
            "from": "praytimes",
            "to": {"url":"glossary/item","params":["term"]}
         }
      ]
   }
]
```
