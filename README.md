# 🌊 Ferramenta SNISB vs SIOUT-RS
## Transformando Dados em Decisões - Da Planilha ao Dashboard Empresarial

> **Solução web que substituiu planilhas complexas por um dashboard inteligente, facilitando análise de 10+ mil barragens com filtros, mapa interativo e export em múltiplos formatos.**

[![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://sioutrs.streamlit.app/)
[![Python 3.11+](https://img.shields.io/badge/python-3.11+-blue.svg)](https://www.python.org/downloads/)
[![Agência Zetta](https://img.shields.io/badge/Agencia-Zetta-green.svg)](https://agenciazetta.ufla.br/)

## 🚀 Acesso Rápido

**Veja em ação:** https://sioutrs.streamlit.app/

**Desenvolvedor:** Denner Caleare | [GitHub](https://github.com/DennerCaleare) | [LinkedIn](https://linkedin.com/in/dennercaleare)

---

## 📚 O Problema Que Resolvi

Agência Zetta trabalhava com **10.129 registros de barragens em planilhas Excel**, resultando em:
- 💪 Dificuldade em navegar dados complexos
- 🌈 Impossibilidade de visualizar padrões geográficos
- 📒 Filtros manuais lentos e propensos a erros
- 🚫 Falta de interatividade para tomadas de decisão

## ✨ A Solução Que Entreguei

**Dashboard web interativo** com:

### 📊 Visualização Inteligente
- 💫 Tabelas paginadas e coloridas por compatibilidade
- 🗺️ Mapa interativo mostrando localização de cada barragem
- 🎯 Sistema de cores por nível de risco (verde/amarelo/vermelho)
- 📊 8+ gráficos de análise dinâmicos

### 🔍 Filtros Avançados
- 📅 Por período de cadastro
- 🔖 Código SNISB com autocompletar
- 🍰 Por finalidade de uso (Irrigação, Dessedentação, etc)
- 👥 Por empreendedor/proprietário
- 📚 Por número de autorização

### 📥 Export Profissional
- 📋 Excel (.xlsx)
- 📄 CSV (.csv)
- 📚 JSON (.json)

## 📙 Impacto Entregue

✅ **Facilidade de acesso** - Equipe da Agência agora consulta dados em segundos
✅ **Análise geográfica** - Mapa permite ver padrões regionais instantaneamente
✅ **Tomada de decisão** - Cores e filtros destacam inconsistências cadastrais
✅ **Documentos dinâmicos** - Export em tempo real de dados filtrados

## 🛠️ Stack Técnico

```python
Streamlit 1.32+         # Framework web responsivo
Pandas 2.0+            # Processamento de dados
Folium 0.14+           # Mapas interativos
Plotly                 # Gráficos avançados
GeoPandas 0.14+        # Análise geoespacial
Shapely 2.0+           # Geometrias espaciais
Python 3.11+           # Linguagem
```

## 📂 Estrutura do Projeto

```
streamlit-siout/
├── app.py                          # Aplicação principal
├── requirements.txt               # Dependências
├── README.md                      # Este arquivo
├── RELATORIO_FINAL_SNISB_SIOUT.csv # Dataset principal
├── RELATORIO_FINAL_SNISB_SIOUT.xlsx # Dataset alternativo
└── image/app/
    ├── Logo.png                     # Favicon
    └── LogoZetta.png                # Logo Agência
```

## 🚀 Como Usar

### Acessar Online
```
Acesse: https://sioutrs.streamlit.app/
```

### Rodar Localmente
```bash
git clone https://github.com/DennerCaleare/streamlit-siout.git
cd streamlit-siout
pip install -r requirements.txt
streamlit run app.py
```

## 📊 Funcionalidades Detalhadas

### 🗺️ Mapa Interativo
- Visualização geoespacial com satélite Esri
- Marcadores coloridos por compatibilidade
- Popups com dados detalhados
- Polígonos ANA sobrepostos
- Legenda fixa interativa

### 💫 Tabela Inteligente
- Paginação de 50 registros
- Código de cores por status
- Contador dinâmico
- Busca e filtros combinados

### 📚 Glossário Completo
- Critérios de elegibilidade
- Descrição de 23 colunas
- Dicionário de situações
- FAQ detalhado

## 📊 Dados Principais

| Métrica | Valor |
|---------|-------|
| Total de registros | 10.129 barragens |
| Com polígonos ANA | 9.642 (95,2%) |
| Colunas de dados | 23 campos |
| Formato preferido | CSV |
| Sistema de coordenadas | SIRGAS 2000 |

## 👨‍💻 Desenvolvido por

**Denner Caleare**

- 🌟 Desenvolvedor Full Stack em Streamlit
- 📚 Especialista em dashboards de dados
- 💼 Agência Zetta - UFLA

**Contato:**
- [GitHub](https://github.com/DennerCaleare)
- [LinkedIn](https://linkedin.com/in/dennercaleare)

## 📝 Licença

Desenvolvido para uso institucional. Agência Zetta, UFLA.

---

**Desenvolvido com ❤️ em Lavras, MG**
