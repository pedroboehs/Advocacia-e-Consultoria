# 📋 Guia de Importação de Skills - Advocacia e Consultoria

Este guia explica como sua equipe pode importar todas as skills customizadas do projeto.

## 📁 Arquivos de Exportação

- **SKILLS_EXPORT.md** - Documentação completa de todas as skills
- **skills-config.json** - Configuração em JSON (para referência e automação)
- **SKILLS_IMPORT.md** - Este guia

## 🚀 Opção 1: Importação Manual (Recomendado para começar)

### Passo 1: Acessar Claude Code
1. Abra [claude.ai/code](https://claude.ai/code)
2. Faça login com sua conta
3. Abra ou crie um novo workspace

### Passo 2: Importar uma Skill
Cada skill pode ser criada/importada usando a skill `/skill-creator`:

```
/skill-creator
```

Então descreva a skill que quer importar com base nas informações em `SKILLS_EXPORT.md`.

### Passo 3: Exemplo de Importação
Para importar a skill **squad-copy**, por exemplo:

```
/skill-creator

Nome da skill: Squad Copy

Descrição: Escreve todos os textos persuasivos do sistema: bio do Instagram, CTAs, copy de landing pages, sequências de venda e textos de afiliados. Especialista em conversão sem parecer publicidade.

Gatilhos (triggers):
- copy
- bio
- CTA
- texto de venda
- landing page
- persuasão
- converter
- chamada
- oferta

Quando ativar:
- Escrever bio de perfil
- Criar CTA para post
- Montar página de vendas
- Redigir copy de info-produto
- Criar sequência de mensagens
- Refinar qualquer texto de venda
```

## 📋 Ordem Recomendada de Importação

Para manter a coesão do projeto, importe nesta ordem:

### Camada 1: Identidade e Branding
1. **identidade-visual** - Base visual do projeto
2. **humanizer-pt-br** - Qualidade de linguagem

### Camada 2: Content & Copy
3. **squad-conteudo** - Criação de conteúdo
4. **squad-copy** - Textos persuasivos
5. **squad-tendencias** - Identificação de tendências

### Camada 3: Performance e Monetização
6. **squad-analytics** - Análise de performance
7. **squad-afiliados** - Monetização
8. **squad-trafego** - Crescimento e tráfego

### Camada 4: Coordenação (Opcional)
9. **squad-orquestrador** - Coordenação entre squads
10. **squad-design** - (Escopo a definir)
11. **squad-dev** - (Escopo a definir)

## 🔗 Integração com Seu Projeto

### Passo 1: Clone/Acesse o Repositório
```bash
git clone https://github.com/seu-usuario/advocacia-consultoria.git
cd advocacia-consultoria
```

### Passo 2: Leia a Documentação
Leia os seguintes arquivos em ordem:
1. `CLAUDE.md` - Visão geral do projeto
2. `SKILLS_EXPORT.md` - Descrição de todas as skills
3. `skills-config.json` - Referência técnica

### Passo 3: Configure as Skills no Seu Ambiente
1. Abra Claude Code no projeto
2. Use `/skill-creator` para adicionar cada skill
3. Teste cada skill conforme a documentação

## ✅ Checklist de Implementação

- [ ] Leu CLAUDE.md
- [ ] Leu SKILLS_EXPORT.md
- [ ] Importou identidade-visual
- [ ] Importou humanizer-pt-br
- [ ] Importou squad-conteudo
- [ ] Importou squad-copy
- [ ] Importou squad-tendencias
- [ ] Importou squad-analytics
- [ ] Importou squad-afiliados
- [ ] Importou squad-trafego
- [ ] Importou squad-orquestrador
- [ ] Testou todas as skills no projeto
- [ ] Documentou customizações locais

## 🔄 Sincronização Contínua

O projeto usa **GitHub Sync** automático:

```bash
# A cada commit, as mudanças são automaticamente sincronizadas com GitHub
git commit -m "Sua mensagem"
# O hook pós-commit automaticamente roda: git push
```

Isso garante que toda a equipe sempre tenha as versões mais recentes.

## 📞 Suporte

Se encontrar problemas ao importar uma skill:

1. **Verifique a descrição** em SKILLS_EXPORT.md
2. **Copie os gatilhos exatos** (triggers)
3. **Use a skill /skill-creator** com as informações do JSON
4. **Teste** com um exemplo do caso de uso

## 🎯 Próximos Passos Após Importação

1. **Customize conforme necessário** para sua região/nicho
2. **Teste em posts/conteúdos reais** antes de usar em produção
3. **Documente customizações** no arquivo `SKILLS_IMPORT.md` da sua equipe
4. **Compartilhe feedbacks** sobre o que funciona melhor
5. **Monitore performance** usando squad-analytics

## 📊 Rastreamento de Versões

- **Versão de Exportação**: 1.0
- **Data de Exportação**: 2026-06-02
- **Projeto**: Advocacia e Consultoria
- **Status**: Ativo - Atualizando regularmente

---

**Última atualização**: 2026-06-02  
**Mantido por**: Sistema Claude Code  
**Próxima revisão**: 2026-07-02
