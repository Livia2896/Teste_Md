### 1.4 Comparativo BD x Aplicação

| Critério | Banco de Dados | Aplicação |
|---|---|---|
| Consistência | Garante que as regras de integridade sejam aplicadas diretamente aos dados, mesmo que existam diferentes aplicações acessando o banco. | Depende de cada aplicação implementar e seguir corretamente as mesmas regras. |
| Segurança | Pode bloquear operações que violem as regras definidas para os dados. | Permite controlar acessos, permissões e validar operações antes de enviá-las ao banco. |
| Performance | Pode ser eficiente quando a regra envolve diretamente os dados e pode ser resolvida em uma única operação. | Pode evitar consultas ao banco quando consegue fazer uma validação antes de enviar a operação. |
| Manutenção | Facilita a alteração de regras que precisam ser aplicadas a várias aplicações, pois ficam centralizadas. | Pode facilitar a organização e os testes da lógica, mas mudanças podem precisar ser feitas em diferentes aplicações. |
| Portabilidade | Pode exigir adaptações quando utiliza recursos específicos do SGBD. | Pode facilitar a mudança de banco quando a lógica não depende diretamente de recursos específicos dele. |
| Controle central da regra | Permite manter uma regra em um único lugar e aplicá-la às diferentes aplicações que acessam o banco. | O controle fica distribuído entre as aplicações, o que pode gerar diferenças na implementação da mesma regra. |
