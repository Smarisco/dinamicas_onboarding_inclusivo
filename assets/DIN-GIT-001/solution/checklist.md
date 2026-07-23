# DIN-GIT-001 — Checklist de Materiais
## Git em Conflito (Git in Conflict)

> **Duração:** 60 min | **Participantes:** 2–6 | **Modalidade:** Digital

---

## Pré-Dinâmica

### Ambiente técnico
- [ ] Repositório de treinamento clonado e com conflitos pré-fabricados verificados
- [ ] `user.name` e `user.email` configurados em cada máquina participante
- [ ] VS Code com extensão GitLens ou GitKraken instalado (visualização 3-way merge)
- [ ] Diff side-by-side projetado/compartilhado na tela antes do início
- [ ] Checklist de 5 passos impresso ou exibido: Identificar → Abrir → Escolher/combinar → Remover marcadores → Commitar

### Materiais de apoio
- [ ] Cenário narrativo do conflito preparado (quem fez o quê em qual branch)
- [ ] 3 conflitos preparados e verificados: C1 (Merge Simples), C2 (Lógica Conflitante), C3 (Rebase — opcional)
- [ ] Guia de recuperação disponível: como recriar o repositório se necessário

### Participantes
- [ ] Número confirmado (2–6) e duplas formadas
- [ ] Facilitador verificou que todos têm Git instalado e configurado
- [ ] Facilitador preparado para apresentar narrativa completa antes de começar

---

## Durante a Execução

### Conflitos
- [ ] Narrativa do conflito apresentada antes de qualquer comando (quem, o quê, qual branch)
- [ ] C1 — Merge Simples (15 min): duplas executam `git merge` e resolvem conflito de texto
- [ ] Revisão coletiva (5 min): estratégias comparadas entre duplas
- [ ] C2 — Lógica Conflitante (15 min): ambas versões válidas — combinação necessária
- [ ] C3 — Rebase (10 min): **somente para perfis avançados** — verificar perfil antes de acionar

### Acessibilidade Sensorial (TEA)
- [ ] VS Code 3-way merge view ou GitKraken ativo — não usar diff em terminal puro
- [ ] Mensagens de erro Git contextualizadas antes de ocorrerem: "erros são esperados e reversíveis"
- [ ] Repositório de treinamento pode ser recriado a qualquer momento — comunicar isso antes de começar
- [ ] Prática em dupla mantida — não solicitar resolução individual sem suporte

---

## Pós-Dinâmica

### Debriefing
- [ ] Pergunta-chave lançada: *"Como comunicar melhor ao fazer um PR para evitar conflitos futuros?"*
- [ ] Lição central registrada: **Conflito Git = divergência de intenção — resolver requer comunicação, não apenas comandos**
- [ ] Compromisso pessoal escrito por cada participante (1 prática de PR)

### Registro
- [ ] Conflitos resolvidos por dupla anotados (C1 / C2 / C3)
- [ ] Estratégia mais usada na resolução registrada
- [ ] Observações sensoriais (ansiedade com erros, pressão de tempo) registradas
- [ ] Template de debriefing preenchido e arquivado
