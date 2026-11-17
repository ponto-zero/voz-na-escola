# VozNaEscola

PWA para canal de escuta e acolhimento da comunidade escolar.

## Recursos
- Envio de denúncia anônima ou identificada.
- Categorias: bullying, ameaças, violência, assédio, discriminação, danos ao patrimônio e outros.
- Protocolo + chave privada para acompanhamento; consulta pública retorna somente o status.
- Painel da equipe com login, lista de relatos, status e notas internas.
- Dados sensíveis em schema privado, com RLS ativa.

## Supabase
Projeto: rigwsunmsigsdheblffj (sa-east-1). URL e chave publicável estão no frontend. A chave publicável pode ficar no navegador. Nunca coloque a service_role key no frontend ou no GitHub.

## Ativação do painel
1. Crie os usuários da equipe em Authentication > Users.
2. Copie o UUID do profissional autorizado e execute no SQL Editor:
   insert into private.school_staff (user_id, full_name) values ('UUID-DO-USUARIO', 'Nome do profissional');

## Importante
Antes de receber relatos reais, a direção deve aprovar o fluxo, definir responsáveis e horários de monitoramento, informar a comunidade sobre privacidade e retenção dos dados e validar as obrigações legais aplicáveis, inclusive proteção de crianças e adolescentes. Esta primeira versão não possui CAPTCHA nem garantia de monitoramento em tempo real e não é um canal de emergência. Em risco imediato, procure um adulto/equipe responsável ou os serviços de emergência.
