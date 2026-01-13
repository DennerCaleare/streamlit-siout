# 🌊 Ferramenta de Comparação de Registros - SNISB vs SIOUT-RS

> Dashboard inteligente para análise e cruzamento de dados de barragens entre o Sistema Nacional de Informações sobre Segurança de Barragens (SNISB) e o Sistema de Outorgas de Água do Rio Grande do Sul (SIOUT-RS).

[![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://sioutrs.streamlit.app/)
[![Python 3.11+](https://img.shields.io/badge/python-3.11+-blue.svg)](https://www.python.org/downloads/)
[![Agencia Zetta](https://img.shields.io/badge/Developed%20by-Ag%C3%AAncia%20Zetta-green.svg)](https://agenciazetta.ufla.br/)

## 🚀 Acesso Rápido

👉 **[Abrir Dashboard Online](https://sioutrs.streamlit.app/)**

## 📋 Sobre o Projeto

Sistema web inteligente que realiza cruzamento, validação e comparação de dados entre três bases de dados críticas:

- **SNISB**: Cadastro Nacional de Barragens gerenciado pela ANA
- **SIOUT-RS**: Autorizações estaduais de recursos hídricos
- **Polígonos ANA**: Massas d'água oficialmente mapeadas

O objetivo principal é **identificar barragens com inconsistências cadastrais** e garantir conformidade com os requisitos legais de outorga.

## ✨ Funcionalidades

### 📊 Visualização de Dados
- 📋 Tabela paginada com 50 registros por página
- 🎨 Código de cores automático por status de compatibilidade
- 📊 Contador dinâmico de registros filtrados
- 📥 Exportação em Excel, CSV e JSON
- 📱 Interface 100% responsiva

### 🔍 Filtros Avançados
- 📅 Filtro por período de cadastro
- 🔖 Busca por código SNISB com autocompletar
- 🎯 Filtros por finalidade de uso
- 👤 Busca por empreendedor/proprietário
- 📋 Filtro por número de autorização
- 🔗 Lógica combinada AND entre filtros

### 🗺️ Mapa Interativo
- 🗺️ Visualização geoespacial com satélite Esri HD
- 🎛️ Controle de camadas sem recarga da página
- 🎯 Marcadores coloridos por compatibilidade
- 📍 Popups informativos ao clicar nos pontos
- 🎨 Polígonos ANA renderizados com otimização

### 📚 Ajuda e Glossário
- 📖 Critérios de elegibilidade e validação
- 📝 Descrição detalhada de 23 colunas
- 📚 Dicionário de situações e status
- 🎨 Legenda completa de cores
- ❓ FAQ com perguntas frequentes

## 🛠️ Tecnologias

```python
Streamlit 1.32+         # Framework web
Pandas 2.0+            # Análise de dados
Folium 0.14+           # Mapas interativos
shapely 2.0+           # Geometrias espaciais
GeoPandas 0.14+        # Dados geoespaciais
OpenPyXL               # Leitura de Excel
Python 3.11+           # Linguagem
```

## 📦 Instalação

### Localmente

```bash
# 1. Clone o repositório
git clone https://github.com/DennerCaleare/streamlit-siout.git
cd streamlit-siout

# 2. Instale as dependências
pip install -r requirements.txt

# 3. Execute o app
streamlit run app.py

# A aplicação abrirá em http://localhost:8501
```

## 📂 Estrutura do Projeto

```
streamlit-siout/
├── app.py                                  # Aplicação principal
├── requirements.txt                        # Dependências Python
├── README.md                               # Este arquivo
├── RELATORIO_FINAL_SNISB_SIOUT.csv        # Dataset principal
├── RELATORIO_FINAL_SNISB_SIOUT.xlsx       # Dataset alternativo
└── image/
    └── app/
        ├── Logo.png                        # Favicon
        └── LogoZetta.png                   # Logo Agência Zetta
```

## 📊 Dados

| Métrica | Valor |
|---------|-------|
| Total de registros | 10.129 barragens |
| Registros com polígonos ANA | 9.642 (95,2%) |
| Polígonos ANA únicos | ~4.214 massas d'água |
| Colunas | 23 campos |
| Sistema de coordenadas | SIRGAS 2000 (EPSG:4674) |
| Formato preferencial | CSV |

## 🎨 Hierarquia de Cores

| Cor | Status | Significado |
|-----|--------|----------|
| 🟢 | Totalmente Compatível | Todos campos conferem |
| 🟡 | Parcialmente Compatível | Alguns campos diferem |
| 🟠 | Compatível Geograficamente | Mesma localização, dados divergentes |
| 🔴 Escuro | Incompatível | Sem correspondência entre sistemas |
| 🔴 Claro | Descartado | Eliminado por hierarquia |
| 🔵 | Selecionado | Aprovado para validação |

## 👨‍💻 Desenvolvido por

**Denner Caleare** | [GitHub](https://github.com/DennerCaleare) | [LinkedIn](https://linkedin.com/in/dennercaleare)

Em parceria com **Agência Zetta** - Agência de inovação da UFLA

[https://agenciazetta.ufla.br/](https://agenciazetta.ufla.br/)

## 📝 Licença

Este projeto foi desenvolvido para uso institucional e análise de dados públicos de recursos hídricos.

---

**Desenvolvido com ❤️ em Lavras, MG**
