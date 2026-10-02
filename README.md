# SrRobs Virtual Ai — Demos privadas para clientes

Site público com **gate de palavra-passe** (GitHub Pages) para enviar demos a clientes.
O cliente abre o link, escreve a palavra-passe e vê as demos — sem conta GitHub.

**URL:** https://robertomf170.github.io/srrobs-demos/
**Palavra-passe atual:** `SrRobsDemo2026` (enviar só ao cliente, por canal à parte)

## ⚠️ Honestidade sobre a proteção
O gate é uma **proteção simples no browser** (dissuasor), **não é segurança forte**:
quem saiba ler o código-fonte consegue contorná-lo. Serve para o link não abrir
diretamente a ninguém. Não meter aqui dados sensíveis de clientes.

## Como mudar a palavra-passe
1. Gerar o novo hash SHA-256, ex.:
   `python -c "import hashlib; print(hashlib.sha256(b'NOVA_PALAVRA_PASSE'.encode()).hexdigest())"`
2. Trocar a constante `HASH` em `index.html`.
3. `git add index.html && git commit -m "..." && git push`

## Fonte de verdade
Os HTMLs das demos são cópias de `entregas/demos/` (workspace da Empresa) + um pequeno
script de guarda que redireciona para `index.html` sem palavra-passe.
**Editar sempre em `entregas/demos/`** e voltar a copiar para aqui.

## Publicar
```bash
git add -A && git commit -m "update demos" && git push
```
O GitHub Pages publica automaticamente a branch `main`.

---

### 📦 Packs Disponíveis

Clique no link abaixo para ver o **DEMO SIMULADO**:

- [Pack 1: Sistema de Automação Comercial](https://robertomf170.github.io/srrobs-demos/pack1/)
- [Pack 2: Plataforma de Gestão de Projetos](https://robertomf170.github.io/srrobs-demos/pack2/)
- [Pack 3: Sistema de Monitorização em Tempo Real](https://robertomf170.github.io/srrobs-demos/pack3/)
