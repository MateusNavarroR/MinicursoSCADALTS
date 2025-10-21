# Simulador Modbus — Executável para Windows e Linux

Este projeto é um **simulador Modbus local**, desenvolvido em **Python**, compatível com **Windows** e **Linux (Ubuntu 24.04 LTS ou superior)**.  
A aplicação cria um servidor Modbus e oferece uma interface web acessível via navegador.

---

## 🚀 Requisitos

### 🪟 Windows
- Nenhum requisito adicional.  
  O executável já contém todas as dependências necessárias.

### 🐧 Linux
- Requer **Ubuntu 24.04 LTS** ou versões compatíveis que possuam:
  - `GLIBC_2.38` ou superior

> ⚠️ Outras distribuições podem não ser compatíveis devido à versão da biblioteca `glibc`.

---

## ⚙️ Execução

### 🪟 **No Windows**

1. Baixe o arquivo executável (`.exe`) do simulador.
2. Dê um duplo clique para executá-lo **ou** abra pelo terminal:
   ```bash
   ./SimuladorModbus.exe
   ```
3. O terminal será aberto e solicitará que você escolha a **porta Modbus** que deseja criar.
4. Após selecionar a porta, a aplicação iniciará automaticamente.
5. Acesse o simulador em seu navegador:
   ```
   http://localhost:5000
   ```

---

### 🐧 **No Linux (Ubuntu 24.04 LTS)**

1. Baixe o arquivo executável para Linux (`SimuladorModbus`).
2. Dê permissão de execução ao arquivo:
   ```bash
   chmod +x SimuladorModbus
   ```
3. Execute o simulador:
   ```bash
   ./SimuladorModbus
   ```
4. Escolha a **porta Modbus** quando solicitado.
5. Assim que o servidor iniciar, acesse no navegador:
   ```
   http://localhost:5000
   ```

---

## 🌐 Funcionamento

- O simulador roda **localmente** na máquina, sem necessidade de conexão externa.
- A interface web pode ser acessada diretamente pelo navegador.
- A comunicação Modbus ocorre na porta configurada no início da execução.

---

## 🧩 Observações

- Caso a porta escolhida já esteja em uso, o programa exibirá uma mensagem de erro e poderá fechar pela permissão do usuário, processo que estão usando essa porta. **ATENÇÃO: Cuidado ao escolher portas proprietarias do sistema, assuma valores seguidos na aula, como 1502 no Linux e 502 no Windows**

---

## 🧱 Tecnologias utilizadas

- **Python 3**
- **Flask** (para interface web)
- **pymodbus** (para simulação Modbus)
- **Threading** (para execução paralela do servidor)

---
