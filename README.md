# 🖼️ Grupo 3 - Rotação e Redimensionamento de Imagens

**Acesse o código completo do projeto [aqui](https://colab.research.google.com/github/PedroLuizPG/Processamento-de-Imagens_E01_Grupo3/blob/main/src/Projeto.ipynb).**


## 🎯 Objetivo Geral
Criar módulos em **Python** que permitam o **redimensionamento** e a **rotação de imagens digitais**, preservando a proporção e a qualidade final.

---

## 🎯 Objetivos Específicos

- Upload individual ou múltiplo de imagens  
- Pré-visualização antes do processamento  
- Redimensionamento sem distorção  
- Rotação em ângulos fixos e livres  
- Controle da qualidade mínima (ex.: JPEG ≥ 80%)  
- Comparação entre imagem original e processada  
- Registro em histórico para auditoria  
- Suporte a múltiplos usuários simultâneos  

---

## ⚙️ Funcionalidades Principais

| **Função** | **Entrada** | **Saída** | **Descrição** |
|-------------|-------------|-----------|----------------|
| **Upload** | Imagem do usuário | Arquivo armazenado | Envio de uma ou várias imagens. |
| **Pré-visualização** | Imagem enviada | Imagem exibida | Confirmação da imagem antes do processamento. |
| **Redimensionar** | Imagem original, largura/altura | Imagem ajustada | Mantém proporção usando interpolação bilinear/bicúbica. |
| **Rotacionar** | Imagem original, ângulo | Imagem girada | Aplicada via transformada afim (*affine transform*). |
| **Comparação** | Original + processada | Exibição lado a lado | Valida se o resultado atende ao esperado. |
| **Salvamento** | Imagem processada | Arquivo exportado | Exporta em formatos e qualidades definidas. |
| **Histórico** | Operações realizadas | Registro | Armazena para auditoria e rastreabilidade. |
| **Qualidade** | Imagem processada JPEG | Aprovada/Rejeitada | Aceita somente qualidade ≥ 80%. |

---

## 🔄 Fluxo de Execução do Módulo
  

### **Fluxo de Operações (Passo a Passo)**

1. **Upload**  
   O usuário envia uma ou mais imagens para o sistema.

2. **Pré-visualização**  
   A imagem é exibida para que o usuário confirme antes do processamento.

3. **Definição de Parâmetros**  
   O usuário define as dimensões (largura e altura) para redimensionamento ou o ângulo desejado para rotação.

4. **Processamento (Redimensionar/Rotacionar)**  
   O módulo executa o redimensionamento e/ou rotação utilizando transformações matemáticas, preservando a proporção e a qualidade da imagem.

5. **Comparação**  
   O sistema apresenta a imagem original e a processada lado a lado, facilitando a avaliação dos resultados.

6. **Salvamento**  
   A imagem final pode ser exportada em diferentes formatos (JPEG, PNG, BMP) e níveis de qualidade.

7. **Histórico**  
   Todas as operações são registradas, permitindo auditoria e rastreabilidade das ações realizadas no sistema.

---

## 💾 Tecnologias Utilizadas
- **Python** — Linguagem principal usada para o desenvolvimento do projeto.  
- **scikit-image (`skimage.transform`)** — Aplicação de transformações geométricas em imagens, como rotação e redimensionamento.  
- **OpenCV (`cv2`)** — Processamento e manipulação de imagens digitais.  
- **Matplotlib (`matplotlib.pyplot`)** — Visualização gráfica e exibição de imagens e comparações.  
- **NumPy (`numpy`)** — Manipulação de arrays e operações matemáticas sobre matrizes de pixels.  
- **OS** — Gerenciamento de diretórios e arquivos.  
- **Time** — Controle de tempo de execução e medições de desempenho.  
- **Datetime** — Registro de data e hora de execução dos testes.  
- **IPython.display** — Exibição dinâmica de saídas e mensagens formatadas no ambiente do Colab.  
- **Pillow (`PIL`)** — Manipulação, conversão e salvamento de imagens.  
- **Pandas** — Criação e manipulação de tabelas de resultados e comparações.  
- **Google Colab Files (`google.colab.files`)** — Upload e download de arquivos dentro do ambiente Colab.  
- **Zipfile** — Compactação e descompactação de conjuntos de imagens.  
- **Ipywidgets** — Criação de controles interativos para ajustar parâmetros e visualizar resultados dinamicamente.
---

## 🧠 Descrição Técnica

O projeto foi desenvolvido utilizando diversas bibliotecas e ferramentas voltadas para o **processamento e análise de imagens**, com o objetivo de realizar transformações, visualizações e comparações de resultados de forma eficiente.  
A seguir estão as principais tecnologias empregadas:

- **`skimage.transform`** – utilizada para aplicar transformações geométricas em imagens, como rotação e redimensionamento, mantendo a qualidade visual.  
- **`cv2 (OpenCV)`** – biblioteca poderosa para manipulação e processamento de imagens, responsável por leitura, exibição e conversão entre diferentes formatos.  
- **`matplotlib.pyplot`** – empregada na visualização de imagens e gráficos comparativos de resultados.  
- **`numpy`** – utilizada para operações matemáticas e manipulação de matrizes de pixels.  
- **`os` e `time`** – usadas para gerenciamento de diretórios, arquivos e controle de tempo de execução dos processos.  
- **`datetime`** – responsável por registrar data e hora das execuções, auxiliando no versionamento e acompanhamento dos testes.  
- **`IPython.display`** – empregada para exibir saídas dinâmicas, como imagens e mensagens formatadas no ambiente do Colab.  
- **`Pillow (PIL)`** – utilizada para abrir, converter e salvar imagens em múltiplos formatos.  
- **`pandas`** – usada na criação e manipulação de tabelas de comparação de resultados, facilitando a análise quantitativa.  
- **`google.colab.files`** – possibilita o upload e download de arquivos diretamente no ambiente do Google Colab.  
- **`zipfile`** – usada para compactar e descompactar conjuntos de imagens de teste.  
- **`ipywidgets`** – responsável pela criação de interfaces interativas, permitindo controlar parâmetros de forma dinâmica durante a execução do projeto.


## 📈 Aplicações

O módulo de Rotação e Redimensionamento pode ser utilizado em diversas áreas, como:

- Edição e tratamento digital de imagens  
- Sistemas de visão computacional  
- Reconhecimento de padrões  
- Otimização de imagens para web  
- Processos industriais e inspeção automatizada  

---

## 👨‍💻 Equipe — Grupo 3
### Responsabilidade de cada integrante: 
- Gabriel Schettino :
  -> responsável pela estrutura base do projeto, upload de imagens com validação, desenvolvimento das funções de rotação e redimensionamento, criação e atualização do vídeo de demonstração, implementação de métricas e comparações, definição da arquitetura do código e organizar as funcionalidades para cada integrante.
- Igor Gabriel :
  -> responsável pelas funções para aplicar transformações e processar lotes. 
Formatações e organização do documento final.
- Pedro Luiz :
  -> responsável pelos módulos de rotacionamentoe, recorte e auto-align, Readme e alguns testes.
- Antonny :
  -> responsável pelo desenvolvimento das funções log_performance&baixar_resultados e comparar_imagens e Edição do documento.
- Ian Lucas :
  -> responsável pela análise e desenvolvimento do documento das semanas 1 a 5 e desenvolvimento de algumas funções.

**Projeto Acadêmico:** Disciplina de *Processamento de Imagem com Python*  
**Tema:** Rotação e Redimensionamento de Imagens Digitais  
