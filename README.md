# 📱 Análise e Previsão de Preços de Dispositivos Móveis

## 🎯 Objetivo
Analisar fatores que influenciam o preço de dispositivos móveis e desenvolver um modelo preditivo para estimar valores com base em suas características.

## 🛠️ Pré-processamento e Manipulação dos Dados

### Verificando valores nulos
![Verificação de nulo](images/verificacaodenulo.png)

## 📊 Análise Exploratória (EDA)



### Correlação entre Features
![Análise de Correlação](images/correlacao.png)
*Bateria e qualidade da câmera mostraram alta correlação com preço*

### Principais Insights
- Dispositivos com bateria > 4500mAh têm 3x mais chance de ser premium
- Qualidade da câmera (MP) correlaciona 0.65 com preço final
- 70% dos produtos premium têm menos de 2 anos de lançamento

## 🤖 Modelagem Preditiva

### Resultados dos Modelos
![Comparação de Modelos](images/resultados_modelos.png)

| Modelo | R² | MSE |
|--------|----|-----|
| **Random Forest** | **0.88** | **20.824** |
| XGBoost | 0.87 | 20.965 |
| Regressão Linear | 0.38 | 105.553 |

### Feature Importance
![Feature Importance](images/feature_importance.png)
*As features mais importantes para o modelo Random Forest*

## 🛠️ Tecnologias Utilizadas
- Python 3.x
- Pandas, NumPy
- Scikit-learn
- Matplotlib, Seaborn
- Jupyter Notebook

## 🚀 Como Executar
```bash
git clone https://github.com/seu-usuario/projeto-analise-dispositivos
cd projeto-analise-dispositivos
jupyter notebook analise_dispositivos.ipynb
