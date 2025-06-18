# TrabalhoRequisitos2

Trabalho Final – Engenharia de Requisitos II
Projeto: Plataforma para Conexão de Professores Particulares e Alunos
a) Definição do Problema e Escopo do Produto
Descrição Geral da Ideia do Sistema
A plataforma tem como objetivo conectar professores particulares e alunos de forma prática e eficiente, funcionando como um "iFood de professores". Nela, professores podem oferecer aulas ao vivo ou gravadas, organizar sua agenda e receber pagamentos. Alunos podem encontrar profissionais com base em filtros personalizados, agendar aulas, assistir a conteúdos e realizar pagamentos diretamente pela plataforma.

Objetivos Principais
Facilitar a conexão entre alunos e professores.

Oferecer uma agenda interativa para controle de horários e aulas.

Disponibilizar videoaulas e conteúdos complementares.

Automatizar pagamentos e permitir avaliações públicas.

Criar uma experiência similar a marketplaces modernos, como iFood ou Airbnb, porém voltada à educação.

Escopo (O que estará incluído no produto de software)
Cadastro de usuários: professores e alunos.

Criação de perfil profissional com especialidades, valor/hora e currículo.

Sistema de busca e filtros por matéria, preço, idioma, avaliação e disponibilidade.

Agenda interativa para marcação de aulas.

Upload de aulas gravadas e materiais complementares.

Sistema de aula ao vivo com integração externa ou nativa.

Sistema de pagamento seguro e automatizado.

Sistema de avaliação e comentários de alunos.

Notificações automáticas por e-mail ou push.

Interface web responsiva para desktop e dispositivos móveis.

b) Levantamento de Requisitos
Técnicas Utilizadas
Entrevista simulada com stakeholders (professores e alunos).

Brainstorming com equipe de desenvolvimento.

Observação indireta de plataformas similares (Superprof, Udemy, iFood, Airbnb).

Resumo da Entrevista (Simulada)
Professores relataram dificuldades com organização de horários, múltiplas plataformas de comunicação, cobrança de pagamentos e exposição online. Querem um sistema centralizado, simples de usar e com controle total sobre seus serviços.

Alunos relataram dificuldade em encontrar professores confiáveis, comparar preços, conteúdos e realizar pagamentos com segurança. Desejam uma experiência fluida, onde consigam agendar e consumir aulas com poucos cliques.

Resumo do Brainstorming
Durante o brainstorming, ficou evidente a importância de:

Um sistema unificado para comunicação, organização e transações.

Dashboards adaptados a cada perfil (professor/aluno).

Interface simples e com foco em acessibilidade.

Possibilidade de aula ao vivo + conteúdos sob demanda.

Notificações automatizadas para compromissos e atualizações.

Registro dos Requisitos Coletados
Cadastro de professores e alunos com perfis completos.

Sistema de busca com filtros por especialidade, idioma, nota, valor e disponibilidade.

Agenda digital com sincronização entre ambas as partes.

Aula ao vivo integrada com ferramenta de vídeo.

Upload e visualização de conteúdos gravados.

Dashboard com indicadores personalizados (agendas, pagamentos, avaliações).

Avaliações públicas de professores por parte dos alunos.

Integração com meios de pagamento (Pix, cartão, boleto).

Notificações automáticas por e-mail/push.

Interface intuitiva e responsiva para múltiplas plataformas.

c) Classificação e Organização dos Requisitos
Requisitos Funcionais (RF)
Código	Descrição
RF01	Permitir cadastro de professores e alunos.
RF02	Permitir que professores editem seu perfil profissional.
RF03	Permitir que alunos filtrem professores por critérios específicos.
RF04	Permitir agendamento de aulas com base na disponibilidade dos professores.
RF05	Permitir integração com sistemas de videoconferência para aulas ao vivo.
RF06	Permitir upload e visualização de aulas gravadas e materiais.
RF07	Permitir a realização de pagamentos pela plataforma.
RF08	Exibir avaliações e comentários dos alunos sobre os professores.
RF09	Enviar notificações automáticas sobre aulas, pagamentos e novidades.
RF10	Apresentar dashboards distintos para professores e alunos.

Requisitos Não Funcionais (versão expandida)
Código	Descrição
RNF01	O sistema deve ser responsivo, funcionando em desktop, tablets e smartphones.
RNF02	O tempo de resposta para ações do usuário deve ser de no máximo 3 segundos.
RNF03	Os dados sensíveis devem ser protegidos por criptografia (TLS/SSL e armazenamento criptografado).
RNF04	A plataforma deve ser escalável, suportando o crescimento no número de usuários simultâneos.
RNF05	O sistema deve estar disponível pelo menos 99% do tempo (alta disponibilidade).
RNF06	A interface deve ser intuitiva, simples e acessível para usuários com diferentes níveis de experiência.
RNF07	O sistema deve seguir as normas de acessibilidade (WCAG 2.1 nível AA, por exemplo).
RNF08	O sistema deve suportar internacionalização para possibilitar diferentes idiomas no futuro.
RNF09	O sistema deve ser compatível com os principais navegadores modernos (Chrome, Firefox, Safari, Edge).
RNF10	Os pagamentos devem ser processados via gateway seguro com certificações PCI-DSS.
RNF11	O sistema deve realizar backups automáticos diários dos dados essenciais.
RNF12	O sistema deve permitir autenticação segura, com política de senhas e possibilidade de autenticação em dois fatores (2FA).
RNF13	O sistema deve ser modular, facilitando manutenção e atualizações futuras.
RNF14	O tempo de inatividade para manutenção não programada não pode ultrapassar 1 hora por mês.

📊 Matriz de Rastreabilidade dos Requisitos
A matriz abaixo faz o mapeamento entre os requisitos funcionais (RF), os requisitos não funcionais (RNF), e os objetivos do sistema (OBJ), facilitando a rastreabilidade:

Código	Descrição do Requisito	Objetivo(s) Relacionado(s)	RNF Relacionado(s)
RF01  -Cadastro de professores e alunos	-OBJ1, OBJ2-	RNF01, RNF03, RNF06
RF02	-Edição de perfil profissional por professores	-OBJ2, OBJ4	-RNF01, RNF06
RF03	-Busca de professores com filtros	-OBJ1, OBJ5	-RNF01, RNF02, RNF06
RF04	-Agendamento de aulas	-OBJ2, OBJ3-	RNF01, RNF02, RNF05
RF05	-Aulas ao vivo (vídeo)	-OBJ3	-RNF01, RNF02, RNF09
RF06	-Upload e acesso a conteúdos gravados	-OBJ3, OBJ4-	RNF01, RNF04, RNF11
RF07	-Pagamentos pela plataforma	-OBJ4-	RNF03, RNF10, RNF12
RF08	-Avaliações e comentários	-OBJ5	-RNF01, RNF06
RF09	-Notificações automáticas	-OBJ2, OBJ3	-RNF01, RNF06
RF10	-Dashboards personalizados	-OBJ2, OBJ4-	RNF01, RNF02, RNF13

Legenda de Objetivos (OBJ):

OBJ1: Facilitar a conexão entre alunos e professores.

OBJ2: Oferecer uma agenda interativa para controle de horários.

OBJ3: Disponibilizar videoaulas e conteúdos complementares.

OBJ4: Automatizar pagamentos e organização da rotina docente.

OBJ5: Permitir avaliações e promover transparência.


