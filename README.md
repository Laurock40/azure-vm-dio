# azure-vm-dio
# 🖥️ Documentação: Criação de Máquina Virtual na Azure

Este projeto documenta o processo de criação e configuração de uma máquina virtual (VM) no portal Microsoft Azure. Serve como material de apoio para estudos, testes e futuras implementações.

---

## 📌 Etapas Realizadas

### 1. Acesso ao Portal Azure

- Acesse o portal: [https://portal.azure.com]

---

### 2. Criação da Máquina Virtual

1. No menu lateral, clique em “Máquinas Virtuais” ou pesquise por “Virtual Machines”.
2. Clique em **“+ Criar” > “Máquina Virtual”**.
3. Preencha os campos obrigatórios:
   - Assinatura e Grupo de Recursos
   - Nome da VM: `myVM`
   - Imagem: `Windows Server 2022 Datacenter: Azure Edition - x64 Gen 2`
   - Conta de administrador: 
     - Usuário: `azureuser`
     - Senha com pelo menos 12 caracteres (atendendo aos requisitos de complexidade)
4. Prossiga clicando em **“Avançar”** até chegar à aba **“Revisar + criar”**.
5. Clique em **“Criar”** e aguarde a implantação da VM.

---

### 3. Configuração de Rede

Durante ou após a criação:

- Verifique se a porta 3389 (Windows/RDP) ou 22 (Linux/SSH) está habilitada.
- Vá em **VM > Rede** e confira as regras de entrada do Grupo de Segurança de Rede (NSG).
- Se necessário, adicione uma nova regra de entrada para liberar a porta necessária.

---

### 4. Conexão à Máquina Virtual

#### 🔹 Para Windows (RDP)

1. Acesse sua VM no portal Azure.
2. Clique em **“Conectar” > “Área de Trabalho Remota”**.
3. Baixe o arquivo `.rdp` e abra no seu computador.
4. Insira as credenciais criadas anteriormente.

#### 🔹 Para Linux (SSH)

1. Clique em **“Conectar”** e copie o comando SSH (ex: `ssh azureuser@<IP-da-VM>`).
2. Execute o comando no terminal usando sua chave privada.

---

### 5. Testes e Validações

Após o acesso à VM:

- Verifique se a VM está ativa no painel.
- Teste a conectividade (ex: ping, navegador ou terminal).
- Realize ações básicas no sistema:
  - Atualização do sistema
  - Instalação de pacotes
  - Verificação de conectividade com a internet
- Acompanhe o uso de recursos em **"Métricas"** da VM (CPU, RAM, Disco).

---

## 📷 Capturas de Tela

As imagens estão disponíveis na pasta `/images`.

---

## 👤 Autor

Lauriana Resende Santos

