# 🌐 Tunfex VPN - Perfis Remotos

Um jeito simples de gerenciar seus perfis de VPN e compartilhar com a galera.

---

## 🤔 Como funciona?

1. Você cria seus perfis VPN (SSH, Proxy, SSL, etc)
2. Criptografa com sua chave secreta
3. O app do seu celular baixa automaticamente
4. Pronto! Seus perfis sempre atualizados!

---

## 🔒 É seguro?

Sim! O arquivo `profiles.enc` é público mas tá criptografado. Só quem tem a chave consegue ler.

- Ninguém vê suas senhas
- Ninguém vê seus IPs
- Ninguém vê nada!

---

## 🚀 Como usar

### No PC/Servidor:

```bash
# Baixa o script
wget https://raw.githubusercontent.com/sothefex/tunfex/main/vpn_manager.sh
chmod +x vpn_manager.sh
bash vpn_manager.sh
