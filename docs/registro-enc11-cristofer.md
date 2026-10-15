Folha de registro — Encontro de 15/10
Arquitetura de Software SAAS · o CampoConta rodando
Nome: _Cristofer Mateus Rutzen_  
O que é: o seu registro dos seis experimentos (frente) e o primeiro desenho dos serviços do seu produto (verso). O que não é: prova. Os comandos estão em experimentos.md, no repositório.
☐ Frente: a resposta de abertura e as seis previsões, cada uma escrita ANTES de rodar.
☐ Verso: as caixas do seu produto e as quatro respostas.
☐ Verso fotografado antes de entregar a folha ao professor.
Não entra aqui: comando copiado, saída do terminal colada.
Abertura (2 min, sem consulta). O que é um microsserviço? E o que muda nele quando o produto é multi-tenant?
O microsserviço é um componente autônomo, desacoplado e focado em um único domínio de negócio, 
que possui seu próprio ciclo de deploy, escala independentemente e gerencia sua própria base de dados persistente. Ele muda quando o produto é multi-tenant pois todo o ciclo de vida da requisição 
e do dado precisa ser isolado por inquilino (tenant). As requisições exigem contexto de identificação (ex.: tenant_id via cabeçalhos/tokens JWT) e as operações de 
banco/armazenamento precisam garantir segregação lógica ou física para impedir vazamento de dados entre clientes distintos.

Os seis experimentos. Previsão antes do sinal; "O que saiu", depois de rodar; "O nome disso", com o professor, no fim de cada experimento.
Experimento	Minha previsão	O que saiu	O nome disso
1 — Seguir uma requisição			
2 — A Buricá tenta ver o dado da Alvorada			
3 — O relatório da diretoria			
4 — A cobrança sai do ar			
5 — O mesmo evento chega duas vezes			
6 — O vizinho barulhento			

No fim do encontro (2 min). Releia a sua resposta de abertura e reescreva:


Verso — agora o seu produto
É o produto que a sua equipe propôs no começo do semestre e vai defender em 29/10, na Etapa 2, com dois serviços no ar. O CampoConta não é o seu projeto: use o formato do desenho, não a divisão dele.
1. As caixas. Desenhe a porta de entrada, os dois serviços e onde cada um guarda dado. Ponha uma seta para cada conversa entre eles.


2. Quatro respostas, uma linha cada. "Ainda não sei" vale, desde que escrito: vira a sua primeira pendência até 29/10.
a) Qual é o segundo serviço, e o que ele recebe do primeiro?


b) Onde o tenant é descoberto, e como chega ao segundo serviço?


c) Se alguém esquecer o filtro no código, o que segura o vazamento?


d) Se o segundo serviço cair, o que o usuário ainda consegue fazer?


Em casa, até sábado, 17/10, 23h59: passe este verso para o arquivo docs/servicos-rascunho.md no repositório do seu projeto: salve a foto do desenho na pasta docs/, 
cite o nome dela no arquivo e digite as quatro respostas. Faça o commit e o push. Um arquivo por projeto: se o projeto é de dupla, cada um faz o commit com as respostas combinadas. 
É o rascunho do ADR de comunicação que a Etapa 2 pede.
