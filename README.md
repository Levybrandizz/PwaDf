# 🏛️ Participa DF - Solução de Ouvidoria (PWA)

> **Desafio:** 1º Hackathon em Controle Social - Participa DF  
> **Categoria:** Ouvidoria  
> **Status:** 🚀 Versão Final (Candidate Release)

---

## 📺 Demonstração da Solução

**[CLIQUE AQUI PARA ASSISTIR AO VÍDEO DE DEMONSTRAÇÃO (YouTube)]**  
*(Cole aqui o link do seu vídeo "Não Listado" no YouTube, conforme Item 6.5.2-V do Edital. O vídeo deve ter até 7 minutos)*

---

## 🎯 Objetivo e Visão Geral

Esta solução é um **Progressive Web App (PWA)** desenvolvido para democratizar o acesso à Ouvidoria do Distrito Federal. Focada na experiência do usuário (UX/UI) e na inclusão digital, a aplicação resolve os principais atritos do sistema atual: complexidade no cadastro, dependência de conexão estável e falta de acessibilidade.

### Principais Diferenciais:
1.  **🤖 Integração com IZA (IA):** Um chatbot simulado que guia o cidadão e sugere automaticamente a classificação da manifestação (Denúncia, Reclamação, etc) com base no relato.
2.  **📴 Modo Offline (Offline-first):** Graças aos Service Workers, o cidadão pode redigir sua manifestação sem internet. O app salva o rascunho localmente e permite o envio assim que a conexão retorna.
3.  **♿ Acessibilidade Universal:** Menu dedicado (WCAG 2.1 AA) com alto contraste, fonte para dislexia, zoom e integração nativa com **VLibras**.
4.  **🎙️ Multicanalidade:** Suporte nativo para gravação de áudio e captura de vídeo direto pelo navegador, sem necessidade de plugins.

---

## 🛠️ Tecnologias Utilizadas

O projeto foi construído utilizando tecnologias web padrão (Vanilla JS) para garantir leveza, compatibilidade e facilidade de manutenção pelo GDF, sem dependência de frameworks pesados.

*   **Frontend:** HTML5, CSS3 (Variáveis CSS para temas), JavaScript (ES6+).
*   **Framework CSS:** Bootstrap 5.3 (Grid e Componentes).
*   **Mapas:** Leaflet.js (OpenStreetMap) para georreferenciação.
*   **Onboarding:** Driver.js para tutorial interativo.
*   **Armazenamento Local:** LocalStorage e Cache API (Service Workers).
*   **Ícones:** Bootstrap Icons.

---

## 📂 Estrutura de Arquivos

A organização do código prioriza a clareza e separação de responsabilidades:

```text
/
├── index.html          # Estrutura principal (Single Page Application simulada)
├── style.css           # Estilos customizados, temas (Dark/Light) e animações
├── app.js              # Lógica principal, controle de estado, IZA Chatbot e API de Mídia
├── sw.js               # Service Worker para funcionalidade Offline e PWA
├── manifest.json       # Configuração para instalação (Adicionar à Tela Inicial)
├── assets/             # Imagens e recursos estáticos
└── README.md           # Documentação do projeto
