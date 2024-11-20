# cbea-cloud
Arquitetura para um sistema em nuvem para a Confederação Brasileira de Esportes Aquáticos

Precisamos propor uma arquitetura para um sistema em nuvem para a Confederação Brasileira de Esportes Aquáticos identificando inicialmente a seguinte realidade:

1. A CBEA precisa manter um cadastro de todos os campeonatos de natação realizados. Para isto, utiliza atualmente uma ficha em papel para cada campeonato. Nesta ficha consta o ano em que o campeonato será realizado, um número sequencial do campeonato neste ano, uma data de início, uma data de término e o local em que será realizado.

2. A CBEA também mantém um cadastro de todas as pessoas inscritas na Confederação, cada qual com um número único de matrícula, sejam elas treinadores, sejam nadadores.

2.1. Para os nadadores é mantida a data de inscrição, o nome, o e-mail, diversos telefones, diversos endereços, cada qual com a indicação da rua, número e complemento, sua data de nascimento, o número de medalhas de ouro, prata e bronze que obteve, o número de campeonatos de que já participou e seu sexo.

2.2. Para os treinadores é mantida a data de inscrição, o nome, seu e-mail, diversos telefones, diversos endereços, cada qual com a indicação da rua, número e complemento, sua formação e o número de títulos que obteve.

3. Todo o inscrito está associado a uma equipe, identificada por um código e possuindo um nome, uma data de fundação, um número de títulos e um número de campeonatos disputados.

4. Todas as provas possíveis em um campeonato de natação serão previamente cadastradas (por exemplo: 200m nado de peito masculino).

4.1. Para isto, é necessário cadastrar os estilos (borboleta, costas, peito, livre, medley e revezamento), que receberão um código único e um nome.

4.2. Cada prova é de um estilo e possui uma distância e o sexo dos nadadores, além de um código único.

4.3. Para cada prova são mantidos diversos recordes, identificados por um código sequencial na prova e possuindo uma data, uma descrição e um tempo.

5. Cada campeonato inclui diversas das provas que são previamente cadastradas e, obviamente, a mesma prova pode ser disputada em diversos campeonatos.

6. Cada nadador disputa diversas provas do campeonato e uma prova do campeonato, obviamente, pode reunir diversos nadadores.

6.1. Cada prova do campeonato é disputada em uma determinada data, em uma bateria classificatória e uma final.

6.2. Logo, cada nadador poderá nadar duas vezes a mesma prova, uma para classificar-se (pela manhã classificam-se os 8 primeiros para a final à tarde – mas isto é
irrelevante em nosso contexto –) e outra valendo medalhas.

6.3. Para cada uma das vezes em que nada uma prova do campeonato (classificatória e final), o nadador recebe um tempo e uma classificação.
