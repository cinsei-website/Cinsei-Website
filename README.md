# 🌐 CINSEI Website

Website oficial da CINSEI - Consultoria em Investimento e Serviços, E.I.

![CINSEI Logo](cinsei_logo.png)

## 📋 Descrição

Website institucional com formulário de solicitação de serviços, suporte multilíngue (Português, Inglês e Chinês) e integração com email e WhatsApp.

## 🚀 Funcionalidades

- ✅ **Três idiomas**: PT 🇵🇹 | EN 🇬🇧 | 中文 🇨🇳
- ✅ **Formulário de serviços** com seleção múltipla
- ✅ **Envio para múltiplos emails**:
  - cinseiconsultorias25@gmail.com
  - zenhani.consultantadt@gmail.com
- ✅ **Integração WhatsApp** direta
- ✅ **Design responsivo** (mobile-first)
- ✅ **Animações suaves** e interface moderna

## 📁 Estrutura de Ficheiros

```
/
├── index.html              # Página principal
├── solicitar-servicos.html # Formulário de serviços
├── obrigado.html          # Página de agradecimento
├── cinsei_logo.png        # Logotipo principal
├── cinsei_favicon.png     # Favicon
└── README.md              # Este ficheiro
```

## 🔧 Configuração do Formulário

O formulário utiliza o **FormSubmit.co** para envio de emails. Configurações atuais:

```html
<input type="hidden" name="_cc" value="zenhani.consultantadt@gmail.com">
<input type="hidden" name="_subject" value="Nova Solicitação de Serviços - CINSEI">
<input type="hidden" name="_template" value="table">
<input type="hidden" name="_next" value="https://cinsei.co.mz/obrigado.html">
```

### Para alterar os emails de destino:

1. Abra `solicitar-servicos.html`
2. Localize a linha: `action="https://formsubmit.co/cinseiconsultorias25@gmail.com"`
3. Altere para o email principal desejado
4. Na linha `_cc`, adicione emails em cópia separados por vírgula

## 📱 WhatsApp Integration

Botão flutuante de WhatsApp configurado para:
- **Número**: +258 82 774 3075
- **Mensagem pré-preenchida**: "Olá! Gostaria de solicitar informações sobre os serviços da CINSEI."

Para alterar:
```javascript
// Em solicitar-servicos.html, linha do WhatsApp float
href="https://wa.me/258827743075?text=SUA_MENSAGEM"
```

## 🌐 Publicação no GitHub Pages

1. Crie um novo repositório no GitHub
2. Faça upload de todos os ficheiros
3. Vá em **Settings** → **Pages**
4. Em "Source", selecione "Deploy from a branch"
5. Selecione a branch `main` e pasta `/ (root)`
6. Clique em **Save**
7. O site estará disponível em: `https://seuusername.github.io/nomedorepositorio/`

## 🎨 Personalização

### Cores principais (CSS Variables)
```css
--primary: #1e3a5f;      /* Azul escuro */
--accent: #d69e2e;       /* Dourado */
--success: #48bb78;      /* Verde sucesso */
```

### Serviços disponíveis
Para adicionar/remover serviços no formulário, edite a secção `.services-grid` em `solicitar-servicos.html`.

## 📞 Contactos

- **Email 1**: cinseiconsultorias25@gmail.com
- **Email 2**: zenhani.consultantadt@gmail.com
- **WhatsApp**: +258 82 774 3075
- **Localização**: Maputo, Moçambique

## 📝 Notas

- O formulário permite selecionar **múltiplos serviços** simultaneamente
- O utilizador pode escolher a **preferência de contacto** (Email, WhatsApp ou Telefone)
- Todos os campos marcados com * são obrigatórios
- A página de agradecimento redireciona automaticamente após 10 segundos

## 🔒 Privacidade

Os dados submetidos através do formulário são enviados diretamente para os emails configurados via FormSubmit.co. Não são armazenados em servidores externos.

---

**CINSEI** © 2024 - Consultoria em Investimento e Serviços, E.I.
