🎥 Cinema Seat Reservation

![image](https://github.com/user-attachments/assets/211f6696-1e0c-436a-8b76-9e6c2fabb0b9)


Este é um projeto interativo de reserva de assentos de cinema, com suporte a modo claro/escuro, interface responsiva e funcionalidades intuitivas, como seleção de assentos e cálculo dinâmico do preço total.

🚀 Funcionalidades

✔️ Seleção Dinâmica de Assentos:

Os usuários podem selecionar ou desmarcar os assentos disponíveis. Assentos já reservados são desativados.

✔️ Cálculo de Preço Automático:

O valor total é atualizado em tempo real com base nos assentos selecionados.

✔️ Modo Claro/Escuro:

Alternância entre dois temas para melhor experiência visual.

✔️ Layout Responsivo:

Adaptação perfeita para dispositivos móveis, tablets e desktops.

🛠️ Tecnologias Utilizadas

React: Construção da interface interativa.

Tailwind CSS: Estilização moderna e responsiva.

CSS Custom Properties: Gerenciamento de temas claro e escuro.

JavaScript: Manipulação de lógica de seleção e cálculo de preço.

🎬 Pré-visualização do Projeto

Modo Claro

![image](https://github.com/user-attachments/assets/cae82cef-f64a-4441-ad79-63d2e74fa10e)


Modo Escuro

![image](https://github.com/user-attachments/assets/84614da6-1f9b-488d-a657-e718eb3dbda0)


📂 Estrutura do Projeto

src/

├── components/

│   └── CinemaSeats.js    # Componente principal para exibição e seleção de assentos

├── pages/

│   └── globals.css       # Estilos globais para o projeto

├── data/

│   └── movie.json        # Dados do filme (exemplo)

└── App.js                # Entrada principal do React

⚙️ Como Executar o Projeto

 Pré-requisitos:
 
  - Node.js instalado (versão 14 ou superior recomendada).

Gerenciador de pacotes como npm ou yarn.


Instale as dependências:

 - bash

 - Copiar código

 - npm install

Inicie o servidor de desenvolvimento:

- bash

- Copiar código

- npm start

Acesse o projeto no navegador:

- text

- Copiar código

http://localhost:3000

🖼️ Funcionalidades em Detalhe

 Seleção de Assentos:
   
- Clique em qualquer assento disponível para selecioná-lo.

- Assentos selecionados serão destacados.

- O sistema desativa os assentos já reservados (cinza escuro).

Exemplo de Seleção:

Modo Claro/Escuro:
   
- Alternância rápida entre os modos através do botão no cabeçalho.

- Tema escuro para ambientes com pouca luz e tema claro para leitura diurna.

Preview:

 Compra Dinâmica:

- O botão "Comprar" exibe o valor total com base nos assentos selecionados.

- Caso nenhum assento esteja selecionado, o valor será R$ 0.00.

Exemplo de Compra:

📱 Responsividade

O layout se adapta automaticamente a diferentes dispositivos:

Dispositivo	Comportamento

- Desktop	Exibe 10 colunas de assentos.

- Tablet	Ajusta para 5 colunas.

- Mobile	Ajusta para 4 colunas.

🛠️ Personalização do Projeto


Dados do Filme:

Os dados do filme são carregados a partir do arquivo movie.json. Exemplo de estrutura:

json :

{
  "title": "A Forja",
  "time": "16:40",
  "description": "Um ano depois de encerrar o ensino médio...",
  "releaseDate": "26 de setembro de 2024",
  "director": "Alex Kendrick",
  "seats": [
    ["available", "available", "unavailable"],
    ["available", "unavailable", "available"]
  ],
  "pricePerSeat": 12.5
}
Temas Claro e Escuro
As cores do tema são definidas em globals.css com as variáveis:

css :

:root {
  --background: #ffffff;
  --foreground: #171717;
}

.dark {
  --background: #0a0a0a;
  --foreground: #ffffff;
}

📚 Melhorias Futuras

✅ Adicionar animações ao alternar temas.

✅ Implementar um backend para persistência de reservas.

✅ Permitir personalização do layout por administrador.



