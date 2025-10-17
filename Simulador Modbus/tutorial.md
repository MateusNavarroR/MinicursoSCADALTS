# Tutorial: Utilizando o ModSim64 como Simulador MODBUS

O **ModSim64** é um software gratuito que simula dispositivos escravos MODBUS (RTU e TCP).  
Ele é bastante útil para **testar comunicação** com supervisórios, como o **SCADA-LTS**, sem precisar de um CLP físico.

Neste tutorial, você aprenderá a **instalar, configurar e utilizar** o ModSim64 para testes de comunicação.

---

## 📥 1. Download e Instalação

1. Vá para a pasta Simulador Modbus presente no repositório (lembre de baixar a pasta toda do repositório para ter acesso aos arquivos)
2. Inicie o arquivo **ModBus64.exe**

> ⚠️ Não é necessário instalação — o programa é **portátil**.

![](/home/mateus/Documents/GitHub/MinicursoSCADALTS/Simulador Modbus/Images/Tutorial00.png)

---

## ⚙️ 2. Configuração Inicial

Ao abrir o ModSim64, você verá alguns avisos que o programa irá mostrar, apenas clique nos avisos e você terá a seguinte tela:

![](/home/mateus/Documents/GitHub/MinicursoSCADALTS/Simulador Modbus/Images/Tutorial01.png)



## 🔢 3. Configurando o Servidor TCP/IP e criando a conexão

1. Na aba **Connection**, selecione a aba **Connect** e por fim **Modbus/TCP Serv**
2. Configure a **porta** (padrão Modbus TCP: `502`).

![](/home/mateus/Documents/GitHub/MinicursoSCADALTS/Simulador Modbus/Images/Tutorial02.png)

3. Para criar uma conexão, clique em **File** -> **New** e será aberto uma janela com acesso aos registradores e as memórias do MODBUS

   > ⚠️ Como o aplicativo é a versão gratuita, a conexão dura alguns minutos, para reconectar, feche a janela e abra novamente.

---

## 📊 4. Inserindo Valores nos Registradores

1. Para modificar uma memória, selecione o seu tipo (Coil, Holding Register, Input Status, Input Register) e selecione qual endereço atualizar, modifique o valor e selecione a opção **Update**.

   ![](/home/mateus/Documents/GitHub/MinicursoSCADALTS/Simulador Modbus/Images/Tutorial03.png)