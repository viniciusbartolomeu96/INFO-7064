# INFO7064 – Tópicos em Processamento de Imagens

## Descrição da Tarefa

Neste trabalho, você deverá implementar uma pipeline de segmentação de imagens por textura, utilizando algoritmos clássicos (sem deep learning).  
O objetivo é explorar filtros de textura para agrupar regiões semelhantes em um conjunto de imagens de um mesmo domínio (médico, paisagem, urbano, equipamentos, agrícola etc.).

---

## Requisitos Gerais

1. **Seleção de imagens**  
   - Escolha **ao menos 16 imagens** de um mesmo tipo (por exemplo, imagens médicas, paisagens, cenários urbanos, equipamentos industriais, áreas agrícolas etc.).

2. **Filtros de textura**  
   - Defina um conjunto de filtros de textura em **pelo menos 3 escalas**.  
     - Orientações obrigatórias:  
       - Horizontal  
       - Vertical  
       - Diagonal a 45°  
       - Diagonal a 135°  
       - Circular  
   - Duas estratégias sugeridas:  
     - Criar filtros em 3 escalas distintas e aplicá-los diretamente.  
     - Trabalhar com filtros em escala única e, a cada iteração, aplicar um filtro gaussiano + reduzir a imagem em metade de cada dimensão.

3. **Extração de descritores**  
   - Divida cada imagem em janelas (patches) e, para cada janela, compute estatísticas de textura (por exemplo, média dos valores de resposta de cada filtro).

4. **Agrupamento (clustering)**  
   - Utilize um algoritmo clássico de agrupamento (por exemplo, K-Means) baseado em distância euclidiana em N-dimensões para agrupar as janelas semelhantes.

5. **Visualização dos resultados**  
   - Gere imagens que mostrem a segmentação, colorindo cada região de acordo com o cluster ao qual pertence.

---

## Ferramentas e Linguagens Permitidas

- **Python + OpenCV** (pode usar Google Colab)  
- **C ou C++** (bibliotecas à escolha)  

---

## Trabalho em Grupo

- **2 a 4 participantes** por grupo.  
- **Atenção:** grupos fora desse intervalo sofrerão desconto de 25% na nota por participante excedente ou faltante.

---

## Entrega

- **Relatório** no formato de artigo científico (PDF), contendo:  
  - Introdução e motivação  
  - Descrição da metodologia (filtros, escalas, extração de descritores, clustering)  
  - Experimentos e resultados (com figuras das segmentações)  
  - Conclusões e possíveis extensões  
  - **Link clicável para o repositório Git** com o código-fonte e instruções de uso.

---




