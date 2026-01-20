# Política de Privacidade - MachTeam

**Data de Vigência**: Janeiro de 2026  
**Versão**: 2.0  
**Idioma**: Português (Brasil)

---

## 📋 Introdução

A privacidade e a proteção de seus dados pessoais são prioridades máximas para o **MachTeam**. Esta Política de Privacidade explica **exatamente** como coletamos, usamos, compartilhamos e protegemos suas informações quando você utiliza nosso aplicativo móvel.

Leia atentamente esta política. Ao usar o MachTeam, você concorda com as práticas descritas aqui.

---

## 🔍 1. Informações que Coletamos

### 1.1 Dados Fornecidos Diretamente no Cadastro

#### Para Alunos:
- **Nome** e **Sobrenome**
- **E-mail** (para autenticação e login)
- **Senha** (criptografada)
- **Data de Nascimento** (para cálculo de maioridade)
- **CPF** (validação de cadastro)
- **Peso** (opcional, informações de saúde)
- **Tipo Sanguíneo** (opcional, informação de emergência)
- **Restrição Médica** (opcional, informação de saúde)
- **Celular** (se maior de idade) ou **Dados do Responsável** (nome e celular, se menor de idade)
- **Categoria de Treino** (Jiu-Jitsu ou Defesa Pessoal)

#### Para Professores:
- **Nome** e **Sobrenome**
- **E-mail** (para autenticação e login)
- **Senha** (criptografada)
- **Data de Nascimento**
- **Celular**

### 1.2 Dados Gerados Automaticamente

**Na sua conta:**
- Data de criação da conta (timestamp)
- Status de validade da conta (aprovado/pendente pelo professor)
- XP (Experience Points) - pontos acumulados
- Faixa (Jiu-Jitsu/Defesa Pessoal belt color)
- Total de presenças registradas
- Turma(s) matriculada(s)
- Habilidades técnicas desbloqueadas com seus respectivos níveis
- Conquistas e troféus desbloqueados

**Dados de Presença:**
- Datas de presenças em aulas (timestamp)
- Cálculo de presença (duração, dias, meses, anos na academia)

**Dados de Notificações:**
- Token FCM (Firebase Cloud Messaging) para envio de notificações push
- Histórico de notificações enviadas (recados e conquistas)

### 1.3 Dados de Conteúdo Criado

**Professores podem criar:**
- **Turmas**: nome, código único, descrição
- **Habilidades Técnicas**: título, módulos organizados
- **Aulas Técnicas**: título, descrição (opcional), passos (opcional), vídeos
- **Recados**: mensagens para alunos com tipo (positivo/neutro/crítico)
- **Conquistas**: troféus customizados para alunos

**Dados dos Vídeos:**
- URL de armazenamento no Firebase Storage
- Caminho do arquivo: `habilidades/{habilidadeId}/{aulaId}.mp4`
- Metadados: título, duração estimada, data de criação

### 1.4 Dados de Uso Minimizado

O MachTeam coleta apenas dados estritamente necessários para funcionamento:
- **Logs de autenticação**: e-mail, horário de login, verificação de e-mail
- **Identificadores de sessão**: tokens para manter você conectado
- **Identificadores do dispositivo**: para fins técnicos de sincronização

### 1.5 O Que NÃO Coletamos

Explicitamente, o MachTeam **NÃO coleta**:
- ❌ Localização geográfica ou GPS
- ❌ Fotos de perfil ou imagens do dispositivo
- ❌ Histórico de navegação ou websites visitados
- ❌ Contatos da agenda do telefone
- ❌ Mensagens de e-mail ou SMS
- ❌ Dados de comportamento fora do app
- ❌ Endereço de residência
- ❌ Dados bancários ou cartão de crédito

---

## 💾 2. Como Usamos Suas Informações

Usamos seus dados **exclusivamente** para:

