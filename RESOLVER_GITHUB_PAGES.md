# 🔧 Resolver Problemas - GitHub Pages não Funciona

## ✅ Checklist Completo

### **1. Verificar Nome do Arquivo**

❌ **ERRADO:** guardador.html
✅ **CORRETO:** index.html

**O arquivo DEVE se chamar `index.html`** (não guardador.html)

#### Como Corrigir:
1. Vá no seu repositório do GitHub
2. Clique no arquivo `guardador.html`
3. Clique no ícone do lápis (editar)
4. No topo, mude o nome para `index.html`
5. Scroll para baixo
6. Clique "Commit changes"

---

### **2. Verificar GitHub Pages Está Ativo**

1. Vá em **Settings** (Configurações) do repositório
2. No menu lateral, clique em **Pages**
3. Em "Source" (Origem), deve estar:
   - Branch: **main** (ou master)
   - Folder: **/ (root)**
4. Clique **Save** se não estiver configurado

**Aguarde 1-2 minutos** para o site ficar ativo!

---

### **3. Verificar URL Correto**

O link deve ser **exatamente assim**:

```
https://SEU_USUARIO.github.io/NOME_DO_REPOSITORIO/
```

**Exemplos:**
- Se usuário é `joao123` e repositório é `guardador`:
  ```
  https://joao123.github.io/guardador/
  ```

- Se usuário é `maria_silva` e repositório é `meus-links`:
  ```
  https://maria-silva.github.io/meus-links/
  ```

**⚠️ IMPORTANTE:** 
- Use letras minúsculas
- Substitua underscores por hífens se necessário
- Não esqueça a `/` no final

---

### **4. Aguardar Build Completar**

Após fazer upload ou ativar GitHub Pages:

1. Vá em **Actions** (Ações) no topo do repositório
2. Veja se há um processo "pages build and deployment"
3. Aguarde aparecer ✅ verde (pode levar 1-5 minutos)
4. Só depois acesse a URL

---

### **5. Verificar Estrutura do Repositório**

Sua estrutura deve estar assim:

```
seu-repositorio/
└── index.html   ← Arquivo na raiz (não dentro de pasta!)
```

❌ **ERRADO:**
```
seu-repositorio/
└── www/
    └── index.html   ← Não funciona dentro de pasta
```

✅ **CORRETO:**
```
seu-repositorio/
└── index.html   ← Direto na raiz
```

---

## 🚀 Passo a Passo Completo (Do Zero)

### **Método 1: Criar Repositório Novo**

1. **GitHub.com** → Login
2. Clique no **+** (canto superior direito) → **New repository**
3. **Repository name:** `guardador` (ou outro nome)
4. Marque ✅ **Public**
5. **NÃO** marque "Add a README file"
6. Clique **Create repository**

7. Na página que abrir, clique **uploading an existing file**
8. Arraste o arquivo `guardador.html`
9. **ANTES de fazer commit**, mude o nome para `index.html`
10. Clique **Commit changes**

11. Vá em **Settings** → **Pages**
12. Em "Source", escolha **main**
13. Clique **Save**
14. Aguarde 2 minutos

15. Acesse: `https://SEU_USUARIO.github.io/guardador/`

---

### **Método 2: Corrigir Repositório Existente**

Se já criou o repositório mas não funciona:

1. Vá no repositório
2. Verifique se o arquivo se chama `index.html`
   - Se não, renomeie (editar → mudar nome → commit)
3. Vá em **Settings** → **Pages**
4. Verifique se Source está em **main** e **/ (root)**
5. Clique **Save**
6. Aguarde 2 minutos
7. Tente acessar novamente

---

## 🔍 Diagnóstico de Problemas

### **Erro: "404 - Page not found"**

**Causa:** Arquivo não se chama `index.html` ou está em pasta errada

**Solução:**
1. Renomear arquivo para `index.html`
2. Verificar que está na raiz (não em pasta)
3. Aguardar rebuild (1-2 min)

---

### **Erro: Página em branco**

**Causa:** Arquivo HTML pode ter erro ou não carregou

