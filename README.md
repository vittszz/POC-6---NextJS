# POC-6---NextJS
Projeto assentos cinema

Cinema Seat Reservation
Este é um projeto de sistema de reservas de assentos para cinemas, desenvolvido em React com suporte a modo claro e escuro e interface responsiva para dispositivos móveis. Ele permite selecionar assentos, alternar entre temas claro/escuro e ajustar automaticamente o layout para diferentes tamanhos de tela.

Funcionalidades
Seleção de Assentos:

Os assentos podem ser selecionados clicando sobre eles.
Os assentos indisponíveis estão desativados e visualmente destacados.
O preço total da compra é calculado com base nos assentos selecionados.
Modo Claro/Escuro:

Um botão no cabeçalho permite alternar entre o modo claro e escuro.
As cores do layout se ajustam automaticamente com base no tema selecionado.
Responsividade:

O layout é adaptado para funcionar bem em desktops, tablets e dispositivos móveis.
O grid de assentos ajusta o número de colunas de acordo com o tamanho da tela.
Compra Simulada:

Um botão de "Comprar" exibe uma mensagem simulando a confirmação da compra.
Tecnologias Utilizadas
React: Para construir a interface do usuário.
Tailwind CSS: Para estilização e responsividade.
CSS Custom Properties: Para definir temas claros e escuros com variáveis CSS.
Como Executar o Projeto
Pré-requisitos
Ter o Node.js instalado na sua máquina.
Um gerenciador de pacotes como npm ou yarn.
Instalação
Clone este repositório:

bash
Copiar código
git clone https://github.com/seu-usuario/cinema-seat-reservation.git
cd cinema-seat-reservation
Instale as dependências do projeto:

bash
Copiar código
npm install
Inicie o servidor de desenvolvimento:

bash
Copiar código
npm start
Acesse o projeto em http://localhost:3000.

Estrutura do Projeto
kotlin
Copiar código
src/
├── components/
│   └── CinemaSeats.js    # Componente principal do sistema de assentos
├── pages/
│   └── globals.css       # Estilos globais do projeto
├── data/
│   └── movie.json        # Dados do filme
└── App.js                # Entrada principal do React
Explicação dos Principais Arquivos
CinemaSeats.js
Responsável por:
Exibir o grid de assentos.
Lidar com a seleção de assentos.
Calcular o total do preço da compra.
Alternar entre os modos claro e escuro.
globals.css
Contém:
Variáveis para o tema claro e escuro (--background, --foreground).
Estilos para tornar o layout responsivo.
Configurações para o grid de assentos e botões.
movie.json
Exemplo de dados do filme, com informações como:
Título.
Horário de exibição.
Descrição.
Preço por assento.
Disponibilidade dos assentos.
Estilos e Responsividade
Modo Claro e Escuro:

As cores de fundo e texto são definidas usando as variáveis CSS:
--background: Cor de fundo.
--foreground: Cor do texto.
A classe dark no elemento <html> ativa o tema escuro.
Responsividade:

O grid de assentos usa CSS Grid e ajusta o número de colunas com base no tamanho da tela:
Desktop: 10 colunas.
Tablet: 5 colunas.
Mobile: 4 colunas.
Comportamento das Funcionalidades
Seleção de Assentos
Clicando em um assento disponível, ele é selecionado e marcado visualmente.
Clicando novamente no assento, ele é desmarcado.
Os assentos indisponíveis não podem ser clicados.
Botão de Compra
Mostra o preço total com base nos assentos selecionados.
Caso nenhum assento seja selecionado, o valor exibido será R$ 0.00.
Tema Claro/Escuro
O botão no cabeçalho alterna entre os dois temas.
A classe dark é adicionada ou removida do <html> dinamicamente.
Melhorias Futuras
Implementar autenticação para reserva de assentos.
Salvar as seleções no armazenamento local ou em um backend.
Adicionar uma animação ao alternar entre os temas.
Contribuição
Contribuições são bem-vindas! Siga os passos abaixo:

Faça um fork do repositório.
Crie uma nova branch:
bash
Copiar código
git checkout -b minha-nova-feature
Commit suas mudanças:
bash
Copiar código
git commit -m "Minha nova feature"
Faça o push para a branch:
bash
Copiar código
git push origin minha-nova-feature
Abra um Pull Request.