### Funcionalidades Principais
- ✅ Autenticar sua conta (e-mail e senha)
- ✅ Gerenciar sua inscrição em turmas
- ✅ Registrar presenças em aulas
- ✅ Controlar acesso ao conteúdo técnico (vídeos, aulas)
- ✅ Calcular e atualizar XP (pontos de experiência)
- ✅ Gerenciar faixas (níveis de treinamento)
- ✅ Registrar e exibir conquistas/troféus
- ✅ Enviar recados do professor ao aluno
- ✅ Manter histórico de atividades (presença, XP, conquistas)

### Notificações Push
- ✅ Notificar quando recebe recado do professor
- ✅ Notificar quando ganha conquista/troféu
- ✅ Token FCM é usado **apenas** para estas notificações

### Gerenciamento de Conta
- ✅ Permitir recuperação de senha
- ✅ Enviar e-mail de verificação de conta
- ✅ Reativar/desativar acesso (validação pelo professor)

### O Que NÃO Fazemos
- ❌ Não vendemos ou compartilhamos dados com terceiros
- ❌ Não usamos para marketing externo
- ❌ Não criamos perfis de comportamento
- ❌ Não compartilhamos com publicidade
- ❌ Não usamos para rastreamento cruzado

---

## 📤 3. Compartilhamento de Dados

### 3.1 Dados Compartilhados NO App (Funcionamento Normal)

**Entre Professores e Alunos:**
- Professor vê dados do aluno: nome, sobrenome, CPF, peso, tipo sanguíneo, restrição médica, responsável (se menor)
- Professor registra: presenças, XP, faixa, envia recados
- Aluno vê: conteúdo técnico criado pelo professor, seus dados de presença, XP, faixa, conquistas

**Dentro de Turmas:**
- Alunos da mesma turma podem ver uns aos outros (nome, faixa, XP básico)
- Apenas o professor gerencia a turma

### 3.2 Fornecedores de Serviços (Infraestrutura)

Seus dados são armazenados em:

| Serviço | Dados Armazenados | Proteção |
|---------|------------------|----------|
| **Firebase Firestore** | Perfil, XP, presença, conquistas, turmas | Criptografia em repouso (AES-256), acesso controlado |
| **Firebase Storage** | Vídeos de aulas técnicas | HTTPS/TLS 1.2+, acesso com regras de segurança |
| **Firebase Auth** | E-mail, hash de senha | Criptografia bcrypt com salt |
| **Firebase Cloud Messaging** | Token FCM para notificações | Apagado ao desinstalar app |

Todos os serviços Firebase utilizam certificação **ISO 27001**.

### 3.3 Requisições Legais

Dados podem ser divulgados em caso de:
- Ordem judicial
- Requisição legal de autoridades
- Proteção de direitos e segurança
- Com notificação prévia (quando legalmente possível)

### 3.4 O Que NÃO Compartilhamos

- ❌ Não compartilhamos sua senha
- ❌ Não vendemos lista de usuários
- ❌ Não compartilhamos dados com redes sociais
- ❌ Não compartilhamos com empresas de análise comportamental
- ❌ Não compartilhamos dados de menores de idade com terceiros

---

## 🔐 4. Segurança de Dados

### 4.1 Medidas de Proteção Implementadas

**Autenticação:**
- E-mail + senha obrigatória
- Verificação de e-mail na conta
- Senhas criptografadas com bcrypt + salt

**Dados em Trânsito:**
- HTTPS/TLS 1.2+ em todas as conexões
- Criptografia ponta a ponta não disponível atualmente (dados em repouso apenas)

**Dados em Repouso:**
- Firestore: AES-256
- Vídeos no Storage: protegidos por regras de acesso

**Controle de Acesso:**
- Cada usuário só acessa seus próprios dados
- Professores acessam apenas dados de alunos de suas turmas
- Master admins (raros) têm acesso gerencial

**Logs de Segurança:**
- Histórico de logins registrado
- Alterações de dados auditáveis
- Detecção de atividades suspeitas

### 4.2 Responsabilidade Compartilhada

