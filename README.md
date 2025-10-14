# 🖼️ Grupo 3 - Rotação e Redimensionamento de Imagens

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


---

## 📈 Aplicações

O módulo de Rotação e Redimensionamento pode ser utilizado em diversas áreas, como:

- Edição e tratamento digital de imagens  
- Sistemas de visão computacional  
- Reconhecimento de padrões  
- Otimização de imagens para web  
- Processos industriais e inspeção automatizada  

---

## 👨‍💻 Equipe — Grupo 3

**Projeto Acadêmico:** Disciplina de *Processamento de Imagem com Python*  
**Tema:** Rotação e Redimensionamento de Imagens Digitais  
