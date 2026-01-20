# MachTeam 🥋

MachTeam é um aplicativo mobile desenvolvido em Flutter para gerenciamento de ensino de artes marciais, especialmente focado em Jiu-Jitsu. A plataforma conecta professores e alunos, permitindo o compartilhamento de técnicas, gerenciamento de turmas e acompanhamento do progresso dos estudantes.

## 📱 Funcionalidades

### Para Professores
- **Gerenciamento de Turmas**: Criação e administração de múltiplas turmas
- **Cadastro de Técnicas**: Upload de vídeos com descrições e passos detalhados
- **Área Técnica**: 
  - Técnicas Gerais (sistema unificado)
  - Habilidades Técnicas por módulo (com múltiplas aulas por habilidade)
- **Gestão de Alunos**: Adicionar, remover e acompanhar alunos
- **Sistema de Conquistas**: Atribuição de faixas e medalhas
- **Notificações Push**: Comunicação direta com alunos

### Para Alunos
- **Acesso a Técnicas**: Visualização de vídeos em tela cheia
- **Aulas Organizadas**: Conteúdo dividido por módulos e habilidades
- **Progresso Pessoal**: Acompanhamento de conquistas e evolução
- **Interface Intuitiva**: Design moderno com tema escuro

### Recursos do Sistema
- **Autenticação Firebase**: Login seguro para professores e alunos
- **Cloud Storage**: Armazenamento de vídeos e imagens
- **Firestore Database**: Dados em tempo real
- **Video Player**: Reprodução com controles de play/pause e tela cheia
- **Notificações**: Sistema de push notifications

## 🚀 Tecnologias

- **Framework**: Flutter 3.x
- **Linguagem**: Dart
- **Backend**: Firebase
  - Authentication
  - Cloud Firestore
  - Cloud Storage
  - Cloud Functions
  - Firebase Messaging
- **Arquitetura**: Clean Architecture com separação de camadas
- **State Management**: StatefulWidget + Provider pattern

## 📋 Pré-requisitos

- Flutter SDK (versão 3.0 ou superior)
- Android Studio / Xcode (para desenvolvimento)
- Conta Firebase configurada
- Dart SDK

## 📁 Estrutura do Projeto

```
lib/
├── main.dart                 # Entry point
├── firebase_options.dart     # Configurações Firebase
├── models/                   # Modelos de dados
│   ├── tecnica.dart
│   ├── habilidade_tecnica.dart
│   ├── aula_tecnica.dart
│   └── ...
├── services/                 # Serviços e lógica de negócio
│   ├── tecnica_service.dart
│   ├── habilidade_tecnica_service.dart
│   ├── notification_service.dart
│   └── ...
├── screens/                  # Telas do aplicativo
│   ├── aluno/               # Área do aluno
│   │   ├── home_aluno.dart
│   │   └── widgets/
│   └── professor/           # Área do professor
│       ├── home_professor.dart
│       └── widgets/
├── widgets/                  # Widgets reutilizáveis
│   └── fullscreen_video_player.dart
└── utils/                    # Utilitários
    └── app_snack_bar.dart
```

## 🔐 Configuração de Segurança

### Firestore Rules
As regras de segurança garantem que:
- Usuários só acessem seus próprios dados
- Professores controlem suas turmas e técnicas
- Alunos visualizem apenas conteúdo autorizado

### Storage Rules
Controle de upload de vídeos:
- Professores podem fazer upload (máx. 100MB)
- Apenas vídeos em formato MP4
- Path estruturado: `habilidades/{habilidadeId}/{aulaId}.mp4`

## 🎨 UI/UX

- **Tema**: Escuro com gradientes roxo/azul
- **Cores principais**: 
  - Primary: `#8B5CF6` (Purple)
  - Secondary: `#6366F1` (Indigo)
  - Accent: Orange
- **Tipografia**: Roboto/SF Pro
- **Componentes**: Material Design 3

## 📱 Plataformas Suportadas

- ✅ Android
- ✅ iOS

## 🧪 Testes

```bash
# Análise de código
flutter analyze

# Testes unitários
flutter test

# Build de produção
flutter build apk --release  # Android
flutter build ios --release  # iOS
```

## 📦 Build de Produção

### Android
```bash
flutter build apk --release
# ou
flutter build appbundle --release
```

### iOS
```bash
flutter build ios --release
```

## 🤝 Contribuindo

1. Fork o projeto
2. Crie uma branch para sua feature (`git checkout -b feature/AmazingFeature`)
3. Commit suas mudanças (`git commit -m 'Add some AmazingFeature'`)
4. Push para a branch (`git push origin feature/AmazingFeature`)
5. Abra um Pull Request

## 📝 Licença

Este projeto está sob a licença MIT. Veja o arquivo `LICENSE` para mais detalhes.

## 👥 Autores

- **Equipe MachTeam** - *Desenvolvimento inicial*

## 🙏 Agradecimentos

- Comunidade Flutter
- Firebase Team
- Contribuidores do projeto

## 📞 Suporte

Para suporte, envie um email para nullnod@gmail.com ou abra uma issue no GitHub.

---

**Desenvolvido com ❤️ por Fagales Software**
