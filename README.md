# SIGGO
## Aplicação gerenciamento de RH

### Demonstração
Caso queira testar o aplicativo online, vá para o link: [https://immense-escarpment-11106.herokuapp.com](https://immense-escarpment-11106.herokuapp.com).<br>

### Parte externa do site
- Página inicial estática, com informações sobre a empresa. A princípio eu coloquei informações sobre o que pode ser feito e tudo mais, mas tudo isso pode ser alterado pra que tudo fique com logo da sua empresa, informações daí e tudo mais.
- Login pode ser feito com e-mail ou nome de usuário cadastrado pelo usuário, o que este achar mais conveniente
- Parte interna do site (área exclusiva a usuários cadastrados)

### Níveis de usuários:
- Candidato: <br>
Acesso apenas ao próprio perfil e mensagens <br>
Atualização de informações, envio de documentos e envio/recebimento de mensagens internas; <br>
- Funcionário: Tudo que o "Candidato" tem acesso, além de:  <br>
Visualização e edição do próprio perfil, envio de documentos para serem anexados ao seu perfil <br>
Adição de registros de folha de ponto restritos aos últimos 7 dias (visualização ilimitada, porém após passados 7 dias o funcionário não pode mais alterar informações - esse limite pode ser alterado) <br>
Pedido de férias <br>
Visualização de holerites <br>
- Gerente: Tudo que o "Funcionário" tem acesso, além de:  <br>
Acesso aos perfis de funcionários da sua mesma unidade (local de trabalho).  <br>
Edição de outros usuários em campos que eles não podem alterar, como cargo, nível de acesso, entre outros.  <br>
Enviar ou remover holerites de funcionários que estejam na mesma unidade que ele mesmo <br>
Alterar folha de ponto de mais de 7 dias atrás, já que o próprio funcionário não tem esse poder <br>
- Administrador: Tudo que o "Gerente" tem acesso, além de:  <br>
Acesso a todos os perfis de todos os funcionários <br>
Acesso a holerites de todos os funcionários <br>
Acesso a folhas de ponto de todos os funcionários <br>

### Funcionalidades adicionais
- Modo noturno no site disponível para maior conforto do usuário que desejar habilitar essa opção
Todas as funcionalidades podem ser acessadas pelo celular. O site foi projetado para funcionar perfeitamente em qualquer tamanho de tela, seja celular, tablet, notebook ou telas maiores.
- Apenas administrador ou gerente podem cadastrar novos funcionários. O cadastro pede informações básicas e uma senha inicial para o novo funcionário/candidato. Após entrar no perfil, o novo funcionário/candidato pode (e deve) alterar sua senha.
Usuário pode atualizar o perfil com sua foto
- Envio de arquivos de PDF e imagens para serem anexados ao perfil do usuário
- Envio de holerite em PDF para cada funcionário. Pode também ser enviado em formato .png ou .jpg, por computador, celular, tablet, entre outros. O limite do tamanho do arquivo é de 10mb (também pode ser alterado caso ache necessário).
- Adição de folha de ponto por cada funcionário. No momento habilitei a edição para os últimos 7 dias, mas isso pode ser restrito ao dia atual, por exemplo.
- Geração de relatório de dias e horas trabalhadas por funcionário e por local de trabalho, com possibilidade de exportação para Excel, cópia ou impressão em apenas um clique
- Geração de folha com todas as marcações de folha de ponto de cada funcionário com linha para assinatura após cada marcação, para que o funcionário possa assinar ao final do mês e entregar ao RH
- Ao serem realizados requerimentos de férias, tanto usuário quanto gerentes (da mesma unidade) e administradores gerais receberão uma mensagem automática, para que analisem.

### Informações adicionais de segurança:
- Todos os arquivos enviados ao site são criptografados e armazenados na nuvem da Amazon. Os links para visualização expiram após 5 minutos que a página foi aberta. Isso possibilta maior segurança aos dados. Após este tempo basta recarregar a página que um novo link é gerado e o arquivo pode ser acessado automaticamente, sem que o usuário perceba.
- As senhas dos usuários também são criptografadas. Nem administrador nem quem tem acesso ao banco de dados tem acesso às senhas, que são armazenadas através do que é chamado de "hash". Um exemplo é a senha '123456', que está armazenada no banco de dados como "$2a$11$NRgCPQZWSI5gU64FB/aJ2uHYWIcetg6oLTxYYX.02B8S6CPDE59la". Isso é muito importante para a segurança das informações.
- O site possui certificado de segurança SSL, que permite a comunicação criptografada entre um site e um navegador, oferecendo mais uma camada de segurança.


### Este programa é gratuito/código aberto?

Não, já que foi criado para que empresas consigam ganhar dinheiro de forma mais rápida e eficiente! O repositório privado, que contém o código (proprietário e fechado) atualizado, está concluído. A versão do link [aqui](https://immense-escarpment-11106.herokuapp.com) está atualizada com a última versão

#### Dados técnicos

Linguagens de programação: Ruby, HTML5, CSS3, SCSS, Javascript, Coffeescript<br>
Framework: Ruby on Rails<br>
Banco de dados utilizado: PostgreSQL<br>

## Para mais informações: 

* Autor: André de Souza Lima
* E-mail: andre.szlima1@gmail.com / andreszlima@ufrn.edu.br
* Instagram: www.instagram.com/andreszlima
* Twitter: www.twitter.com/andreszlima
