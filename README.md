# 🌐 IPv4 Subnet Intelligence Platform (Steel & Saffron Edition)

[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)](https://developer.mozilla.org/pt-BR/docs/Web/HTML)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=flat-square&logo=tailwind-css&logoColor=white)](https://tailwindcss.com/)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=flat-square)](LICENSE)

Uma plataforma didática e interativa de engenharia de redes para **cálculo, planejamento, análise e auditoria de sub-redes IPv4**. Desenvolvida com a estética **Steel & Saffron** inspirada no design prático de IDEs profissionais (com alto contraste em temas Claro e Escuro), o aplicativo oferece processamento reativo em tempo real para alunos, professores e profissionais de redes.

---

## 📸 Recursos em Destaque

- ⚡ **Cálculo Reativo em Tempo Real:** Atualização instantânea dos parâmetros ao digitar o IP ou alterar o prefixo CIDR.
- 🎯 **Dimensionador Reverso por Hosts:** Digite a quantidade de dispositivos e receba a indicação do menor prefixo `/CIDR` ideal.
- 🔒 **Diagnóstico de Escopo e Segurança (RFC 1918):** Identificação automática de IPs Privados, Públicos, Loopback (`127.0.0.1`), APIPA (`169.254.x.x`) ou Multicast.
- 🛠️ **Máscara Coringa (Wildcard):** Cálculo da máscara invertida utilizada em ACLs Cisco e protocolos como OSPF.
- 🧠 **Fluxo Lógico e Método do Número Mágico:** Visualização do salto ($256 - \text{octeto}$) e das operações binárias *Bitwise AND*.
- 🏛️ **Tabela Histórica de Classes (Classful A-E):** Referência detalhada com padrões de bits iniciais e faixas RFC 1918.
- ✍️ **Exercícios Práticos com Gabarito Expansível:** Exercícios resolvidos com passo a passo para certficações (CCNA/CompTIA Network+).
- 📄 **Exportação Exata para PDF:** Formatação dedicada para impressão e salvamento em relatório PDF sem poluentes visuais.

---

## 📊 Parâmetros Calculados

Ao informar um IP e um prefixo CIDR, o sistema calcula e exibe:

| Parâmetro | Descrição |
| :--- | :--- |
| **Máscara Decimal** | Formato pontilhado de 32 bits (ex: `255.255.255.192`) |
| **Máscara Coringa (Wildcard)** | Inverso binário da máscara (ex: `0.0.0.63`) |
| **ID da Rede (Network ID)** | Endereço de identificação do segmento de rede |
| **Endereço de Broadcast** | Endereço de difusão de pacotes para todos os hosts |
| **Faixa de IPs Úteis** | Intervalo atribuível a hosts utilizáveis (`Primeiro IP` ao `Último IP`) |
| **Total de IPs / Hosts Úteis** | Quantidade total ($2^H$) e utilizáveis ($2^H - 2$) |
| **Decomposição Binária** | Conversão em base 2 do IP, da Máscara e do Network ID |

---

## 🚀 Como Executar o Projeto

Como a aplicação é **100% Client-Side** (Single File Architecture), não há necessidade de Node.js, compilação ou instalação de dependências.

### Opção 1: Abrir diretamente no navegador
1. Clone o repositório ou baixe os arquivos:
   ```bash
   git clone https://github.com/seu-usuario/ipv4-subnet-intelligence.git
   ```
2. Abra o arquivo `index.html` em qualquer navegador moderno (Chrome, Edge, Firefox, Safari).

### Opção 2: Servidor Local (Live Server no VS Code)
1. Abra a pasta do projeto no VS Code.
2. Com a extensão **Live Server** instalada, clique com o botão direito no `index.html` e selecione **Open with Live Server**.

---

## 🎨 Paleta de Cores (Steel & Saffron)

A interface utiliza uma combinação de tons cinzas frios combinados com destaque em amarelo açafrão:

```
 Hexagonal: #2A2F35 | #5B6770 | #F2C14E | #FFF4D6 | #9AA5B1
```

- **Cinza Aço Escuro (`#2A2F35`):** Fundo principal e barras estruturais.
- **Cinza Aço Médio (`#5B6770`):** Cards, contornos e tabelas.
- **Amarelo Açafrão (`#F2C14E`):** Botões primários e dados em destaque.
- **Creme Soft (`#FFF4D6`):** Fundo do tema claro e textos com excelente contraste visual.

---

## 🛠️ Tecnologias Utilizadas

- **HTML5:** Estruturação semântica e acessível.
- **Tailwind CSS (via CDN):** Estilização utilitária e responsiva.
- **JavaScript (Vanilla ES6+):** Algoritmos de cálculo binário, manipuladores de bits e interatividade com o DOM.

---

## 📜 Licença

Este projeto está licenciado sob a licença **MIT** - consulte o arquivo [LICENSE](LICENSE) para obter mais detalhes.

---

<p align="center">
  Desenvolvido para fins de ensino e engenharia de redes IPv4. 🚀
</p>