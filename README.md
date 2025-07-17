Sistema de Ponto Facial – Pai Company LTDA
Este é um sistema de controle de ponto baseado em reconhecimento facial, desenvolvido com foco na automação de registros de entrada, saída e horários de pausa dos funcionários de forma prática, segura e moderna.

🚀 Funcionalidades
📷 Reconhecimento facial em tempo real usando a biblioteca face-api.js.

🧑‍💼 Cadastro de funcionários com coleta de imagens faciais.

⏰ Registro automático de ponto com verificação de horário e controle de atrasos.

📊 Relatórios diários com resumo dos registros.

📩 Envio automático de relatório por e-mail com um clique.

📋 Listagem dos funcionários cadastrados com data de registro.

💻 Tecnologias utilizadas
HTML5, CSS (TailwindCSS) e JavaScript

Face-api.js para reconhecimento facial

LocalStorage para persistência de dados faciais

JS Mailto Link para envio de relatórios via e-mail padrão

⏱️ Lógicas de Registro de Ponto
O sistema reconhece automaticamente a marcação com base no horário:

Horário	Tipo de Registro
07:40 às 08:10	Entrada
11:40 às 12:10	Início do Almoço
12:50 às 13:10	Volta do Almoço
17:20 às 17:40	Saída

Caso o funcionário registre fora do horário correto, o sistema calcula o atraso em minutos e registra junto ao horário.

🧪 Como usar
Abra o arquivo index.html (ou code.html) em um navegador moderno com acesso à câmera.

Cadastre um funcionário clicando em "Cadastrar Funcionário" e posicionando o rosto na frente da câmera.

O sistema reconhecerá automaticamente o funcionário sempre que ele estiver em frente à câmera dentro de um horário válido.

Use o botão de Gerar Relatório para enviar o resumo diário por e-mail.

🛡️ Observações
Todos os dados faciais são armazenados localmente no navegador (localStorage) – não são enviados para servidores.

Para ambientes reais, é recomendado adicionar camadas de segurança, autenticação e backend persistente.

📁 Estrutura do Projeto
scss
Copiar
Editar
📁 SistemaPontoFacial
├── code.html (arquivo principal)
├── face-api.js (CDN)
├── TailwindCSS (CDN)
👨‍💻 Desenvolvedor
João Victor Oliveira Santos