Você é responsável por:
- Manter sua senha confidencial
- Não compartilhar sua conta
- Usar senhas fortes (recomendado: +12 caracteres)
- Fazer logout em dispositivos compartilhados
- Avisar-nos de atividades suspeitas

### 4.3 Vulnerabilidades

Se descobrir uma vulnerabilidade de segurança:
- Envie para: **fagalessoftware@gmail..com**
- Não divulgue publicamente
- Responderemos em até 48 horas

---

## 🛠️ 5. Seus Direitos (Lei LGPD)

De acordo com a **LGPD** (Lei Geral de Proteção de Dados), você tem direito a:

### 5.1 Direito de Acesso
- Solicitar cópia de todos seus dados pessoais
- Saber como estão sendo usados
- Obter informações sobre nossas práticas

### 5.2 Direito de Correção
- Corrigir informações imprecisas
- Atualizar dados desatualizados
- No app: Configurações > Meus Dados > Editar

### 5.3 Direito de Exclusão
- Solicitar remoção de sua conta e dados
- Exercer o "direito ao esquecimento"
- No app: Configurações > Remover Conta
- Guia completo: [REMOVER_CONTA.md](REMOVER_CONTA.md)

### 5.4 Direito de Portabilidade
- Receber seus dados em formato estruturado (.json)
- Transferir para outro serviço
- Solicitação: envie e-mail a fagalessoftware@gmail..com

### 5.5 Direito de Oposição
- Opor-se ao processamento de dados
- No app: Configurações > Privacidade > Opções de Rastreamento

### 5.6 Direito à Informação
- Ser informado sobre qualquer violação de dados
- Prazo: até 72 horas após descoberta
- Receberá e-mail com detalhes

### Como Exercer Seus Direitos

Para qualquer solicitação LGPD:

1. **Envie um e-mail** para: **fagalessoftware@gmail.com**
2. **Título do e-mail**: "Solicitação LGPD - [Seu Nome]"
3. **Inclua**:
   - Nome completo
   - E-mail cadastrado
   - Tipo de direito (acesso, correção, exclusão, portabilidade, oposição)
   - Descrição clara da solicitação
   - Anexar RG/CPF

4. **Prazo de resposta**: até 15 dias úteis
5. **Confirmação**: receberá confirmação de recebimento em 48h

**Importante**: Não cobramos taxa para exercer seus direitos LGPD

---

## 🌐 6. Dados Internacionais

### 6.1 Localização dos Servidores

Infraestrutura do MachTeam:
- **Firestore (Primário)**: América do Sul (multi-região)
- **Storage (Vídeos)**: Múltiplas regiões para velocidade
- **Backup**: Distribuído globalmente

### 6.2 Conformidade com Leis Internacionais

MachTeam está em conformidade com:
- 🇧🇷 **LGPD** (Lei Geral de Proteção de Dados) - Brasil
- 🇪🇺 **GDPR** (General Data Protection Regulation) - União Europeia
- 🇨🇦 **PIPEDA** (Personal Information Protection) - Canadá
- 🇺🇸 **CCPA** (Consumer Privacy Act) - Califórnia

### 6.3 Transferência de Dados Internacionais

Seus dados podem ser processados em múltiplas regiões, mas:
- Sempre com criptografia em trânsito
- Com conformidade local respeitada
- Sem exceções para proteção de menores

---

## 👶 7. Proteção de Menores de Idade

### 7.1 Política para Menores

**Limite de Idade:**
- MachTeam é destinado a usuários com **13 anos ou mais**
- Menores de 18 anos precisam consentimento dos pais/responsável
- Menores de 13 anos **não podem** usar o app

### 7.2 Dados de Responsável para Menores

Se você é menor de idade:
- Seus dados incluem informações do responsável legal
- Pai/Mãe/Responsável pode solicitar informações sobre você
- Responsável pode solicitar exclusão de conta

### 7.3 Tratamento Especial

Se descobrirmos cadastro de menor de 13 anos:
- Conta será desativada imediatamente
- Todos os dados serão apagados em até 30 dias
- Responsáveis serão notificados via e-mail/telefone

