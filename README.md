# ⚙️ Configuração de Recursos e Dimensionamento de Máquinas Virtuais no Microsoft Azure

Este repositório apresenta um guia passo a passo para configurar recursos e dimensionar máquinas virtuais (VMs) na plataforma **Microsoft Azure** de forma eficiente.

---

## 🎯 Objetivo

- Entender como ajustar recursos das VMs no Azure (CPU, memória, disco).
- Aprender a escalar verticalmente (scale up) e horizontalmente (scale out) as VMs.
- Conhecer boas práticas para dimensionamento conforme necessidades do sistema.

---

## 🧰 Pré-requisitos

- Conta ativa no [Microsoft Azure](https://portal.azure.com)
- Permissão para criar e modificar máquinas virtuais
- Conhecimentos básicos em computação em nuvem e VMs

---

## 🚀 Passos para Configurar Recursos da VM

### 1. Acessar a VM no Portal Azure

1. No portal Azure, acesse **Máquinas Virtuais** no menu lateral.
2. Selecione a VM desejada.

### 2. Ajustar o Tamanho da VM (Scale Up)

- No painel da VM, clique em **"Tamanho"**.
- Escolha um novo tamanho que atenda melhor às suas necessidades (mais CPU, memória, disco).
- Clique em **"Redimensionar"**.
- A VM será reiniciada para aplicar as mudanças.

---

### 3. Configurar Discos da VM

- No menu da VM, clique em **"Discos"**.
- Adicione ou remova discos gerenciados conforme necessidade.
- Escolha tipos de discos: HDD padrão, SSD Premium ou Ultra Disk.
- Salve as alterações.

---

### 4. Ajustar Configurações de Rede e Segurança (Opcional)

- Configure regras de firewall e grupos de segurança de rede (NSG).
- Configure balanceadores de carga se necessário para distribuir o tráfego.

---

## 🔄 Escalabilidade

### Escala Vertical (Scale Up)

- Aumentar recursos (CPU, RAM, armazenamento) mudando o tamanho da VM.

### Escala Horizontal (Scale Out)

- Criar múltiplas instâncias da VM e distribuir carga entre elas.
- Usar **Conjuntos de Escala de Máquinas Virtuais (Virtual Machine Scale Sets)** para automatizar esse processo.

---

## 🛡️ Boas Práticas

- Monitore uso de CPU, memória e disco com Azure Monitor antes de redimensionar.
- Escolha o tamanho da VM conforme carga real do aplicativo.
- Use Scale Sets para alta disponibilidade e escalabilidade automática.
- Evite mudanças constantes para não impactar a estabilidade do ambiente.

---

## 📚 Links Úteis

- [Redimensionar uma máquina virtual do Azure](https://learn.microsoft.com/azure/virtual-machines/windows/resize-vm)
- [Gerenciar discos em máquinas virtuais do Azure](https://learn.microsoft.com/azure/virtual-machines/windows/manage-disks)
- [Virtual Machine Scale Sets](https://learn.microsoft.com/azure/virtual-machine-scale-sets/)
