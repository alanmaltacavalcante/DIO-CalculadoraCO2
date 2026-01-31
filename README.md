# 🌿 Calculadora de CO₂ - Brasil

<div align="center">

![License](https://img.shields.io/badge/license-MIT-green)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)

**Calculadora de Emissões de CO₂ para Transportes no Brasil**

[Demo ao Vivo](https://alanmaltacavalcante.github.io/DIO-CalculadoraCO2/)

</div>

---

## 📋 Sobre o Projeto

Este projeto foi desenvolvido como **Trabalho de Conclusão do Bootcamp GitHub Copilot - Código na Prática** da [DIO.me](https://dio.me), demonstrando o uso de IA generativa no desenvolvimento de aplicações web modernas.

A **Calculadora de CO₂** é uma aplicação web que permite calcular as emissões de dióxido de carbono geradas por diferentes meios de transporte em rotas brasileiras, ajudando usuários a tomar decisões mais sustentáveis sobre seus deslocamentos.

### ✨ Características Principais

- 🚴 **4 Modos de Transporte**: Bicicleta, Carro, Ônibus e Caminhão
- 🗺️ **52 Rotas Pré-configuradas**: Principais cidades brasileiras
- 🔄 **Busca Bidirecional**: Rotas funcionam em ambas as direções
- 💰 **Cálculo de Créditos de Carbono**: Estimativa de preços em BRL
- 📊 **Comparação Inteligente**: Ranking de eco-eficiência
- 🎨 **Design Liquid Glass**: Interface moderna com glassmorphism
- 📱 **Totalmente Responsivo**: Funciona em todos os dispositivos
- ⚡ **Zero Dependências**: Vanilla JavaScript puro

---

## 🎯 Funcionalidades

### Cálculo de Emissões
- Cálculo preciso baseado em fatores de emissão por km
- Comparação automática com baseline de carro
- Exibição de economia potencial de CO₂

### Créditos de Carbono
- Conversão automática para créditos (1 crédito = 1000kg CO₂)
- Estimativa de preços em Reais (R$ 50-150 por crédito)
- Valores mínimo, médio e máximo

### Rotas Brasileiras
- 52 rotas pré-configuradas entre capitais e cidades principais
- Auto-preenchimento de distância ao selecionar origem/destino
- Opção de entrada manual para rotas personalizadas

---

## 🚀 Tecnologias Utilizadas

### Frontend
- **HTML5**: Estrutura semântica
- **CSS3**: Estilização avançada com glassmorphism
- **JavaScript (ES6+)**: Lógica de aplicação

### Design
- **Liquid Glass Design System**: Efeitos de vidro líquido
- **Dark Theme**: Paleta de cores escura e moderna
- **Glassmorphism**: Blur forte (20-25px) e transparências
- **Font Awesome**: Ícones vetoriais
- **Google Fonts (Inter)**: Tipografia moderna

### DevOps
- **GitHub Pages**: Hospedagem estática
- **GitHub Actions**: Deploy automático

---

## 📦 Estrutura do Projeto

```
CalculadoraCO2/
├── .github/
│   └── workflows/
│       └── deploy.yml          # Workflow de deploy automático
├── css/
│   └── style.css               # Estilos liquid glass
├── js/
│   ├── app.js                  # Orquestração da aplicação
│   ├── calculator.js           # Lógica de cálculo de CO₂
│   ├── config.js               # Fatores de emissão e configurações
│   ├── routes-data.js          # Banco de dados de rotas
│   └── ui.js                   # Renderização de componentes
├── index.html                  # Página principal
├── .gitignore                  # Arquivos ignorados pelo Git
└── README.md                   # Este arquivo
```

---

## 🎨 Design System

### Paleta de Cores

```css
/* Background */
--bg-dark: #0a1929
--bg-dark-secondary: #1e293b

/* Accents */
--primary: #22c55e (Verde eco-friendly)
--accent: #4ade80 (Verde claro)
--info: #3b82f6 (Azul)

/* Text */
--text: #f1f5f9 (Branco)
--text-light: #cbd5e1 (Cinza claro)
```

### Efeitos Glass

- **Blur**: 20-25px (backdrop-filter)
- **Transparência**: rgba(255, 255, 255, 0.08-0.15)
- **Bordas**: rgba(255, 255, 255, 0.2-0.4)
- **Sombras**: Multicamadas para profundidade

---

## 🌍 Fatores de Emissão

| Transporte | Emissão (kg CO₂/km) | Ícone |
|------------|---------------------|-------|
| 🚴 Bicicleta | 0.00 | Emissão zero |
| 🚗 Carro | 0.12 | Baseline de comparação |
| 🚌 Ônibus | 0.089 | 25.8% mais eficiente |
| 🚛 Caminhão | 0.96 | Carga pesada |

---

## 💻 Como Usar

### Opção 1: Acessar Online
Acesse a [versão hospedada no GitHub Pages](#) (disponível após o deploy)

### Opção 2: Executar Localmente

1. **Clone o repositório**
```bash
git clone https://github.com/seu-usuario/CalculadoraCO2.git
cd CalculadoraCO2
```

2. **Abra no navegador**
```bash
# Abrir diretamente no navegador
open index.html

---

## 📖 Como Funciona

### 1. Selecione Origem e Destino
Escolha entre 52 rotas pré-configuradas de cidades brasileiras

### 2. Escolha o Meio de Transporte
Selecione entre Bicicleta, Carro, Ônibus ou Caminhão

### 3. Calcule as Emissões
Clique em "Calcular Emissões" para ver:
- Emissão total de CO₂ (kg)
- Comparação com outros transportes
- Créditos de carbono necessários
- Estimativa de preços em BRL

### 4. Tome Decisões Sustentáveis
Use as informações para escolher o meio de transporte mais eco-friendly!

---

## 🗺️ Rotas Disponíveis

### Principais Capitais
- São Paulo ↔ Rio de Janeiro (430 km)
- São Paulo ↔ Belo Horizonte (586 km)
- São Paulo ↔ Curitiba (408 km)
- Rio de Janeiro ↔ Belo Horizonte (434 km)
- Brasília ↔ Goiânia (209 km)

### Regiões Cobertas
- ✅ Sudeste (16 rotas)
- ✅ Sul (12 rotas)
- ✅ Centro-Oeste (8 rotas)
- ✅ Nordeste (10 rotas)
- ✅ Norte (6 rotas)

**Total**: 52 rotas bidirecionais entre as principais cidades brasileiras

---

## 🛠️ Desenvolvimento

### Arquitetura

O projeto segue uma arquitetura modular baseada em objetos globais:

```javascript
// Módulos principais
Calculator  // Cálculos de emissão e créditos
CONFIG      // Configurações e fatores de emissão
RoutesDB    // Banco de dados de rotas
UI          // Renderização de componentes
```

### Padrões de Código

- **ES6+**: Arrow functions, template literals, destructuring
- **Modular**: Separação clara de responsabilidades
- **Documentado**: JSDoc em funções principais
- **Semântico**: HTML5 semântico e BEM-like CSS

### Commits Semânticos

Este projeto segue o padrão [Conventional Commits](https://www.conventionalcommits.org/):

```
feat: nova funcionalidade
fix: correção de bug
style: mudanças de estilo/UI
docs: documentação
chore: tarefas de manutenção
ci: integração contínua
```

---

## 🚀 Deploy

O projeto é automaticamente deployado no GitHub Pages via GitHub Actions sempre que há push na branch `main`.

### Workflow de Deploy

```yaml
# .github/workflows/deploy.yml
on:
  push:
    branches: [main]
```

O site fica disponível em: `https://seu-usuario.github.io/CalculadoraCO2`

---

## 🤝 Contribuindo

Contribuições são bem-vindas! Siga estes passos:

1. Fork o projeto
2. Crie uma branch para sua feature (`git checkout -b feat/nova-feature`)
3. Commit suas mudanças (`git commit -m 'feat: adiciona nova feature'`)
4. Push para a branch (`git push origin feat/nova-feature`)
5. Abra um Pull Request

---

## 📝 Licença

Este projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

---

## 👨‍💻 Autor

Desenvolvido como projeto de conclusão do **Bootcamp GitHub Copilot - Código na Prática** da [DIO.me](https://dio.me)

### Bootcamp
- **Instituição**: Digital Innovation One (DIO.me)
- **Curso**: GitHub Copilot - Código na Prática
- **Ano**: 2026

### Tecnologias Aprendidas
- ✅ GitHub Copilot para desenvolvimento assistido por IA
- ✅ Boas práticas de versionamento com Git
- ✅ Conventional Commits
- ✅ GitHub Actions e CI/CD
- ✅ Deploy automático com GitHub Pages
- ✅ Desenvolvimento web moderno (HTML5/CSS3/JS ES6+)

---

## 🌟 Agradecimentos

- [DIO.me](https://dio.me) pela oportunidade do bootcamp
- [Font Awesome](https://fontawesome.com) pelos ícones
- [Google Fonts](https://fonts.google.com) pela fonte Inter
- Comunidade open source por inspiração e recursos

---

<div align="center">

**⭐ Se este projeto foi útil, considere dar uma estrela!**

Feito com 💚 e ♻️ para um futuro mais sustentável

</div>
