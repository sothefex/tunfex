# 🚀 TUNFEX - Gerenciador de Perfis VPN

![GitHub repo size](https://img.shields.io/github/repo-size/sothefex/tunfex)
![GitHub last commit](https://img.shields.io/github/last-commit/sothefex/tunfex)
![GitHub](https://img.shields.io/github/license/sothefex/tunfex)
![GitHub stars](https://img.shields.io/github/stars/sothefex/tunfex?style=social)

---

## 📌 **Sobre o Projeto**

O **TUNFEX** é um gerenciador de perfis VPN desenvolvido para facilitar a criação, edição e distribuição de configurações SSH/SSL/Proxy de forma segura e organizada.

Os perfis são armazenados em um arquivo `profiles.json` e criptografados com **AES-256-CBC** usando a biblioteca **Fernet** do Python, garantindo que suas credenciais estejam protegidas.

---

## 🔐 **Segurança**

- 🔑 **Chave AES-256** gerada aleatoriamente pelo usuário
- 🔒 Arquivo `profiles.enc` **nunca** armazena dados em texto puro
- 🚫 **Token GitHub** salvo localmente com permissões restritas
- ⚠️ **A chave de criptografia NUNCA deve ser compartilhada**

### Como gerar sua chave:

```bash
# Usando Python (recomendado)
python3 << 'EOF'
from cryptography.fernet import Fernet
chave = Fernet.generate_key()
print(chave.decode())
EOF

# Ou usando OpenSSL
openssl rand -base64 32
