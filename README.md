# 🛒 Plataforma de Ofertas e Classificados

Este repositório documenta a estrutura e a arquitetura de uma plataforma web/mobile focada na publicação, busca e gerenciamento de ofertas de produtos.

## 📋 Sobre o Projeto

A plataforma permite que os usuários criem contas, gerenciem seus dados pessoais e publiquem produtos para venda. Durante a criação da oferta, é possível incluir detalhes como título, descrição, categoria, preço, estado de conservação do item e imagens.

## 🏗️ Arquitetura do Sistema

A aplicação está dividida em quatro nós principais:

### 1. Aplicação Cliente (Frontend)
* **Acesso:** Web e/ou Mobile.
* **Responsabilidade:** Interface do usuário final (Login, Cadastro, Editar Perfil, Publicar Oferta).

### 2. Balanceamento de Carga (Load Balancer)
* **Responsabilidade:** Ponto de entrada das requisições do cliente, distribuindo tráfego.

### 3. Servidores de Aplicação (Backend)
* **Serviço de Autenticação:** Login e emissão de tokens.
* **Serviço de Produtos/Ofertas:** Formulários de "Publicar Oferta".
* **Serviço de Perfil:** Gerencia edição de dados pessoais.

### 4. Persistência de Dados
* **Banco de Dados Relacional (PostgreSQL/MySQL):** Usuários, Ofertas.
* **Armazenamento de Arquivos (AWS S3):** Imagens dos Produtos.

---
*Para mais detalhes, consulte o pdf que está disponível no repositório
