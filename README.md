🐾 VetCare — Hospital Veterinário e Centro Diagnóstico

Aplicação web desenvolvida para a VetCare, uma clínica veterinária e centro diagnóstico fictício. O projeto foi construído focando em boas práticas de front-end, semântica, acessibilidade, arquitetura CSS modular e responsividade.

📌 Sumário

Visão Geral e Objetivo

Tecnologias e Conceitos Aplicados

Arquitetura de Arquivos

Instruções de Execução

Funcionalidades e Especificações

Principais Desafios Técnicos e Aprendizados

Licença e Autoria

🩺 Visão Geral e Objetivo

O objetivo deste projeto é simular o desenvolvimento front-end em um cenário profissional, entregando uma landing page responsiva, moderna e acessível para a VetCare.

A aplicação apresenta a estrutura da clínica, corpo clínico, especialidades, horários de funcionamento, perguntas frequentes (FAQ) e canal de contato direto via WhatsApp.

🛠️ Tecnologias e Conceitos Aplicados

HTML5 Semântico: Estruturação utilizando tags como <header>, <nav>, <main>, <section>, <article>, <details>, <summary> e <footer>, garantindo acessibilidade e SEO.

CSS3 Moderno:

Design System & CSS Tokens (:root): Padronização de cores, tipografia, espaçamentos, bordas e sombras através de variáveis CSS.

Metodologia BEM (Block Element Modifier): Padrão de nomenclatura rigoroso para classes (.card, .card__title, .card--highlighted).

Escala REM e Unidades Relativas: Uso de porcentagem no elemento raiz (html { font-size: 62.5%; }), unidades rem para tipografia e espaçamentos, e %, vw, vh para layouts fluídos.

Flexbox Layout: Organização e alinhamento responsivo de componentes e cards.

Google Fonts: Importação e aplicação da família tipográfica Poppins (pesos 400, 500, 600 e 700).

API do WhatsApp: Integração de botão flutuante direcionado ao atendimento oficial.

Responsividade (Mobile First / Breakpoints): Adaptação para smartphones, tablets e desktops via @media queries.

📂 Arquitetura de Arquivos

A arquitetura adota a separação rigorosa de responsabilidades, sem estilos inline ou blocos <style> internos no HTML.

vetcare-hospital/
├── assets/
│   ├── css/
│   │   ├── variables.css   # Tokens de Design System (:root)
│   │   ├── reset.css       # Normalização de estilos globais
│   │   ├── components.css  # Componentes reutilizáveis (botões, cards, etc.)
│   │   └── style.css       # Estilos estruturais e media queries
│   └── images/             # Recortes e imagens do projeto
├── index.html              # Estrutura HTML5 da aplicação
└── README.md               # Documentação oficial do projeto


🚀 Instruções de Execução

Não é necessário instalar dependências ou executadores de scripts para visualizar este projeto.

Clonar o repositório:

git clone https://github.com/seu-usuario/vetcare-hospital.git


Navegar até a pasta do projeto:

cd vetcare-hospital


Executar a aplicação:

Abra o arquivo index.html em qualquer navegador web de sua preferência.

Alternativamente, utilize a extensão Live Server no VS Code para simulação em tempo real.

📋 Funcionalidades e Especificações

Menu Lateral Esquerdo Fixo: Navegação vertical constante no desktop (position: fixed).

Navegação Suave (Smooth Scroll): ROLAGEM suave ao clicar nos links de ancoragem (scroll-behavior: smooth) com compensação de offset.

Seção Hero / Boas-vindas: Apresentação da clínica ocupando a viewport inicial (100vh).

Especialidades Médicas & Corpo Clínico: Exibição em cards interativos com efeitos de elevação e transição em :hover.

Seção FAQ Interativa: Sanfona nativa utilizando <details> e <summary>.

Rodapé Fixo: Informações de copyright e localização fixadas na base (position: fixed).

Botão Flutuante do WhatsApp: Atalho permanente no canto inferior direito conectado ao telefone oficial da Escola SENAI Henrique Lupo.

🎯 Principais Desafios Técnicos e Aprendizados

Ajuste de Âncora e Layout Fixo:

Desafio: Garantir que o menu lateral fixo e o rodapé fixo não cobrissem o conteúdo das seções durante o scroll.

Solução: Aplicação de margens/paddings estratégicos e propriedades de recuo de rolagem (scroll-margin-top / scroll-margin-left).

Adopção da Escala REM Proporcional:

Desafio: Garantir que todos os elementos seguissem uma proporção precisa sem o uso de valores rígidos em pixels.

Solução: Configuração do font-size: 62.5% no html, permitindo a conversão simples de 1rem = 10px para agilidade no desenvolvimento mantendo a acessibilidade do navegador.

Modularização CSS e Nomenclatura BEM:

Desafio: Manter a consistência do CSS sem criar conflitos de especificidade.

Solução: Divisão em arquivos CSS organizados e aplicação rigorosa da convenção .bloco__elemento--modificador.

📝 Licença e Autoria

Desenvolvido por [Seu Nome Aqui] como parte do projeto avaliativo de Front-End (Turma B).

Orientação e requisitos por SENAI Henrique Lupo.