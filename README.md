# Projeto-DesenvolvimentoDeSistemas-2 TG1
## Cenário de negócio / Concepção:
### 1. Problema ou oportunidade percebida:

A biblioteca faz todo o controle de empréstimos manualmente, em fichas de papel.

Isso gera atrasos, perda de informações e dificuldade para acompanhar disponibilidade dos livros.

Oportunidade: informatizar o processo para aumentar a eficiência e confiabilidade.

### 2. Razão ou justificativa para esta demanda:

Reduzir erros de controle (como livros que “somem” do acervo).

Agilizar o processo de empréstimo e devolução.

Permitir relatórios que ajudem na gestão do acervo.

Melhorar a experiência do usuário (consultar disponibilidade de livros facilmente).

### 3. Descrição sucinta do produto de software:

Um sistema web simples que permite:

Cadastro de usuários (leitores).

Cadastro de livros.

Registro de empréstimos e devoluções.

Emissão de relatórios (livros mais emprestados, usuários com livros em atraso).

(Opcional) Notificação de atraso por e-mail/SMS.

### 4. Clientes, usuários e demais envolvidos/impactados:

Clientes: a gestão da biblioteca comunitária.

Usuários finais:

Bibliotecário (administra cadastros, empréstimos e relatórios).

Leitores/usuários (consultam livros e realizam empréstimos/devoluções).

Envolvidos indiretos:

Comunidade do bairro (beneficiada por uma biblioteca mais organizada).

Fornecedor de tecnologia (quem dará suporte/manutenção ao sistema).

### 5. Principais critérios de qualidade do produto:

Usabilidade: fácil de usar, interface intuitiva.

Confiabilidade: não perder registros de empréstimos.

Disponibilidade: sistema deve estar acessível sempre que a biblioteca funcionar.

Desempenho: consultas rápidas sobre disponibilidade de livros.

Segurança: evitar acesso não autorizado a cadastros e dados pessoais.

## Modelo de caso de uso:
### 1. Identificação de casos de uso de negócio por ator:

Bibliotecário:

Cadastrar usuário.

Cadastrar livro.

Registrar empréstimo.

Registrar devolução.

Gerar relatórios.

Leitor:

Consultar disponibilidade de livro.

Realizar empréstimo/devolução.

Sistema de Notificação (opcional):

Enviar aviso de atraso.

### 2. Casos de uso descritos de forma resumida:

Cadastrar usuário: registrar dados do leitor no sistema.

Cadastrar livro: inserir informações de um novo livro no acervo.

Consultar disponibilidade: verificar se um livro está emprestado ou disponível.

Registrar empréstimo: associar um livro a um leitor e definir prazo de devolução.

Registrar devolução: marcar o livro como devolvido e liberar para novo empréstimo.

Gerar relatórios: obter informações gerenciais sobre acervo e usuários.

Notificar atraso: enviar aviso ao usuário sobre devolução vencida.

### 3. Caso de uso crítico (detalhado): Registrar Empréstimo

#### Ator principal: Bibliotecário.

#### Objetivo: Registrar o empréstimo de um livro para um leitor.

#### Pré-condições:

O usuário já está cadastrado.

O livro já está cadastrado e disponível.

#### Fluxo principal de eventos:

O bibliotecário acessa a função "Registrar empréstimo".

O sistema solicita a identificação do usuário (leitor).

O bibliotecário seleciona o livro desejado.

O sistema verifica se o livro está disponível.

O sistema registra o empréstimo, define data de devolução e salva no histórico.

O sistema emite um comprovante (digital ou impresso).

#### Fluxos alternativos:

3a. Se o livro não estiver disponível, o sistema informa ao bibliotecário.

2a. Se o usuário não estiver cadastrado, o sistema solicita cadastro antes de prosseguir.

Pós-condições:

O livro passa para o estado "emprestado".

O usuário fica associado a este empréstimo até a devolução.
