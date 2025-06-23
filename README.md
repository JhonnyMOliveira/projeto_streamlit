# 📒 Sistema de Cadastro de Clientes com Streamlit

Este é um projeto simples de sistema de cadastro de clientes desenvolvido em **Python** com **Streamlit**, utilizando armazenamento local em CSV.

---

## 🚀 Funcionalidades

- ✅ **Cadastro de novos clientes**, com os seguintes campos:
  - Nome
  - Data de nascimento
  - Tipo de cliente (Pessoa Física ou Jurídica)

- ✅ **Consulta dos clientes cadastrados**, exibindo os dados em uma tabela interativa.

- ✅ **Persistência de dados** em um arquivo CSV local (`clientes.csv`).

---

## 🗂️ Estrutura de Pastas

```
PROJETO_STREAMLIT/
├── Cadastro.py          # Página principal (Cadastro de Clientes)
├── clientes.csv         # Base de dados local (gerada após o primeiro cadastro)
├── pages/
│   └── Consulta.py      # Página de consulta dos clientes cadastrados
├── .venv/               # Ambiente virtual (se estiver usando)
├── pyproject.toml       # Configuração de dependências (se usar Poetry)
└── README.md            # Documentação do projeto
```

---

## ▶️ Como Executar o Projeto

### 1. Criar o ambiente virtual (opcional, mas recomendado):

Se estiver usando **Poetry**:

```bash
poetry install
poetry shell
```

Ou com o ambiente padrão do Python:

```bash
python -m venv .venv
# Ative o ambiente:
# No Windows:
.venv\Scripts\activate

# No Linux/Mac:
source .venv/bin/activate
```

---

### 2. Instalar as dependências necessárias:

```bash
pip install streamlit pandas
```

---

### 3. Executar a aplicação:

```bash
streamlit run Cadastro.py
```

---

## 🖥️ Navegação entre as páginas

- **Página principal:** `Cadastro.py`
- **Outras páginas:** Dentro da pasta `/pages`, o Streamlit reconhece automaticamente as páginas adicionais (exemplo: `Consulta.py`).

👉 Ao executar o app, a **sidebar do Streamlit** irá exibir um menu de navegação entre as páginas.

---

## 📂 Sobre o arquivo `clientes.csv`

- O arquivo é criado automaticamente após o primeiro cadastro.
- Os dados são salvos no seguinte formato:

```
nome, data_nascimento, tipo_cliente
```

- A página de **Consulta** lê e exibe os dados dessa base.

---

## 👨‍💻 Desenvolvido por:

**Jhonny Marcelo de Oliveira**  
Especialista em Redes | Python para Dados | Streamlit | Transformação Digital