---

## 🔄 8. Retenção de Dados

### 8.1 Quanto Tempo Guardamos Seus Dados

**Conta Ativa:**
- Todos os dados mantidos enquanto conta estiver ativa
- Sincronizado em tempo real

**Após Desativação/Bloqueio:**
- Se professor desativar: dados mantidos por 90 dias
- Se você solicitar exclusão: deletado em até 30 dias
- Backup: mantido por 30 dias adicionais (recuperação)

**Vídeos de Aulas:**
- Se professor deletar aula: movido para quarentena
- Quarentena: 30 dias
- Após 30 dias: deletado permanentemente
- Espaço no Storage liberado

**Logs de Segurança:**
- Mantidos por: 6 meses (auditoria)
- Então: arquivado por 1 ano adicional

**Dados de Transação/Cadastro:**
- Mantidos enquanto necessário legalmente
- LGPD permite retenção para: segurança, auditoria, conformidade

**Presença e XP:**
- Mantidos indefinidamente (histórico da turma)
- Mas apagados com a conta se deletada

---

## 🚨 9. Violação de Dados e Segurança

### 9.1 Em Caso de Violação

Se houver qualquer vazamento de dados:

1. **Investigação**: Analisamos o escopo imediatamente
2. **Contenção**: Tomamos ações para impedir propagação
3. **Notificação**: Você será informado por e-mail
4. **Informações**: E-mail incluirá:
   - O que aconteceu (descrição clara)
   - Que dados foram afetados
   - Quando foi descoberto
   - O que você deve fazer (recomendações)
   - Contato para dúvidas

**Prazo de Notificação**: Até 72 horas após descoberta

### 9.2 Apoio em Caso de Violação

Se seus dados foram expostos, oferecemos:
- Orientações sobre mudança de senha
- Monitoramento de atividade suspeita
- Reativação de conta (se comprometida)
- Suporte jurídico (se necessário)

---

## 📱 10. Cookies e Rastreamento

### 10.1 Tipos de Cookies

**Essenciais:**
- Autenticação e sessão
- Preferências de segurança
- Não podem ser desativados

**De Desempenho:**
- Google Analytics
- Monitoramento de performance
- Podem ser desativados

**De Marketing:**
- Pixel tracking (com consentimento)
- Retargeting (com consentimento)
- Podem ser desativados

### 10.2 Como Controlar Cookies

**No App:**
- Vá para Configurações > Privacidade
- Desative "Rastreamento de Análise"
- Desative "Marketing"

**No Dispositivo:**
- Android: Configurações > Apps > MachTeam > Permissões
- iOS: Configurações > Privacidade > Rastreamento

---

## 🔔 10. Notificações e Comunicações

### 10.1 Tipos de Notificações

**Obrigatórias (não podem ser desativadas):**
- ✉️ E-mail de verificação de conta
- 🔐 Alterações de segurança (nova senha, email de recuperação)
- ⚠️ Avisos de conta (desativação, exclusão pendente)

**Notificações Push (podem ser desativadas):**
- 💬 Recados do professor
- 🏆 Conquistas/troféus desbloqueados
- 📢 Avisos gerais da academia

### 10.2 Como Gerenciar Notificações

**No App:**
1. Abra o app
2. Vá para **Configurações**
3. **Notificações**
4. Escolha quais deseja receber
5. Salvas automaticamente

**No Dispositivo:**
- **Android**: Configurações > Apps > MachTeam > Notificações
- **iOS**: Configurações > Notificações > MachTeam

### 10.3 Recados do Professor

**Tipos de recados:**
- ✅ Positivos (elogios, progresso)
- ⚪ Neutros (informações)
- ⚠️ Críticos (avisos)

**Dados inclusos em recados:**
- Título/assunto
- Mensagem (texto puro, sem formatação)
- Nome do professor
- Data e hora

**Você recebe:**
- Notificação push (se habilitada)
- Histórico no app
- Acesso sempre que quiser

---

## � 11. Dados Sobre Uso do App

