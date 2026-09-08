# PeopleHub — Gestão de funcionários

Painel interno para organizar funcionários por departamento e consultar uma ficha individual.

## O que o painel mostra

- Departamento e função atual;
- Data de admissão e de demissão;
- Histórico de promoções e mudanças de setor;
- Horário de entrada e saída;
- Contatos e documento mascarado;
- Salário mensal;
- Situação: ativo ou desligado.

## Como consultar

1. Abra o arquivo `index.html` em um navegador autorizado pela empresa.
2. Use a busca por nome ou o filtro de departamento.
3. Clique em um funcionário para ver sua ficha completa.

## Como cadastrar ou alterar pessoas

No fim do arquivo `index.html`, localize a lista `const employees = [...]`.

Cada registro segue este formato:

```js
{
  id: 6,
  name: 'Nome da Pessoa',
  department: 'Departamento',
  role: 'Função',
  status: 'Ativo',
  admission: 'dd/mm/aaaa',
  dismissal: '—',
  schedule: '08:00 às 17:00',
  salary: 'R$ 0,00',
  email: 'email@empresa.com',
  phone: '(00) 00000-0000',
  document: '***.000.000-**',
  history: [['dd/mm/aaaa', 'Admissão · Função inicial']]
}
```

## Segurança e privacidade

Este repositório é privado e usa somente registros fictícios de exemplo. Antes de inserir dados reais:

- limite o acesso somente a pessoas autorizadas;
- não armazene senhas, documentos sem máscara, dados bancários ou laudos médicos;
- lembre-se de que o histórico de commits preserva versões antigas dos arquivos;
- prefira um sistema com autenticação, banco de dados criptografado e controle de permissões para dados reais de RH;
- verifique as regras aplicáveis de privacidade, incluindo a LGPD.

> Este protótipo serve para organização visual. Não substitui um sistema de RH seguro.
