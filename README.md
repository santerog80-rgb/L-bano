# 🇲🇿 Luvano - Marketplace de Moçambique

Marketplace completo com autenticação, múltiplas moedas, upload de fotos, avaliações e integração WhatsApp.

## 📁 Arquivos do Projeto

### Páginas HTML (com CSS e JavaScript Interno)

1. **index.html** - Página principal do marketplace
   - Exibição de produtos
   - Busca e filtros por categoria
   - Conversão de moedas (MZN, USD, EUR, ZAR, GBP)
   - Sistema de ordenação

2. **cadastro.html** - Página de registro
   - Formulário de criação de conta
   - Validação de senhas
   - Login automático após cadastro

3. **login.html** - Página de login
   - Autenticação de usuários
   - Modo demonstração (cria conta automaticamente)
   - Redirecionamento para painel

4. **painel.html** - Painel do usuário
   - Dashboard com estatísticas
   - Formulário para criar anúncios
   - Upload de até 5 fotos
   - Gerenciamento de produtos

5. **logout.html** - Página de logout
   - Limpeza de sessão
   - Contagem regressiva
   - Redirecionamento automático

## ✨ Funcionalidades Implementadas

### 🔐 Sistema de Autenticação
- ✅ Cadastro de usuários
- ✅ Login com validação
- ✅ Sessão persistente (localStorage)
- ✅ Logout com confirmação

### 💰 Múltiplas Moedas
- ✅ MZN - Metical Moçambicano
- ✅ USD - Dólar Americano
- ✅ EUR - Euro
- ✅ ZAR - Rand Sul-Africano
- ✅ GBP - Libra Esterlina
- ✅ Conversão automática de preços

### 📱 Integração WhatsApp
- ✅ Botão de contacto direto
- ✅ Mensagem pré-formatada
- ✅ Abre WhatsApp do vendedor

### ⭐ Sistema de Avaliações
- ✅ Classificação de 1 a 5 estrelas
- ✅ Exibição de avaliações médias
- ✅ Contador de reviews

### 📸 Upload de Fotos
- ✅ Múltiplas imagens (até 5)
- ✅ Preview antes do upload
- ✅ Armazenamento em Base64
- ✅ Remoção individual de fotos

### 🗂️ Categorias Completas
- 📱 Electrónicos
- 🚗 Veículos
- 🏠 Imóveis
- 👗 Moda
- 🛋️ Casa & Jardim
- ⚽ Desportos
- 🔧 Serviços
- 🌾 Agricultura
- 📚 Livros

### 🔍 Busca e Filtros
- ✅ Busca por texto
- ✅ Filtro por categoria
- ✅ Ordenação (data, preço, avaliação)

### 👤 Painel do Usuário
- ✅ Estatísticas de vendas
- ✅ Total de visualizações
- ✅ Avaliação média
- ✅ Criar novos anúncios

## 🚀 Como Usar

### Instalação

1. **Baixe todos os arquivos HTML**
2. **Coloque na mesma pasta**
3. **Abra `index.html` no navegador**

Pronto! Não precisa de servidor ou configuração adicional.

### Começando

1. **Navegue pelos produtos** na página inicial
2. **Crie uma conta** em cadastro.html
3. **Faça login** em login.html
4. **Acesse o painel** em painel.html
5. **Crie anúncios** com fotos e detalhes

### Modo Demonstração

O sistema inclui:
- 6 produtos de exemplo pré-carregados
- Login simplificado (qualquer email/senha funciona)
- Criação automática de conta no primeiro acesso

## 💾 Armazenamento de Dados

Todos os dados são salvos no **localStorage** do navegador:

- `luvanoUsers` - Lista de usuários cadastrados
- `luvanoUser` - Sessão do usuário atual
- `luvanoProducts` - Lista de produtos publicados

## 🎨 Design

- **Cores de Moçambique**: Vermelho, Verde, Amarelo
- **Tipografia**: Playfair Display + DM Sans
- **Animações**: Transições suaves e micro-interações
- **Responsivo**: Funciona em desktop e mobile

## 📊 Taxas de Câmbio (Exemplo)

```javascript
MZN: 1      (Base)
USD: 0.0157 (1 MZN = $0.0157)
EUR: 0.0145 (1 MZN = €0.0145)
ZAR: 0.29   (1 MZN = R0.29)
GBP: 0.0125 (1 MZN = £0.0125)
```

> **Nota**: Atualize as taxas regularmente no código

## 🔧 Personalização

### Alterar Cores

Edite as variáveis CSS no `<style>` de cada página:

```css
:root {
    --primary-red: #D32F2F;
    --primary-green: #2E7D32;
    --primary-yellow: #F9A825;
}
```

### Alterar Taxas de Câmbio

Edite no script da index.html:

```javascript
const EXCHANGE_RATES = {
    MZN: 1,
    USD: 0.0157,
    EUR: 0.0145,
    ZAR: 0.29,
    GBP: 0.0125
};
```

### Adicionar Categorias

Edite o menu de categorias e o select no formulário em todas as páginas relevantes.

## 🌐 Navegação

```
index.html ──────┐
                 │
cadastro.html ───┼──> painel.html ──> logout.html ──> index.html
                 │
login.html ──────┘
```

## 📱 Recursos Mobile

- Interface totalmente responsiva
- Touch-friendly (botões grandes)
- Menu scroll horizontal em categorias
- Formulários adaptados para mobile

## 🔒 Segurança

⚠️ **IMPORTANTE**: Este é um projeto de demonstração.

Para produção, implemente:
- Hash de senhas (bcrypt)
- Validação server-side
- Sanitização de inputs
- Tokens de sessão seguros
- Backend com banco de dados real

## 🚀 Próximos Passos

Para transformar em aplicação completa:

1. **Backend**: Criar API com Node.js/PHP/Python
2. **Banco de Dados**: Usar Supabase/Firebase/MySQL
3. **Storage**: Cloudinary/AWS S3 para imagens
4. **Pagamentos**: Integrar M-Pesa/PayPal
5. **Chat**: Adicionar mensagens entre usuários
6. **Notificações**: Push notifications
7. **PWA**: Converter para Progressive Web App

## 📄 Licença

Projeto livre para uso educacional e comercial.

## 🤝 Suporte

Para dúvidas:
1. Verifique o código no navegador (F12)
2. Veja o Console para erros
3. Teste em modo de demonstração primeiro

---

**Desenvolvido com ❤️ para Moçambique** 🇲🇿

*Luvano - O marketplace que une todo Moçambique*
