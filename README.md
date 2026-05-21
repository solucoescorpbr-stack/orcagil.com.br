# Orça Ágil — Site Institucional

Site estático do app **Orça Ágil**, da **Support Soluções Corporativas LTDA**. Pronto para hospedar no **GitHub Pages**.

## 📁 Estrutura do projeto

```
.
├── index.html         # Landing page principal
├── privacidade.html   # Política de Privacidade (LGPD)
└── README.md          # Este arquivo
```

Não há dependências, build, frameworks ou backend. Tudo são arquivos estáticos prontos para servir.

---

## 🚀 Como publicar no GitHub Pages

### Opção 1 — Pela interface do GitHub (mais simples)

1. **Crie um repositório novo** no GitHub (público ou privado em conta paga). Exemplo: `orca-agil-site`.
2. **Envie os arquivos** (`index.html`, `privacidade.html`, `README.md`) para a branch `main` do repositório:
   - Pela interface web: botão **"Add file" → "Upload files"** → arraste os arquivos → **"Commit changes"**.
3. No repositório, vá em **Settings → Pages** (menu lateral).
4. Em **"Build and deployment"**:
   - **Source:** `Deploy from a branch`
   - **Branch:** `main` (ou `master`) → pasta `/ (root)` → **Save**.
5. Aguarde 1–2 minutos. O GitHub mostrará a URL no topo da página:
   ```
   https://SEU-USUARIO.github.io/orca-agil-site/
   ```
6. Acesse a URL — pronto! O site está no ar.

### Opção 2 — Via linha de comando (Git)

```bash
# Dentro da pasta com os arquivos
git init
git add .
git commit -m "Site inicial do Orça Ágil"
git branch -M main
git remote add origin https://github.com/SEU-USUARIO/orca-agil-site.git
git push -u origin main
```

Depois, configure o GitHub Pages como descrito na **Opção 1**, passos 3 a 6.

---

## 🌐 Domínio personalizado (opcional)

Se você tiver o domínio `orcagil.com.br`:

1. Crie um arquivo chamado `CNAME` (sem extensão) na raiz do repositório com o conteúdo:
   ```
   orcagil.com.br
   ```
2. No painel do seu provedor de domínio (Registro.br, GoDaddy, etc.), configure os registros DNS:
   - **Registros A** apontando para os IPs do GitHub Pages:
     ```
     185.199.108.153
     185.199.109.153
     185.199.110.153
     185.199.111.153
     ```
   - Ou um **CNAME** `www` apontando para `SEU-USUARIO.github.io`.
3. Volte em **Settings → Pages**, preencha **Custom domain** com `orcagil.com.br` e marque **Enforce HTTPS**.

A propagação DNS pode levar de alguns minutos até 24 horas.

---

## ✏️ Como editar o site

Os arquivos são HTML puro com CSS embutido. Para alterar:

- **Texto, descrições, link da Play Store** → edite diretamente os arquivos `index.html` e `privacidade.html` em qualquer editor (VS Code, bloco de notas, ou pela interface do GitHub).
- **Cor da marca** → no `<style>` do início de cada arquivo, altere a variável CSS `--orange: #E67E22;`.
- **Link da Play Store** → no `index.html`, procure `href="#"` nos botões "Baixar na Play Store" e substitua pelo link real do app.
- **Data da Política de Privacidade** → no `privacidade.html`, atualize a linha que começa com `Última atualização:`.

Após editar e fazer commit, o GitHub Pages republica o site automaticamente em 1–2 minutos.

---

## 📧 Contato

- **E-mail:** contato@orcagil.com.br
- **Empresa:** Support Soluções Corporativas LTDA
