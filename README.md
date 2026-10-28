# AgrogestorBACK

## Estado em 27/10/2026

Este repositório ainda não contém servidor próprio ou esquema de negócio.
Cadastro, login e sessões do frontend são integrados ao Supabase Auth.
Projeto AgroGestor informado: `cijujvueodmjifvlqfxm`.

O Supabase Auth já persiste usuários e credenciais com sua infraestrutura de
autenticação. Não duplicar senhas em tabelas públicas. Papéis privilegiados
devem ser atribuídos pelo servidor em `app_metadata`, nunca por campos livres
do formulário de cadastro ou `user_metadata`.

Para os módulos de gestão, ainda será necessário definir tabelas, vínculos por
propriedade, migrações versionadas e políticas RLS. Inspecionar o esquema atual
antes de aplicar mudanças. Não foi criada migração nem alterado banco nesta etapa.

Configuração do aplicativo, testes e diagnóstico estão em `AgrogestorFRONT`.

## Validação para publicação na main

Este commit é documental. Não existe manifest de aplicação, servidor ou suíte
de testes neste repositório. O plugin Supabase ainda retorna falta de permissão
para consultar o projeto; a API pública de autenticação está disponível.
A implementação operacional dos módulos de negócio continua pendente.

Consulte o [status consolidado no frontend](https://github.com/jpedro00/AgrogestorFRONT/blob/main/docs/STATUS.md).
