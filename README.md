 
### 🎯 Objetivo do Sistema

O sistema tem como objetivo realizar o **cadastro de usuários**. No início, a funcionalidade estava comprometida por uma **falha de conexão com o banco de dados**, o que impedia o cadastro correto.

---

### ⚫ Teste de Caixa Preta

Foca na **funcionalidade do sistema**, sem acesso ou conhecimento do código-fonte. Testa-se o sistema como um "usuário final".

**Cenários testados:**

- ✅ Cadastro de usuário via **Postman**
- ✅ Verificação se o usuário foi persistido com sucesso no banco de dados usando **HeidiSQL**
- ✅ Autenticação do usuário com **senha criptografada**

**Ferramentas utilizadas:**
- `Postman`
- `HeidiSQL`
- `Intellij`


---

### ⚪ Teste de Caixa Branca

Foca na **estrutura interna do código**.

**Alterações feitas no código:**

- 🛠️ Correção na configuração de `application.properties` para resolver problemas de conexão com o banco de dados
- ✅ Implementação e habilitação do **Lombok** para evitar boilerplate (getters, setters, construtores etc.)

**Arquivos relevantes:**
- `application.properties`
- Classes da entidade `User` e configurações do banco


