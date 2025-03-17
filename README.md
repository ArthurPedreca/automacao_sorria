# README

## Automação de Integração entre RD Station CRM e Umbler Talk

### Descrição Geral:

Este script foi criado utilizando Python e automatiza a integração entre duas plataformas:

- **RD Station CRM** (gerenciamento de leads)
- **Umbler Talk** (plataforma de comunicação via chatbot)

A automação realiza as seguintes funções:

1. Acessa automaticamente ambas as plataformas e realiza login utilizando credenciais pré-definidas.
2. Monitora continuamente a presença de novos leads no RD Station.
3. Ao detectar um novo lead, extrai automaticamente nome e telefone.
4. Transfere o lead para o estágio de contato no RD Station.
5. Insere automaticamente o lead como novo contato no Umbler Talk.
6. Inicia uma automação via chatbot diretamente com o novo contato cadastrado.

---

### Tecnologias Utilizadas:

- Python
- Selenium WebDriver
- PyAutoGUI (para manipulação de interface gráfica)
- Regular Expressions (`re`)

---

### Pré-requisitos:

- Python 3.8 ou superior
- Navegador Google Chrome
- ChromeDriver instalado e configurado no PATH
- Dependências Python:
  ```
  pip install selenium pandas pyautogui
  ```

---

### Configuração Inicial:

Antes de executar o script, garanta os seguintes passos:

1. **Credenciais**:
   - Atualize as variáveis de e-mail e senha para ambas as plataformas com suas próprias credenciais.

2. **ChromeDriver**:
   - Instale o ChromeDriver compatível com a sua versão do Chrome.

---

### Execução:

Execute o script diretamente pelo terminal ou por um IDE:

```bash
python nome_do_seu_script.py
```

---

### Funcionamento Detalhado:

- **Login automático:**
  - O script abre duas abas: uma para o RD Station CRM e outra para o Umbler Talk, realizando login automaticamente.

- **Monitoramento Contínuo:**
  - O script monitora indefinidamente a presença de novos leads no RD Station em intervalos regulares.

- **Manipulação do Mouse:**

  Funções auxiliares com `pyautogui` permitem que o script interaja com elementos específicos na tela baseando-se em porcentagens do tamanho da tela.

- **Formatação de Telefone:**

  Os números de telefone são formatados automaticamente para o padrão:
  ```
  (XX) XXXXX-XXXX
  ```

- **Exceções:**

  O script trata automaticamente exceções, como a tentativa de adicionar um número inválido ou já existente.

---

### Logs e Validações:

O script exibe mensagens no terminal informando sobre o sucesso ou possíveis falhas na execução das tarefas.

---

### Considerações Importantes:

- Não interrompa a execução manualmente, a menos que seja necessário.
- Tenha em conta a privacidade e segurança dos dados ao manipular informações de leads.
- Este script deve ser executado com autorização da empresa detentora das contas envolvidas.

---

### Contato:

Para dúvidas ou manutenção do script, entre em contato com o administrador do projeto:

- **Email:** arthurpedreca@gmail.com

---
