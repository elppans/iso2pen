# iso2pen - Criador de Pendrive Bootável (BIOS + UEFI)

O **iso2pen** é um conjunto de scripts Shell para criar um pendrive bootável a partir de uma ISO do Linux, com suporte para **BIOS (Syslinux)** e **UEFI (GRUB)**.

Existem duas versões disponíveis:
- **iso2pen** → Versão de linha de comando (CLI)
- **iso2pen-gui** → Versão gráfica usando Zenity

---

## 🛠️ Requisitos

Antes de usar, instale as dependências necessárias:

### Debian/Ubuntu:
```bash
sudo apt update
sudo apt install syslinux mtools parted grub-efi-amd64-bin zenity -y
```

### Fedora:
```bash
sudo dnf install syslinux mtools parted grub2-efi-x64 zenity -y
```

### Arch Linux:
```bash
sudo pacman -S syslinux mtools parted grub zenity --noconfirm
```

---

## 🚀 Como Usar

### 🔹 **Modo CLI (linha de comando)**
1. **Dê permissão de execução:**
   ```bash
   chmod +x iso2pen
   ```
2. **Execute o script com o caminho da ISO e o dispositivo do pendrive:**
   ```bash
   sudo ./iso2pen linux.iso /dev/sdX
   ```
   **Substitua `/dev/sdX` pelo seu pendrive** (exemplo: `/dev/sdb`).

---

### 🔹 **Modo GUI (interface gráfica)**
1. **Dê permissão de execução:**
   ```bash
   chmod +x iso2pen-gui
   ```
2. **Execute o script e siga as instruções na tela:**
   ```bash
   sudo ./iso2pen-gui
   ```
   - Escolha a ISO  
   - Selecione o pendrive  
   - Confirme a formatação  
   - Acompanhe a barra de progresso  

---

## ⚠️ Avisos Importantes

- **Todos os dados do pendrive serão apagados!**  
- Certifique-se de selecionar o dispositivo correto antes de continuar.  
- Este script **não verifica a integridade da ISO**, então use uma ISO confiável.  

---

## 📜 Licença
Este projeto é open-source e está licenciado sob a **MIT License**.  

---

## ✨ Créditos
Criado por [Elppans] 🛠️  

