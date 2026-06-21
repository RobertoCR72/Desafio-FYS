Copiloto FYS para Ativação de Padarias
Projeto desenvolvido para o desafio **"Copiloto de Vendas com IA para Atendimento ao Cliente"**, usando como inspiração o repositório público da DIO sobre a marca FYS.
> Status: versão inicial/documental. Este projeto não implementa uma aplicação completa; ele apresenta uma proposta de solução com IA, base de conhecimento, prompt estruturado e exemplos simulados de uso.
--## 1. Tema escolhido O tema escolhido foi um **copiloto de vendas para ativação de padarias**.
A ideia é apoiar vendedores, representantes ou profissionais de trade marketing que precisam apresentar a FYS para donos de padarias, responder objeções e sugerir pequenas ações de visibilidade no ponto de venda.
--## 2. Usuário principal da solução
O usuário principal é o **vendedor ou representante comercial** que visita ou prospecta padarias e precisa de apoio para:
- preparar uma abordagem comercial simples; - adaptar argumentos ao perfil da padaria; - responder objeções comuns;
- sugerir ações de exposição e experimentação; - enviar uma mensagem de follow-up após a conversa.
--## 3. Problema de vendas ou atendimento resolvido
O desafio identificado é que padarias são um canal relevante para bebidas não alcoólicas, mas podem ser pouco exploradas quando a força de vendas prioriza pontos de venda com maior potencial para cerveja.
Além disso, a FYS ainda enfrenta desafios como:
- baixo conhecimento da marca por parte de consumidores e clientes; - necessidade de gerar experimentação;- necessidade de melhorar visibilidade e disponibilidade no ponto de venda;
- objeções comuns de donos de padaria, como espaço limitado na geladeira, medo de baixo giro e
preferência por marcas já conhecidas.
---
## 4. Abordagem usada
A abordagem escolhida foi um **copiloto de vendas baseado em prompt e base de conhecimento**.
Nesta versão inicial, a solução funciona como um assistente que recebe informações simples sobre a
padaria e gera uma sugestão de abordagem comercial.
### Formato da entrada
O usuário informa:
- tipo de padaria;
- perfil dos clientes;
- objeção provável;
- espaço disponível;
- objetivo da abordagem.
### Formato da saída
A IA devolve:
1. pitch curto de apresentação;
2. argumentos de venda;
3. resposta para objeção;
4. sugestão de ativação de baixo custo;
5. mensagem de WhatsApp para follow-up.
---
## 5. Informações usadas como base de conhecimento
A base de conhecimento foi montada a partir do repositório público da DIO:
- README do repositório de inspiração;
- transcrição da live sobre a FYS;
- orientações do desafio final.### Pontos usados como referência
- A FYS é apresentada como refrigerante do Grupo HEINEKEN.
- A marca trabalha com comunicação leve, humor e autoironia.
- O produto citado na live tem foco em lata de 350 ml.
- A FYS busca ampliar conhecimento, disponibilidade, visibilidade e experimentação.
- O canal de padarias aparece como oportunidade relevante.
- O desafio citado envolve identificar, priorizar e ativar padarias, reduzindo dependência da força de
vendas tradicional.
Fontes utilizadas:
- Repositório DIO/FYS: https://github.com/digitalinnovationone/copiloto-vendas-ia-atendimento-cliente-
fys
- Transcrição da live: https://raw.githubusercontent.com/digitalinnovationone/copiloto-vendas-ia-
atendimento-cliente-fys/main/knowledge/transcricao-live-fys.txt
- Bootcamp DIO/HEINEKEN: https://www.dio.me/bootcamp/heineken-inteligencia-artificial-aplicada-vendas
---
## 6. Prompt principal da solução
O prompt principal está disponível em:
```text
prompts/copiloto-padarias.md
```
Resumo do funcionamento:
```text
Você é um copiloto de vendas da FYS para ajudar vendedores a abordar padarias.
Use a base de conhecimento fornecida sobre a marca, seu posicionamento, seus desafios comerciais e o
canal de padarias.
A partir do perfil informado, gere uma abordagem comercial simples e útil.
```
---
## 7. Exemplo de conversa gerada### Entrada do usuário
```text
Tipo de padaria: pequena padaria de bairro
Perfil dos clientes: moradores da região, café da manhã, almoço rápido e lanche da tarde
Objeção provável: já vendo marcas conhecidas, não sei se FYS vai girar
Espaço disponível: apenas uma prateleira pequena na geladeira
Objetivo: conseguir um teste inicial com poucas unidades
```
### Resposta esperada da IA
```text
1. Pitch curto
A FYS pode ser uma boa opção para testar na sua geladeira porque é um refrigerante do Grupo HEINEKEN,
com proposta mais moderna, sabores diferentes e comunicação leve. A ideia não é trocar tudo que você já
vende, mas colocar uma alternativa nova para o cliente experimentar.
2. Argumentos de venda
- Teste com baixo risco: começar com poucas unidades reduz o medo de produto parado.
- Curiosidade do consumidor: sabores diferentes podem chamar atenção de quem já está acostumado às
mesmas marcas.
- Consumo individual: a lata de 350 ml combina com café da manhã, almoço rápido e lanche.
3. Resposta para a objeção
Entendo que marcas conhecidas giram mais fácil. Por isso, a sugestão não é substituir o que já vende,
mas fazer um teste pequeno. Se tiver boa saída, você aumenta aos poucos. Se não girar, o risco foi
controlado.
4. Sugestão de ativação
Colocar poucas latas em uma área visível da geladeira, próximas aos produtos de maior saída, com uma
plaquinha simples: "Novo por aqui: experimente FYS".
5. WhatsApp de follow-up
Olá! Obrigado pela conversa de hoje. Como combinamos, a ideia é fazer um teste pequeno com FYS para
medir a aceitação dos clientes, sem mexer no que já funciona na padaria. Posso te enviar uma sugestão
inicial de pedido?```
---
## 8. Possíveis melhorias futuras
- Criar mais exemplos de padarias: bairro, premium, rodoviária, centro comercial e região escolar.
- Adicionar uma matriz simples de objeções e respostas.
- Criar uma interface em formulário para gerar respostas automaticamente.
- Usar dados públicos da região para priorizar bairros ou pontos de venda.
- Criar um simulador de conversa entre vendedor e dono da padaria.
- Medir quais argumentos geram maior aceitação em testes reais.
- Conectar a solução a uma planilha de leads para priorização comercial.
---
## 9. Estrutura do repositório
```text
copiloto-fys-padarias/
├── README.md
├── AGENTS.md
├── .gitignore
├── prompts/
│ └── copiloto-padarias.md
├── knowledge/
│ └── base-conhecimento-fys.md
├── examples/
│ ├── cenario-01-padaria-bairro.md
│ └── cenario-02-padaria-premium.md
└── docs/
└── criterios-avaliacao.md
```
---
## 10. Como usar este projeto
1. Leia a base de conhecimento em `knowledge/base-conhecimento-fys.md`.
2. Abra o prompt em `prompts/copiloto-padarias.md`.
3. Escolha um cenário em `examples/`.
4. Cole o prompt e o cenário em uma ferramenta de IA generativa.5. Analise se a resposta é útil, clara e coerente com a marca. 6. Ajuste o README com seus aprendizados.
--## 11. Observação importante
Este projeto é uma proposta educacional criada para o desafio da DIO. Ele não representa uma solução oficial da FYS, da HEINEKEN ou da DIO
