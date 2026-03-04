# 📊 Dashboard Linha Viva

Painel de controle de produção, faturamento e equipes.

---

## 🚀 Deploy no Vercel

### Opção 1 — Via GitHub (recomendado)

1. Crie um repositório no [GitHub](https://github.com/new)
2. Faça upload dos arquivos:
   - `index.html`
   - `vercel.json`
3. Acesse [vercel.com](https://vercel.com) e faça login com GitHub
4. Clique em **"Add New Project"**
5. Selecione o repositório
6. Clique em **"Deploy"**
7. ✅ Pronto! URL gerada automaticamente

> **Para atualizar:** basta substituir o `index.html` no GitHub — o Vercel republica sozinho.

---

### Opção 2 — Via Vercel CLI

```bash
npm i -g vercel
vercel
```

---

## 📁 Estrutura dos Arquivos

```
/
├── index.html     ← Dashboard completo (único arquivo)
├── vercel.json    ← Configuração do Vercel
└── README.md      ← Este arquivo
```

---

## 📥 Como importar dados

1. Acesse o painel **Importar** no dashboard
2. Faça upload do arquivo Excel `.xlsx`
3. Se o arquivo tiver múltiplas abas, todas são carregadas automaticamente
4. A aba chamada **`cancelados`** alimenta o painel de Cancelamentos

### Colunas aceitas no Excel

| Coluna | Descrição |
|---|---|
| `data` | Data do serviço (dd/mm/aaaa) |
| `equipe` | LV-01, LV-02, LV-03 ou LV-04 |
| `os` | Número da Ordem de Serviço |
| `valor` | Valor executado (R$) |
| `tipo_servico` | Tipo do serviço (SGM, GA, WTS...) |
| `dias_sem_prod` | Dias sem produção |
| `justificativa` | Motivo de parada |

---

## 👥 Equipes

| ID | Responsável | Meta Diária |
|---|---|---|
| LV-01 | Jucier | R$ 5.500 |
| LV-02 | Mauro | R$ 3.500 |
| LV-03 | Gleidson | R$ 3.500 |
| LV-04 | Marcos Pinto | R$ 3.500 |
