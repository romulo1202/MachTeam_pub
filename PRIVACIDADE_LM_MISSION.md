# Política de Privacidade — LM Mission

Última atualização: 02/02/2026

Esta política explica, em linguagem simples, quais dados o app LM Mission coleta, por que precisa desses dados, onde eles ficam armazenados e como você pode controlá-los.

**1. Dados que coletamos**
- Dados da conta: nome, sobrenome, email, data de nascimento, país, status de verificação do email e última data de login. Esses dados são usados para criar e manter sua conta.
- Dados de missão e configurações (armazenados no seu aparelho): planos de missão, pernas, configuração de carga (pallets), alocação de assentos, contagens e pesos de tripulação e passageiros, equipamentos e preferências (sistema de unidades, pesos padrão). Esses itens ficam salvos localmente para que você possa voltar às suas missões.
- Nomes de tripulantes customizados que você preencher nas configurações: são salvos localmente nas preferências do app.

Observação: o app não armazena nomes de passageiros por padrão — apenas contagens, pesos e a alocação de assentos (posição). Senhas nunca são armazenadas em texto pelo app.

**2. Por que coletamos esses dados**
- Conta e email: para permitir login, verificação de email e associar suas missões ao seu usuário.
- Dados de missão e configurações: para salvar, carregar e editar suas missões, calcular o centro de gravidade (CG) e permitir uso offline.

**3. Onde os dados são guardados**
- Perfil de usuário (nome, email, data de nascimento, país, etc.): copiado para o serviço de backend (Firebase/Firestore) para que sua conta exista centralmente e possa ser recuperada em outro dispositivo.
- Sessão e perfil em cache: uma cópia segura do perfil é guardada localmente em armazenamento seguro do aparelho (Keychain no iOS / Keystore no Android) para permitir login offline.
- Configurações e missões: salvas localmente no aparelho usando as preferências do sistema (SharedPreferences). Essas informações normalmente não são enviadas para servidores externos.

**4. Sincronização e acesso à rede**
- O app usa serviços de autenticação e banco de dados em nuvem (Firebase). Quando você cria conta, faz login ou usa funcionalidades que sincronizam perfil, seus dados de conta são transmitidos para os servidores do provedor de autenticação e banco de dados.
- O app também ativa persistência offline do banco de dados para melhorar a experiência sem rede.

**5. Segurança**
- Dados sensíveis de sessão e perfil são guardados localmente de forma protegida pelo armazenamento seguro do aparelho.
- As comunicações com o serviço de backend usam a infraestrutura segura do provedor (transmissão segura). A app não guarda sua senha em texto claro; o provedor de autenticação trata das credenciais.

**6. Compartilhamento e terceiros**
- Não vendemos seus dados.
- Não usamos serviços de rastreamento ou analytics integrados ao app (nenhum tracker de terceiros ativo). Os únicos serviços externos utilizados são os serviços de autenticação e banco de dados em nuvem necessários para o funcionamento (por exemplo, Firebase).

**7. Tempo de retenção**
- Sessão offline: o app mantém uma sessão em cache por até 30 dias a partir do último login para permitir o uso offline. Depois disso, será necessário login online novamente.
- Perfil no servidor: permanece enquanto sua conta existir no serviço de backend (Firestore), até que a conta seja excluída.

**8. Seus direitos e opções**
- Visualizar e editar: você pode acessar e editar seus dados de perfil pelo app (página de perfil/settings), quando a funcionalidade estiver disponível.
- Sair / limpar sessão local: ao fazer logout, o app remove a sessão segura do aparelho. Desinstalar o app também remove os dados locais (dependendo do sistema operacional).
- Excluir conta no servidor: caso deseje que seu perfil seja removido dos servidores, verifique se o app oferece essa opção na página de perfil; caso não exista uma função explícita, procure o contato do desenvolvedor na loja onde baixou o app para solicitar remoção.

**9. Crianças**
O app não é voltado especificamente para crianças. Se você for responsável por uma conta de menor, por favor gerencie o consentimento e o uso conforme aplicável em sua jurisdição.

**10. Alterações nesta política**
Podemos atualizar esta política para refletir mudanças no app. Quando houver alterações importantes, informaremos uma data de atualização no topo deste documento.

**11. Perguntas e contato**
Se tiver dúvidas sobre como seus dados são usados ou se quiser pedir a remoção, procure o canal de suporte indicado na página do aplicativo na loja onde baixou o LM Mission.

---
Este resumo foi gerado a partir das funcionalidades do app (autenticação com conta, uso de Firestore, armazenamento seguro local, SharedPreferences para configurações e missões). Se desejar, posso adaptar o texto incluindo detalhes de contato ou cláusulas legais específicas para sua organização.