**Solução:**
1. Abra a página
2. Pressione **F12** (DevTools)
3. Vá em **Console**
4. Veja se há erros em vermelho
5. Se houver, copie e me envie

**Ou:**
1. Faça upload novamente do arquivo `guardador.html`
2. Renomeie para `index.html`
3. Commit

---

### **Erro: URL não existe**

**Causa:** GitHub Pages não está ativo ou URL errado

**Solução:**
1. Confirme que GitHub Pages está ativo em Settings → Pages
2. Verifique se a URL está correta:
   - `https://SEU_USUARIO.github.io/NOME_REPO/`
   - Tudo em minúsculas
   - Barra no final

---

## 🎯 Teste Rápido

Faça este teste:

1. Acesse: `https://SEU_USUARIO.github.io/NOME_REPO/index.html`
2. Se funcionar → Problema é que falta `/index.html` explícito
   - Solução: Verificar que arquivo se chama `index.html`
3. Se não funcionar → Problema é mais profundo
   - Continue lendo abaixo

---

## 📋 Informações para Diagnosticar

**Me envie estas informações para eu ajudar:**

1. **Nome do usuário GitHub:** 
2. **Nome do repositório:**
3. **URL que está tentando acessar:**
4. **Nome do arquivo no repositório:**
5. **GitHub Pages está ativo?** (Settings → Pages)
6. **Mensagem de erro que aparece:**

---

## 💡 Dicas Extras

### **Forçar Atualização do Navegador:**

Às vezes o navegador guarda cache antigo:

- **Windows:** Ctrl + F5
- **Mac:** Cmd + Shift + R
- **Chrome:** Ctrl + Shift + Delete → Limpar cache

---

### **Usar Modo Anônimo:**

Abra uma aba anônima e teste a URL:
- **Chrome:** Ctrl + Shift + N
- **Firefox:** Ctrl + Shift + P

Se funcionar no modo anônimo → É problema de cache

---

### **Verificar Status do GitHub Pages:**

1. Settings → Pages
2. Deve mostrar:
   ```
   ✅ Your site is live at https://usuario.github.io/repo/
   ```
3. Se mostrar erro ou aviso, leia a mensagem

---

## 🔄 Alternativa: GitHub Pages com Usuário

Se continuar com problemas, tente criar assim:

1. Crie repositório com nome **exato:** `SEU_USUARIO.github.io`
   - Exemplo: Se usuário é `joao123`, repositório deve ser `joao123.github.io`
2. Faça upload do `index.html`
3. Acesse: `https://SEU_USUARIO.github.io/`
   - SEM nome de repositório no final!

Este método sempre funciona!

---

## ⚡ Solução Rápida (Copiar e Colar)

Execute estes passos **exatamente**:

```
✅ 1. Vá em github.com e faça login
✅ 2. Clique no + → New repository
✅ 3. Nome: guardador (ou qualquer nome)
✅ 4. Public ✓
✅ 5. Create repository
✅ 6. Upload arquivo guardador.html
✅ 7. RENOMEIE para index.html
✅ 8. Commit changes
✅ 9. Settings → Pages
✅ 10. Source: main → Save
✅ 11. Aguarde 2 minutos
✅ 12. Acesse: https://SEU_USUARIO.github.io/guardador/
```

---

## 📞 Precisa de Ajuda?

Se seguiu tudo e ainda não funciona, me diga:

1. **Qual é seu usuário GitHub?**
2. **Qual o nome do repositório?**
3. **O arquivo se chama index.html?**
4. **GitHub Pages está ativo? (verde)**
5. **Qual erro aparece quando acessa a URL?**

Com essas informações, posso ajudar especificamente! 🚀

---

## 🎁 Bônus: Ferramentas de Teste

### **Teste se DNS está funcionando:**
```
https://dnschecker.org
```
Cole sua URL do GitHub Pages

### **Teste se site está online:**
```
https://isitdownrightnow.com
```

---

Boa sorte! 99% dos problemas são resolvidos com:
1. ✅ Arquivo se chama `index.html`
2. ✅ Está na raiz do repositório
3. ✅ GitHub Pages ativo
4. ✅ Aguardar 2 minutos

🎯 **Tente isso primeiro!**
