# 📱 Sprint 3 - Mobile

[![React Native](https://img.shields.io/badge/React%20Native-0.74-blue?logo=react)](https://reactnative.dev/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.x-blue?logo=typescript)](https://www.typescriptlang.org/)
[![Expo](https://img.shields.io/badge/Expo-managed%20workflow-black?logo=expo)](https://expo.dev/)
[![Status](https://img.shields.io/badge/status-em%20desenvolvimento-yellow)](#)

Aplicativo mobile desenvolvido como parte da **Sprint 3**.  
O projeto foi feito com **React Native + TypeScript** e possui fluxo completo de autenticação, registro, listagem e edição de usuários, utilizando `AsyncStorage` como persistência local.

---

## 🚀 Funcionalidades

- **Login de usuário** com validação de e-mail e senha.
- **Cadastro de usuário** (nome, e-mail, senha e avatar).
- **Perfil do usuário** com informações e opção de logout.
- **Lista de usuários** com navegação para perfis individuais.
- **Edição de usuário** (nome, e-mail, senha e avatar).
- **Persistência de dados** usando `AsyncStorage`.
- **Navegação customizada** (`RouterProvider`) sem dependência de bibliotecas externas.
- **Componentes reutilizáveis** (`Button`, `Input`, `Card`, `H1`, `AppHeader`).
- **Tema centralizado** com tokens de cor e estilo.

---

## 📂 Estrutura do Projeto

```bash
AppNome/
├── app/                     # (futuro uso com expo-router)
├── src/
│   ├── screens/             # Telas do app
│   │   ├── LoginScreen.tsx
│   │   ├── RegisterScreen.tsx
│   │   ├── ProfileScreen.tsx
│   │   ├── UsersListScreen.tsx
│   │   └── EditUserScreen.tsx
│   ├── components/          # Componentes reutilizáveis
│   │   ├── Button.tsx
│   │   ├── Card.tsx
│   │   ├── Input.tsx
│   │   ├── H1.tsx
│   │   └── AppHeader.tsx
│   ├── layout/              # Estrutura de tela
│   │   └── Screen.tsx
│   ├── services/            # Regras de negócio / acesso a dados
│   │   ├── storage/
│   │   │   └── asyncStorage.ts
│   │   ├── repositories/
│   │   │   └── userRepository.ts
│   │   └── sessionService.ts
│   ├── utils/               # Funções utilitárias
│   │   ├── id.ts
│   │   └── validations.ts
│   ├── theme/               # Estilos e cores globais
│   │   └── tokens.ts
│   ├── types/               # Definições de tipos
│   │   └── user.ts
│   ├── navigation/          # Roteador customizado
│   │   └── router.tsx
│   └── app.tsx              # Composição do app (estado de rotas)
├── App.tsx                  # Reexporta src/app.tsx
└── package.json
