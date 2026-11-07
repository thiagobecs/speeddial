# 🚀 SpeedDial

Seu painel de favoritos rápido, moderno, instalável (PWA) e sincronizado com o GitHub.

---

## 🌟 O que há de novo nesta versão

1. **Sincronização com GitHub (Multi-Dispositivo)**:
   - Salva suas alterações diretamente no arquivo `links.json` do seu repositório via API do GitHub.
   - Qualquer aparelho (celular, tablet, notebook) carrega seus links e notas atualizados.
2. **PWA (Progressive Web App)**:
   - Suporte a instalação como App nativo (no Chrome, Edge, Safari iOS e Android).
   - Suporte offline completo através do `sw.js` (Service Worker).
3. **Widget de Clima ao Vivo**:
   - Detecta o clima e temperatura local automaticamente usando a API gratuita Open-Meteo.
4. **Atalhos de Busca (!bangs)**:
   - `!y [busca]` busca no YouTube
   - `!gh [busca]` busca no GitHub
   - `!c [busca]` busca no ChatGPT
   - `!w [busca]` busca na Wikipedia
   - `!m [busca]` busca no Google Maps
   - `!a [busca]` busca na Amazon
   - `!r [busca]` busca no Reddit
5. **Bloco de Notas Rápidas**:
   - Painel retrátil no rodapé para lembretes e links temporários, salvo e sincronizado junto com os favoritos.
6. **Modo Compacto**:
   - Alternância entre cartões detalhados e modo dock/ícones de aplicativos.
7. **Colapso de Categorias**:
   - Clique no cabeçalho de qualquer categoria para recolher ou expandir.
8. **Atalhos de Teclado**:
   - Pressione `/` para focar na barra de busca.
   - Pressione `Alt + 1` até `Alt + 9` para abrir seus links favoritos rapidamente.

---

## 🛠️ Como subir para o GitHub e ativar o GitHub Pages

### Passo 1: Criar o repositório no GitHub
1. Acesse [github.com/new](https://github.com/new).
2. Dê o nome ao repositório (ex: `speeddial`).
3. Pode deixar **Público** (ou Privado se tiver GitHub Pro).
4. Não precisa marcar para criar README ou .gitignore (já criamos localmente).
5. Clique em **Create repository**.

### Passo 2: Enviar os arquivos pelo Terminal
No terminal, dentro da pasta deste projeto, execute:

```bash
git init
git add .
git commit -m "feat: speeddial com sync github, pwa e melhorias"
git branch -M main
git remote add origin https://github.com/SEU_USUARIO/speeddial.git
git push -u origin main
```
*(Substitua `SEU_USUARIO` pelo seu usuário do GitHub).*

### Passo 3: Ativar o GitHub Pages (100% Gratuito)
1. No seu repositório no GitHub, clique na aba **Settings** (Configurações).
2. No menu lateral esquerdo, clique em **Pages**.
3. Em **Build and deployment > Source**, selecione:
   - Branch: `main`
   - Pasta: `/ (root)`
4. Clique em **Save**.
5. Aguarde 1 a 2 minutos. O GitHub vai gerar sua URL:
   `https://SEU_USUARIO.github.io/speeddial/`

---

## 🔄 Como ativar a Sincronização Automática

1. Crie um Token no GitHub:
   - Vá em [github.com/settings/tokens](https://github.com/settings/tokens) (ou Settings > Developer Settings > Personal access tokens > Tokens (classic)).
   - Clique em **Generate new token (classic)**.
   - Dê um nome (ex: `SpeedDial Sync`).
   - Marque a caixinha **repo** (para poder atualizar o arquivo `links.json`).
   - Clique em **Generate token** e copie o código `ghp_...`.
2. Abra seu SpeedDial no navegador.
3. Clique no botão de engrenagem (⚙️) ou no botão **GitHub** no topo.
4. Vá na aba **Sincronização GitHub** e preencha:
   - Seu usuário
   - Nome do repositório (`speeddial`)
   - Cole seu token
5. Clique em **Salvar e Enviar**.

Pronto! Sempre que adicionar, editar ou excluir um link ou nota, ele salva no seu navegador e no GitHub. Quando abrir no celular ou em outro computador, os links estarão lá!
