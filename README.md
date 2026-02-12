
---

# 📊 Modelagem Estatística em Indicadores Socioeconômicos

### Análise de Impacto na Expectativa de Vida e Inferência para Tomada de Decisão

Este projeto foi desenvolvido como um estudo de caso real dentro da **Pós-Graduação em Data Science e Inteligência Artificial**, em parceria com a **Data Science Academy (DSA)**. O foco principal é a utilização de **Regressão Linear Múltipla** para entender os pilares da longevidade global.

---

## 🎯 1. Problema de Negócio

Governos e ONGs enfrentam o desafio de alocar orçamentos limitados. Onde investir para salvar mais vidas? Este projeto utiliza modelagem estatística para identificar quais variáveis (Saúde, Educação ou Economia) possuem maior correlação e causalidade estatística com a **Expectativa de Vida**, permitindo recomendações baseadas em evidências.

---

## 🚀 2. Funcionalidades (MVP)

* **Diagnóstico de Saúde Populacional:** Identificação automática de fatores de risco.
* **Filtro de Relevância:** Seleção de variáveis com significância estatística ().
* **Simulador de Impacto:** Modelo capaz de explicar 77% das variações na expectativa de vida.
* **Análise de Estilo de Vida:** Avaliação combinada de nutrição e consumo de álcool.

---

## 🏗️ 3. Arquitetura e Engenharia de Dados

O projeto foi estruturado para garantir a integridade estatística:

* **Tratamento de Dados:** Imputação de valores ausentes e normalização.
* **Engenharia de Recursos (Feature Engineering):** Criação da variável `lifestyle` (combinação de BMI e Álcool) e categorização de países por faixas populacionais para reduzir o viés de escala.
* **Redução de Dimensionalidade:** Filtros baseados em multicolinearidade (Corte de correlação em 0.65).

---

## 🛠️ 4. Recursos de Data Science

* **Bibliotecas:** `Pandas`, `NumPy`, `Seaborn`, `Matplotlib`.
* **Modelagem:** `Statsmodels` (OLS - Ordinary Least Squares) e `Scikit-Learn` (StandardScaler).
* **Controle:** `Watermark` para registro de versões e reprodutibilidade.

---

## 📝 5. Passo a Passo do Projeto

O projeto segue um workflow rigoroso de Ciência de Dados:

### **I. Preparação e Limpeza**

1. **Instalando e Carregando Pacotes:** Configuração do ambiente de trabalho.
2. **Carregando e Compreendendo os Dados:** Primeira inspeção da base histórica.
3. **Ajuste Inicial:** Tradução e padronização de labels.
4. **Análise Exploratória:** Visualização da distribuição dos dados.

### **II. Tratamento Estatístico**

5. **Detecção de Outliers:** Uso da regra do **1.5 IQR**. *Nota: A regra não é rígida; analisamos visualmente a distribuição para ajustar limites e evitar a perda de dados valiosos.*
6. **Tratamento de Valores Ausentes:** Aplicação de técnicas de imputação estatística.
7. **Engenharia de Recursos:** Categorização da população em 3 faixas para mitigar discrepâncias entre países pequenos e gigantes.

### **III. Seleção de Variáveis (Feature Selection)**

8. **Análise de Correlação e Multicolinearidade:**
* **1º Filtro:** Seleção de variáveis com alta correlação com a variável alvo (ex: `adult_mortality`, `hiv`, `school`).
* **2º Filtro (Multicolinearidade):** Eliminação de variáveis preditoras altamente correlacionadas entre si (corte > 0.65) para evitar instabilidade no modelo.
* **3º Filtro (Negócio):** Decisão estratégica de manter `lifestyle` em vez de `bmi`, por ser mais informativa para o tomador de decisão.



### **IV. Modelagem e Diagnóstico**

9. **Construção do Modelo OLS:** Estimação de parâmetros através de Mínimos Quadrados Ordinários.
10. **Validação:** Análise de resíduos e verificação das suposições da regressão linear.

---

## 📊 6. Entrega do Resultado e Insights (Tomada de Decisão)

O modelo final revelou descobertas críticas para políticas públicas:

* **Efetividade:** O modelo explica **77%** da variabilidade da expectativa de vida.
* **Fatores Negativos:** Mortalidade adulta e HIV são os maiores detratores da longevidade.
* **Fatores Positivos:** Educação e estilos de vida saudáveis possuem a maior associação positiva.
* **Saúde Básica:** A vacinação (Difteria) e a nutrição infantil surgiram como pilares fundamentais.

**Recomendação Estratégica:** O investimento deve ser híbrido — focado em prevenção de doenças (vacinas/HIV) e promoção social (educação/nutrição).

---

## 💻 7. Como Executar e Artefatos

1. **Clone:** `git clone https://github.com/seu-usuario/projeto6.git`
2. **Dependências:** `pip install -r requirements.txt` (ou instale as bibliotecas listadas no item 4).
3. **Execução:** Abra o `Projeto6.ipynb` e execute as células sequencialmente.
4. **Artefatos:** O projeto inclui o dataset tratado, o notebook documentado e o relatório de performance do modelo.

---

## 🙏 Agradecimentos e Autoria

Este projeto é um marco na minha trajetória na **Pós-Graduação em Data Science e Inteligência Artificial**. Agradeço à **Data Science Academy (DSA)** por fornecer a base teórica e prática necessária para transformar dados brutos em inteligência de negócio.

**Autor:** [Jefferson Ferreira]<br/>
**Linkedin** [Jefferson Franca Ferreira](https://www.linkedin.com/in/jefferson-ferreira-ds/)<br/>
*Cientista de Dados*

---

*Gostou deste projeto? Deixe uma ⭐ no GitHub!*
