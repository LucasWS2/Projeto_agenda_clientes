# 🧾 Gerenciador de Clientes - Documentação para Iniciantes

Bem-vindo ao **Gerenciador de Clientes**, uma aplicação simples em Python que ajuda a gerenciar informações de clientes (como nome, sobrenome, email e CPF) usando um banco de dados SQLite.  

Este projeto foi desenvolvido para alunos que estão começando a aprender **Python**, **SQL** e **SQLite**, com uma interface gráfica feita com **Tkinter**.  

📌 **Objetivo**: Entender como criar uma aplicação com interface, conectar com banco de dados e realizar operações como adicionar, visualizar, buscar, atualizar e deletar registros.

---

## 📚 O que faz esta aplicação?

A aplicação permite:

- ➕ **Adicionar** novos clientes ao banco de dados  
- 👁️ **Visualizar** todos os clientes em uma tabela  
- 🔍 **Buscar** clientes por nome, sobrenome, email ou CPF  
- 📝 **Atualizar** os dados de um cliente existente  
- 🗑️ **Deletar** clientes do banco de dados  

🖥️ A interface gráfica é fácil de usar, com campos para inserir dados e botões para executar ações.  
📂 Os dados são armazenados no arquivo `clientes.db`.

---

## 🗂️ Estrutura do Projeto

O projeto é dividido em três arquivos Python:

1. **`Gui.py`**  
   🎨 Interface gráfica com Tkinter  
   🔘 Campos de texto, botões e tabela (Treeview)  
   🔁 Conecta-se ao backend para operações no banco

2. **`Backend.py`**  
   🛠️ Classe com as operações no banco de dados  
   💾 Inserir, visualizar, buscar, atualizar, deletar  
   🔐 Uso de SQL seguro (parametrizado)

3. **`application.py`**  
   🚀 Arquivo principal  
   🔄 Inicia o banco de dados e a janela gráfica

---

## ⚙️ Pré-requisitos

Para executar este projeto, você precisa de:

- 🐍 **Python 3.x** (ex: Python 3.8 ou superior) → [python.org](https://www.python.org/downloads/)  
- 🧰 **Tkinter** (vem com o Python)  
- 🗃️ **SQLite** (incluso via `sqlite3`)  
- 📦 **PyInstaller** *(opcional)* → criar executável

---

## 🧪 Como Configurar e Executar

1. 📁 **Crie uma pasta para o projeto**  
   Ex: `gerenciador_clientes` com os 3 arquivos Python  

2. 🔎 **Verifique o Python instalado**  
   ```bash
   python --version
   ```

3. ▶️ **Execute a aplicação**  
   ```bash
   cd caminho/para/gerenciador_clientes  
   python application.py
   ```

---

## 🖱️ Como Usar a Aplicação

Ao rodar `application.py`, você verá:

- 🧾 **Campos de entrada**: Nome, Sobrenome, Email e CPF  
- 🔘 **Botões**:  
  - ➕ Adicionar  
  - 🔄 Atualizar  
  - ❌ Deletar  
  - 🔍 Buscar  
  - 🧹 Limpar  
- 📋 **Tabela**: Exibe todos os clientes

---

### ✅ Passo a passo:

1. **Adicionar um cliente**  
   Preencha os campos → clique em "Adicionar" ✅

2. **Visualizar clientes**  
   A tabela carrega automaticamente 🗂️

3. **Buscar clientes**  
   Preencha qualquer campo → clique "Buscar" 🔎

4. **Atualizar cliente**  
   Selecione → edite campos → clique "Atualizar" ✏️

5. **Deletar cliente**  
   Selecione → clique "Deletar" 🗑️

---

## 💻 Criando um Executável com PyInstaller

Para rodar a aplicação sem abrir o terminal:

1. 📥 **Instale o PyInstaller**
   ```bash
   pip install pyinstaller
   ```

2. ⚙️ **Crie o executável**
   ```bash
   pyinstaller --onefile --noconsole application.py
   ```

3. 📁 O executável estará em `dist/`  
   → Clique para abrir normalmente 🖱️

4. 💡 **Dica**:  
   Compartilhe o `.exe` com o arquivo `clientes.db` se quiser enviar com os dados.

---

## 🧱 Estrutura do Banco de Dados

Banco: `clientes.db`  
Tabela: `clientes`

Campos:
- 🆔 **id** (único e automático)  
- 👤 **nome**  
- 👥 **sobrenome**  
- 📧 **email**  
- 🧾 **cpf**

---

## 🛠️ Dicas para Solução de Problemas

- ❌ **"No module named tkinter"**  
  → Reinstale o Python ou:  
    ```bash
    pip install tk
    ```

- ❌ **Erro ao executar**  
  → Verifique se os arquivos estão na mesma pasta

- ❌ **Executável não abre**  
  → Execute pelo terminal e veja o erro

- ❌ **Tabela não atualiza**  
  → Certifique-se de que `clientes.db` está na pasta certa

---

## 🎓 O que você pode aprender com este projeto?

- 🐍 **Python**: Classes, módulos, métodos  
- 🧠 **SQL/SQLite**: Consultas seguras  
- 🖼️ **Tkinter**: Campos, botões, tabelas  
- 📐 **Boas práticas**: Código modular e seguro  
- 🧰 **PyInstaller**: Empacotamento de aplicações

---

## 🚀 Próximos Passos

Desafios:

- ✅ Validação de CPF  
- 📤 Exportar dados para CSV  
- 🔁 Botão de recarregar clientes  
- 🎨 Melhorar a interface com ícones e cores

🧑‍🏫 Dúvidas? Pergunte ao instrutor!

---

## ✍️ Autor

**Lucas Agostinho Wszoek** 🚀
