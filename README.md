# 🏠 Cadastro de Endereço

Projeto desenvolvido como atividade prática para criação de um pequeno formulário de cadastro de endereço utilizando **HTML5**, **CSS3**, **JavaScript** e o framework **Bootstrap**.  
O sistema consome a **API ViaCEP** para preencher automaticamente os campos de endereço a partir do **CEP** informado.

---

## 🚀 Objetivo

Criar uma aplicação web simples que:
- Permita o cadastro de um endereço completo;
- Consulte a API [ViaCEP](https://viacep.com.br/) a partir do CEP informado;
- Preencha automaticamente os campos **Rua**, **Bairro**, **Cidade** e **Estado**;
- Utilize **Bootstrap** para estilização e responsividade.

---

## 🧱 Estrutura do Projeto

```
cadastroEndereco/
│
├── index.html              # Página principal com o formulário
├── css/
│   └── style.css           # Estilos personalizados
└── js/
    └── controller.js       # Lógica e integração com a API ViaCEP
```

---

## 🖥️ Tecnologias Utilizadas

- **HTML5** – estrutura da página  
- **CSS3** – estilização e layout  
- **JavaScript (ES6+)** – lógica de busca e preenchimento automático  
- **Bootstrap 5.3** – framework de design responsivo  
- **API ViaCEP** – consulta de informações de endereço via CEP  

---

## ⚙️ Como Executar

1. **Baixe o projeto**  
   ```bash
   git clone https://github.com/seu-repositorio/cadastroEndereco.git
   ```
   ou extraia o arquivo `.zip` fornecido.

2. **Abra o arquivo `index.html`** diretamente no navegador (recomendado: Google Chrome).

3. **Digite um CEP válido** (exemplo: `01001000`) e pressione **Tab** ou clique fora do campo.  
   Os campos de **Rua**, **Bairro**, **Cidade** e **Estado** serão preenchidos automaticamente.

---

## 🧩 Funcionalidades

✅ Busca automática de endereço pelo CEP  
✅ Validação básica do campo CEP  
✅ Campos de leitura automática bloqueados (readonly)  
✅ Layout responsivo e agradável usando Bootstrap  
✅ Campos opcionais: **Número** e **Complemento**

---

## 🧠 Lógica de Funcionamento

O script `controller.js` adiciona um *event listener* ao campo **CEP**.  
Quando o usuário sai do campo, o sistema:

1. Remove caracteres não numéricos do CEP;  
2. Faz uma requisição `fetch` para `https://viacep.com.br/ws/{cep}/json/`;  
3. Preenche os campos com as informações retornadas pela API;  
4. Exibe alertas em caso de erro ou CEP inexistente.

---

## 🧾 Requisitos

- **Navegador moderno** (Google Chrome, Edge, Firefox, etc.)  
- (Opcional) **Extensão NetBeans Connector** instalada e ativada no navegador para execução integrada pelo NetBeans IDE.  
- **Java JDK + NetBeans IDE** configurados para ambiente de desenvolvimento (requisito da atividade prática).

---

## 📚 Referências

- [ViaCEP – Webservice gratuito de CEP](https://viacep.com.br/)  
- [Documentação do Bootstrap 5](https://getbootstrap.com/docs/5.3/getting-started/introduction/)

---

## 👨‍💻 Autor

**Nome:** Welder Junio  
**Disciplina:** Desenvolvimento Web  
**Instituição:** Faculdade Anhanguera  
**Data:** Outubro de 2025

---

📦 Projeto desenvolvido para fins didáticos como parte de uma **Aula Prática sobre HTML5, CSS3 e JavaScript**.