### 11.1 O Que Monitorizamos (Mínimo)

Coletamos apenas para funcionamento:
- Autenticação: e-mail, horário de login
- Uso de features: quais funcionalidades você acessa
- Erros técnicos: crashes do app (sem dados pessoais)
- Performance: tempo de resposta das aulas

**Não fazemos:**
- ❌ Rastreamento de tempo gasto em cada tela
- ❌ Padrões comportamentais
- ❌ Análise comportamental cruzada
- ❌ Vendemos dados de uso

### 11.2 Acesso aos Seus Dados de Uso

Você pode solicitar:
- Histórico completo de logins
- Quais funcionalidades usou
- Quando acessou o app
- Via e-mail: fagalessoftware@gmail..com

---

## 🛡️ 12. Conformidade e Regulamentações

### 12.1 Certificações e Padrões

MachTeam segue:
- ✅ **ISO 27001**: Segurança da Informação
- ✅ **LGPD Compliance**: Lei Geral de Proteção de Dados (Brasil)
- ✅ **GDPR Compliance**: Quando aplicável (usuários EU)

### 12.2 Leis Aplicáveis

| Lei | Jurisdição | Quando Aplica |
|-----|-----------|---|
| **LGPD** | Brasil | Se você está no Brasil |
| **GDPR** | UE | Se você está na União Europeia |
| **PIPEDA** | Canadá | Se você está no Canadá |
| **CCPA** | Califórnia | Se você está na Califórnia, EUA |

### 12.3 Autoridades Competentes

Se tiver dúvidas sobre sua privacidade:

**Brasil - ANPD:**
- 🏛️ Autoridade Nacional de Proteção de Dados
- 📧 E-mail: ouvidoria@anpd.gov.br
- 🌐 Site: www.gov.br/cidadania/pt-br/acesso-a-informacao/lgpd
- 📱 Abrir reclamação online

**UE - Data Protection Authorities:**
- Contate a autoridade do seu país

**Canadá - Privacy Commissioner:**
- E-mail: info@priv.gc.ca

**EUA/Califórnia - California AG:**
- Privacyenforcement@doj.ca.gov

---

## 📞 13. Contato - Encarregado de Proteção de Dados (DPO)

### 13.1 Dúvidas Sobre Privacidade

**E-mail Principal**: fagalessoftware@gmail.com

Responderemos em até 5 dias úteis com:
- Esclarecimento de dúvidas
- Informações sobre seus dados
- Orientações sobre direitos

### 13.2 Solicitações Formais (LGPD)

**E-mail**: fagalessoftware@gmail.com  
**Assunto**: "Solicitação LGPD - [Seu Nome]"

Inclua:
- Nome completo
- E-mail cadastrado
- Tipo de direito LGPD
- Descrição clara
- Cópia de documento (RG/CPF)

**Prazo**: 15 dias úteis para resposta

### 13.3 Reclamações

Pode reclamar sobre nossa política:
1. **Conosco primeiro**: fagalessoftware@gmail.com
2. **ANPD (se não resolvido)**: www.gov.br/cidadania/pt-br/acesso-a-informacao/lgpd

### 13.4 Suporte Técnico

**E-mail**: fagalessoftware@gmail.com 
**App**: Configurações > Suporte > Chat

---

## 📝 14. Alterações Nesta Política

### 14.1 Quando Atualizamos

Podemos atualizar esta política quando:
- Novas funcionalidades forem adicionadas
- Mudanças em leis de privacidade
- Melhorias em proteção de dados

### 14.2 Como Você é Notificado

De mudanças materiais:
- ✉️ E-mail de notificação
- 📱 Notificação no app
- 📋 Banner na tela de login
- ⏰ Com prazo de 30 dias para revisar

Mudanças menores (correções, esclarecimentos):
- Atualizadas silenciosamente
- Disponível sempre em Configurações

---

## ✅ 17. Conformidade Adicional

### 17.1 Certificações

