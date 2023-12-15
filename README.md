# Projeto criado com Remix!

- [Remix Docs](https://remix.run/docs)

## No ARQUIVO .env

Atribuir valores nas variaveis SMTP_USER e SMTP_PASS

- SMTP_USER: E-mail do g-mail que será utilizado para disparar os e-mails transacionais.
- SMTP_PASS: Senha da aplicação criada no painel de segurança do g-mail

Senha de Apps: https://myaccount.google.com/apppasswords

## No terminal, dentro da pasta do projeto:

### Dependencias

Instalar dependências com NPM

```sh
npm install
```

### Artefatos do banco

Para criar os artefatos das entidades
```sh
npx prisma generate
```

Para criar ou modificar banco conforme arquivo prisma/schema.prisma
```sh
npx prisma db push
```

### Desenvolvimento

Para iniciar a aplicação no modo de desenvolvimento:
```sh
npm run dev
```

### Deployment

Criar um build para Produção

```sh
npm run build
```

Rodar projeto em produção

```sh
npm start
```

### Dados

**Substitua os valores em MAIÚSCULO por infomações reais**

Para inserir um novo usuário no banco

```sql
INSERT INTO Usuario
(email, senha, nome, apartamento, bloco)
VALUES('EMAIL DO USUÁRIO', 'SENHA DO USUÁRIO CRITOGRAFADA COM MD5', 'NOME DO USUÁRIO', 'APARTAMENTO DO USUÁRIO', 'BLOCO DO USUÁRIO');
```
MD5 Generator: https://www.md5hashgenerator.com/

Para inserir um novo usuário no banco

INFORMAÇÃO DE LOCAL PRIVADO: 
- 1 para Privado
- 0 para Público
  
```sql
INSERT INTO Ambiente
(id, nome, ambiente_privado)
VALUES('NOME DO ESPACO', 'INFORMAÇÃO DE LOCAL PRIVADO');
```