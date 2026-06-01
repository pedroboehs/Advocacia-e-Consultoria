# GitHub Setup Instructions

Este arquivo contém as instruções para completar a sincronização com GitHub.

## Passo 1: Criar o repositório no GitHub

1. Acesse https://github.com/new
2. Digite o nome: `advocacia-consultoria`
3. Escolha se quer públiico ou privado
4. **Importante:** NÃO inicialize com README, .gitignore ou LICENSE (já temos arquivos localmente)
5. Clique em "Create repository"

## Passo 2: Configurar o remote local

Após criar o repositório, copie o HTTPS URL dele (ex: `https://github.com/seu-usuario/advocacia-consultoria.git`) e execute:

```bash
cd ~/Desktop/"ADVOCACIA E CONSULTORIA"
git remote add origin https://github.com/seu-usuario/advocacia-consultoria.git
git branch -M main
git push -u origin main
```

## Pronto!

Agora a sincronização automática está funcionando. Cada commit será automaticamente enviado para o GitHub.

## Verificação

Para verificar se está tudo configurado corretamente:

```bash
git remote -v
```

Você deve ver algo como:
```
origin  https://github.com/seu-usuario/advocacia-consultoria.git (fetch)
origin  https://github.com/seu-usuario/advocacia-consultoria.git (push)
```
