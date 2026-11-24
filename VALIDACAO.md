# Validação técnica

## Verificações realizadas nesta entrega
- `node --check server.js`: aprovado.
- `node --check db.js`: aprovado.
- `node --check public/script.js`: aprovado.
- Estrutura SQLite revisada: clientes, produtos, movimentos e itens de movimento.
- Persistência implementada no arquivo SQLite local (`banco.db`), criado na inicialização.
- CRUD de clientes e produtos ligado à API; vendas registradas em transação e estoque atualizado.

## Teste funcional recomendado após instalar dependências
1. Execute `npm install` e `npm start`.
2. Cadastre um cliente e um produto.
3. Feche o servidor com Ctrl+C e execute `npm start` novamente.
4. Confirme que cliente e produto continuam listados.
5. Edite e exclua registros e confirme a atualização na interface.
6. Faça uma venda e confira o movimento e a baixa do estoque.

A execução integrada com `sqlite3` não pôde ser concluída neste ambiente porque a instalação da dependência excedeu o limite de tempo. Portanto, não afirmamos que o teste de reinicialização foi executado aqui; os comandos de sintaxe foram aprovados e a persistência está implementada no código.
