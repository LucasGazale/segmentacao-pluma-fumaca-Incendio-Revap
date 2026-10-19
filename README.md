# Segmentação de pluma de fumaça com o SAM 2

Trabalho da disciplina de **Modelagem Computacional**: segmentação de uma pluma de fumaça em uma fotografia com o *Segment Anything Model 2* (SAM 2), avaliação crítica da máscara obtida e proposição de melhorias nos prompts, no código e na apresentação dos resultados.

**Autor(a):** Lucas alves Gazale
**Disciplina:** Modelagem Computacional

---

## 1. Contexto

O estudo toma como base a notícia do G1 sobre o incêndio na refinaria Henrique Lage (Revap), em São José dos Campos (SP), ocorrido em 29 de setembro de 2019: [Incêndio na Revap mobiliza bombeiros e fumaça assusta moradores em São José, SP](https://g1.globo.com/sp/vale-do-paraiba-regiao/noticia/2019/09/29/incendio-na-revap-mobiliza-bombeiros-e-fumaca-assusta-moradores-em-sao-jose-sp.ghtml).

O incêndio atingiu tanques de armazenamento de produtos utilizados na produção de asfalto e óleo combustível e gerou uma densa coluna de fumaça preta, visível em cidades vizinhas. A segmentação de plumas desse tipo é relevante para o monitoramento de emergências, pois permite estimar a extensão e a forma da fumaça a partir de imagens.

## 2. Objetivo

Segmentar a pluma de fumaça com o SAM 2 e:

1. avaliar se a máscara cobre a pluma, se inclui regiões que não pertencem a ela e se deixa partes da fumaça de fora;
2. comparar pelo menos três configurações de prompt (caixa delimitadora, pontos positivos e pontos negativos);
3. apresentar lado a lado a imagem original, a máscara binária e a máscara sobreposta;
4. identificar quais características da imagem dificultam a segmentação: iluminação, contraste e semelhança entre fumaça e nuvens.
