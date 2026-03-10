# 🗺️ Mapa Colaborativo de Cidades do Brasil

O **Mapa Colaborativo de Cidades do Brasil** é uma aplicação web interativa criada para permitir que usuários selecionem cidades brasileiras e as adicionem a um mapa compartilhado em tempo real. O projeto combina formulários dinâmicos, serviços de geolocalização, banco de dados em nuvem e visualização cartográfica para construir uma experiência simples, visual e colaborativa.

A proposta é facilitar a marcação de localidades no território brasileiro, organizando a escolha por **região**, **estado** e **cidade**, e exibindo os pontos no mapa conforme são adicionados.

## ✨ Funcionalidades

- Seleção hierárquica de localidade por:
  - região
  - estado
  - cidade
- Integração com a API do **IBGE** para carregamento de regiões, estados e municípios
- Geolocalização automática da cidade selecionada
- Marcação da cidade em mapa interativo
- Atualização em tempo real dos pontos adicionados
- Armazenamento compartilhado em nuvem com **Firebase Firestore**
- Autenticação automática do usuário
- Feedback visual para sucesso, erro e carregamento
- Interface responsiva com painel lateral e mapa expandido

## 🛠️ Tecnologias Utilizadas

- **HTML5**
- **CSS3**
- **JavaScript**
- **Tailwind CSS**
- **Leaflet.js**
- **Firebase Authentication**
- **Firebase Firestore**
- **API de Localidades do IBGE**
- **Nominatim / OpenStreetMap**

## 🎯 Objetivo do Projeto

O projeto foi desenvolvido para oferecer uma ferramenta simples e colaborativa de marcação geográfica, podendo ser utilizada em:

- atividades educacionais;
- visualização de participação por cidades;
- mapeamento colaborativo de localidades;
- registro de presença geográfica;
- projetos de extensão, pesquisa ou eventos.

## ⚙️ Como funciona

A aplicação segue este fluxo:

1. O usuário escolhe uma **região** do Brasil.
2. O sistema carrega os **estados** daquela região.
3. Após a seleção do estado, o sistema carrega as **cidades** correspondentes.
4. Ao enviar o formulário, a cidade é geolocalizada com base em serviços do OpenStreetMap.
5. A localização é salva no **Firestore**.
6. O mapa é atualizado em tempo real com um novo marcador.

## ▶️ Como usar

1. Abra a aplicação em um navegador moderno.
2. Escolha uma **região**.
3. Selecione um **estado**.
4. Escolha uma **cidade**.
5. Clique em **Marcar no Mapa**.
6. Aguarde a confirmação e visualize a cidade adicionada ao mapa.

## 🌍 Recursos do mapa

O mapa utiliza a biblioteca **Leaflet.js** com base cartográfica do **OpenStreetMap**, oferecendo:

- navegação fluida;
- zoom interativo;
- marcadores personalizados;
- popups com nome da cidade e estado.

## 🔄 Atualização em tempo real

As localidades adicionadas ficam armazenadas em um banco de dados na nuvem e são escutadas em tempo real. Isso significa que novos pontos aparecem automaticamente no mapa sem necessidade de recarregar a página.

## 🧩 Estrutura da Interface

A aplicação está dividida em duas áreas principais:

- **Painel lateral**: formulário de seleção e mensagens de feedback
- **Mapa principal**: exibição visual dos marcadores das cidades

## 🔐 Integração com Firebase

O projeto utiliza:

- **Firebase Authentication** para autenticação automática do usuário
- **Cloud Firestore** para armazenar e sincronizar as cidades marcadas

Essa integração permite colaboração entre diferentes usuários na mesma aplicação.

## 📱 Responsividade

A interface foi adaptada para funcionar em:

- computadores
- tablets
- celulares

Em telas maiores, o formulário e o mapa aparecem lado a lado; em telas menores, os elementos se reorganizam verticalmente.

## 📁 Estrutura do Projeto

O projeto está concentrado em um único arquivo HTML com:

- **HTML**: estrutura da interface
- **CSS**: personalização visual e ajustes do mapa
- **JavaScript**: lógica de formulários, chamadas de API, autenticação, persistência e renderização dos marcadores

## ✅ Possíveis usos

Este projeto pode ser utilizado como:

- mapa colaborativo de participantes;
- ferramenta educacional sobre geografia do Brasil;
- recurso para projetos de extensão;
- visualização de origem de usuários;
- base para sistemas maiores de mapeamento colaborativo.

## 📄 Licença

Este projeto pode ser utilizado para fins educacionais, institucionais e experimentais.
