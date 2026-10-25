# Apuração 2º Turno 2026

Painel de apuração da eleição presidencial (2º turno, 25/10/2026) com dados oficiais do TSE, eleição 6258.
Atualiza sozinho a cada 15 segundos. Mostra o total Brasil, as 5 regiões e a evolução da apuração.

Site estático: só o `index.html`. Não precisa de build nem de dependências.

## Publicar na Vercel

1. Crie um repositório no GitHub e envie os arquivos desta pasta (`index.html`, `vercel.json`, `README.md`).
2. Na Vercel: Add New > Project > importe o repositório.
3. Framework Preset: Other. Build Command e Output Directory: deixe em branco.
4. Deploy. O link fica no formato `nome-do-projeto.vercel.app`.

## Ajustes rápidos

- Intervalo de atualização: `const INTERVAL = 15;` no `index.html`, em segundos.
- Os dados são lidos de `https://resultados.tse.jus.br/oficial/ele2026/6258/dados/{uf}/{uf}-c0001-e006258-u.json`.
