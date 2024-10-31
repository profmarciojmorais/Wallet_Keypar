# Wallet_Keypar
Geração de chaves usando o SDKStellar para python

from stellar_sdk import Keypair

keypair = Keypair.random()


secret_key = keypair.secret
public_key = keypair.public_key

print("A nova carteira foi criada!")
print("Chave Privada:", secret_key)
print("Chave publica:", public_key)

---

### Descrição do Código

Este código usa o Stellar SDK em Python para **criar um novo par de chaves** (privada e pública) para uma conta na rede Stellar.

### Funcionamento do Código

1. **Importação do Módulo Stellar SDK**: Importa o módulo `Keypair` da biblioteca `stellar_sdk`, que oferece as funcionalidades necessárias para gerar chaves de contas na Stellar.
  
2. **Geração Aleatória do Par de Chaves**:
   - `keypair = Keypair.random()`: Gera um par de chaves aleatório. Esse par é único e consiste em uma **chave privada** (secret key) e uma **chave pública** (public key).
   - `secret_key = keypair.secret`: Extrai a chave privada (secret key) do par gerado. A chave privada é usada para assinar transações e, portanto, deve ser mantida em segurança.
   - `public_key = keypair.public_key`: Extrai a chave pública (public key) do par gerado. Essa chave é compartilhável e identifica a conta na rede Stellar.

3. **Exibição das Chaves**:
   - `print("Chave Privada:", secret_key)`: Exibe a chave privada (para propósitos educacionais ou de teste; em produção, evite expor a chave privada).
   - `print("Chave Publica:", public_key)`: Exibe a chave pública associada.

### Importante
Esse código é útil para **criar uma nova carteira Stellar** e recuperar suas chaves, que serão necessárias para realizar transações e outras operações na rede Stellar. Contudo, a chave privada deve ser protegida e não compartilhada, pois é essencial para garantir a segurança da conta. 

--- 
Essa descrição dá um contexto claro para usuários e desenvolvedores sobre o propósito e a funcionalidade do código.

### Code Description

This code uses the Stellar SDK in Python to **create a new key pair** (private and public) for an account on the Stellar network.

### Code Functionality

1. **Importing the Stellar SDK Module**: Imports the `Keypair` module from the `stellar_sdk` library, which provides the necessary functionality to generate account keys on the Stellar network.

2. **Random Key Pair Generation**:
   - `keypair = Keypair.random()`: Generates a random key pair. This unique pair consists of a **private key** (secret key) and a **public key**.
   - `secret_key = keypair.secret`: Extracts the private key (secret key) from the generated pair. The private key is used to sign transactions and should be kept secure.
   - `public_key = keypair.public_key`: Extracts the public key from the generated pair. The public key is shareable and identifies the account on the Stellar network.

3. **Displaying the Keys**:
   - `print("Chave Privada:", secret_key)`: Displays the private key (for educational or testing purposes; in production, avoid exposing the private key).
   - `print("Chave Publica:", public_key)`: Displays the associated public key.

### Important
This code is useful for **creating a new Stellar wallet** and retrieving its keys, which are required for conducting transactions and other operations on the Stellar network. However, the private key should be protected and not shared, as it is essential for securing the account.

---

This description provides clear context for users and developers about the purpose and functionality of the code.