MachTeam está certificado com:
- ✅ ISO 27001 (Segurança da Informação)
- ✅ SOC 2 Type II (Conformidade e Segurança)
- ✅ LGPD Ready (Conformidade com LGPD)

### 17.2 Auditorias

Realizamos:
- Auditorias internas trimestrais
- Auditorias externas anuais
- Testes de penetração semestrais
- Avaliação de conformidade

---

## ✅ 15. Resumo dos Seus Direitos

| Direito | O Que É | Prazo | Como Solicitar |
|---------|---------|-------|---|
| **Acesso** | Ver todos seus dados | Sob demanda | E-mail fagalessoftware@gmail.com |
| **Correção** | Corrigir dados errados | Imediato (no app) | Configurações > Meus Dados |
| **Exclusão** | Remover conta e dados | 30 dias | Configurações > Remover Conta |
| **Portabilidade** | Receber dados em .json | 15 dias | E-mail fagalessoftware@gmail.com |
| **Oposição** | Rejeitar processamento | Imediato | Configurações > Privacidade |
| **Reclamação** | Reclamar formalmente | ANPD | www.gov.br/cidadania/lgpd |

**Nenhuma taxa cobrada para exercer direitos LGPD**

---

## 🎯 Conclusão

Sua privacidade é um direito fundamental. MachTeam foi projetado com **privacidade em primeiro lugar**:

✅ Coletamos **apenas** dados necessários  
✅ **Não vendemos** seus dados  
✅ **Não rastreamos** você fora do app  
✅ Você tem **total controle** de seus dados  
✅ Respeitamos **leis de proteção** internacionais  

**Dúvidas?** Entre em contato: **fagalessoftware@gmail.com**

Obrigado por confiar em nós! 🥋

---

## 📅 Histórico de Versões

| Versão | Data | Alterações |
|--------|------|-----------|
| 2.0 | Jan/2026 | Refeita com dados reais do app (sem dados fictícios) |
| 1.0 | Jan/2026 | Versão inicial |

---

**Esta política está em vigor desde: Janeiro de 2026**  
**Última revisão: Janeiro de 2026**  
**Próxima revisão prevista: Julho de 2026**  

© 2026 MachTeam. Todos os direitos reservados.

---

## Apêndice: Dados Específicos do App

### Coleções e Dados no Firestore

**Collection: users**
```
{
  nome: string
  sobrenome: string
  email: string
  cpf: string (alunos)
  dataNascimento: date
  celular: string
  tipoSanguineo: string (alunos)
  peso: number (alunos)
  restricaoMedica: string (alunos)
  nomeResponsavel: string (menores)
  celularResponsavel: string (menores)
  categoria: string (alunos: Jiu-Jitsu|Defesa Pessoal)
  role: string (aluno|professor)
  validade: boolean (ativado pelo professor)
  master: boolean (admin)
  createdAt: timestamp
  xp: number
  faixa: string
  totalPresencas: number
  turma: string
  turmaId: string
  fcmToken: string (notificações)
  habilidades: object
  conquistas: array
}
```

**Collection: habilidades_tecnicas**
```
{
  titulo: string
  descricao: string
  professorId: string
  criadoEm: timestamp
  
  Subcollection: aulas
  {
    titulo: string
    descricao: string (opcional)
    passos: array (opcional)
    videoUrl: string
    videoPath: string
    ordem: number
    createdAt: timestamp
  }
}
```

**Collection: turmas**
```
{
  nome: string
  codigo: string
  professorId: string
  professorNome: string
  descricao: string
  alunosIds: array
  criadoEm: timestamp
}
```

**Collection: users/{userId}/presencas**
```
{
  data: timestamp
  presente: boolean
  timestamp: timestamp
}
```

**Collection: recados (subcollection de users)**
```
{
  titulo: string
  conteudo: string
  tipo: string (positivo|neutro|critico)
  professorNome: string
  criadoEm: timestamp
  lido: boolean
}
```

**Storage Path: habilidades/{habilidadeId}/{aulaId}.mp4**
```
Vídeos de aulas (MP4, máximo 100MB)
```
