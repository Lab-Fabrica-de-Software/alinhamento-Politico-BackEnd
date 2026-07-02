# 🚀  Alinhamento Político
Uma plataforma digital que conecta eleitores e políticos, permitindo o posicionamento em temas relevantes e destacando o nível de alinhamento entre ambos.

## 📖 Visão Geral
- **Problema e Objetivo:** A falta de transparência e conexão entre eleitores e políticos dificulta o entendimento das prioridades sociais. O objetivo é criar uma plataforma que permita interação direta, posicionamento em temas e análise de alinhamento político.

- **Público-Alvo e Benefícios:** Voltada para eleitores, políticos e organizações, oferece maior transparência, engajamento e insights estratégicos sobre as preferências da sociedade.

## 📋 Funcionalidades Principais
- ✅ **Cadastro e Autenticação:** Registro de eleitores e políticos com verificação de identidade.
- ✅ **Levantamento e Agrupamento de Temas:** Eleitores sugerem temas organizados por categorias (economia, saúde, segurança, educação, diversidade etc.).
- ✅ **Posicionamento Público:** Eleitores e políticos podem se posicionar a favor ou contra os temas levantados.
- ✅ **Análise de Alinhamento:** Algoritmos calculam o grau de alinhamento entre eleitores e políticos.
- ✅ **Visualização de Dados:** Dashboards interativos mostram temas mais relevantes por região e categoria.

## 🛠️ Tecnologias Utilizadas
Java, AWS, Spring-Boot

## 📦 Bibliotecas Principais  
Spring-Boot

## 📂 Estrutura do Projeto
```bash
├── AlinhamentoApplication     # Ponto de entrada Spring Boot
├── infrastructure        # TUDO relacionado à AWS e configs globais
|   ├── aws               # Pasta para todo e qualquer codigo referente a AWS
|   |   ├── config        # Inicialização dos Clientes SDK da AWS
|   |   ├── s3            # Upload/Download de arquivos
|   |   ├── sqs           # Mensageria/Filas (ex: evento de User criado)
|   |   ├── secret        # Integração com Secrets Manager ou Parameter Store
|   ├── security          # Segurança (ex: Cognito ou JWT)
├── modules               # Onde ficam os módulos de negócio
|   ├── users             # Módulo de Usuário isolado
|       ├── Controllers   # Entrada HTTP (REST/API Gateway)
|       ├── Dtos          # Request/Response Data Transfer Objects
|       ├── Entity        # Entidades de banco de dados
|       ├── Mapper        # Conversão (Entity <-> DTO)
|       ├── Repository    # Interfaces de acesso a dados
|       ├── Services      # Regras de negócio puras
|   ├── politico          # Módulo de usuarios politicos isolado
|
| 
```


> O storybook será iniciado em: [http://localhost:6006/](http://localhost:6006/)

Lab-Fábrica de Software • 2025
