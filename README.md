01. Identificação de Fluxos Importantes 

1. Fluxo de Adição ao Carrinho
Por que é importante?
Se o cliente não conseguir adicionar produtos ao carrinho, a jornada de compra é interrompida imediatamente. Isso pode ocorrer por erros no botão "Adicionar ao carrinho", problemas de estoque não refletidos corretamente ou falhas no carregamento de informações.
Impacto:

O cliente pode desistir da compra e procurar outra loja.
A empresa perde receita devido a um problema técnico evitável.
A experiência do usuário fica prejudicada, afetando a confiança na marca.
2. Fluxo de Pagamento
Por que é importante?
O pagamento é a etapa final e mais crítica da compra. Se houver erros na validação do cartão, falhas no redirecionamento para o banco ou opções de pagamento limitadas, o cliente pode abandonar a compra.
Impacto:

Taxa de conversão reduzida.
Aumento da frustração do cliente, que pode desistir ou escolher um concorrente.
Possíveis falhas de segurança podem gerar desconfiança na loja.
3. Fluxo de Cálculo de Frete e Entrega
Por que é importante?
Muitos clientes desistem da compra ao ver um frete muito alto ou quando há problemas na exibição do prazo de entrega. Se o cálculo do frete não for transparente ou apresentar erros, isso pode impedir a finalização da compra.
Impacto:

Clientes podem abandonar o carrinho se não obtiverem informações claras sobre o prazo de entrega.
Uma má experiência com prazos irreais pode prejudicar a reputação da loja.
Se o valor do frete for incorreto, a empresa pode arcar com prejuízos ou perder vendas.

4. Fluxo de Cadastro e Recuperação de Senha
Por que é importante?

Muitos sites exigem cadastro antes da compra, e um processo complicado pode afastar clientes.
Se um cliente esquece a senha e não consegue redefini-la rapidamente, pode desistir da compra.
Impacto:

Perda de conversões por frustração na criação da conta.
Clientes podem optar por concorrentes com processos mais simples.
Alto abandono do carrinho por dificuldades no login.
5. Fluxo de Aplicação de Cupons de Desconto
Por que é importante?

Muitos clientes utilizam cupons para decidir pela compra.
Se um cupom não funcionar corretamente ou o site não explicar as regras de uso, o cliente pode desistir.
Impacto:

Clientes podem abandonar o carrinho se não conseguirem o desconto esperado.
Insatisfação que pode levar a reclamações e dano à reputação da loja.
6. Fluxo de Escolha de Forma de Pagamento
Por que é importante?

Muitos clientes preferem pagar de formas específicas (cartão, PIX, boleto, PayPal).
Se a opção desejada não estiver disponível ou apresentar erro, o cliente pode desistir.
Impacto:

Perda de conversões devido à limitação de opções.
Frustração do cliente ao não conseguir finalizar a compra com o meio de pagamento desejado.
7. Fluxo de Checkout
Por que é importante?

O checkout deve ser rápido e sem fricções. Pedir muitas informações ou ter uma interface confusa pode gerar abandono.
Impacto:

Taxa de abandono de carrinho alta.
Perda de clientes que poderiam concluir a compra se o processo fosse mais fluido.
8. Fluxo de Disponibilidade de Produtos
Por que é importante?

Produtos podem aparecer como disponíveis no catálogo, mas estarem indisponíveis ao adicionar ao carrinho ou finalizar o pedido.
Impacto:

Cliente pode se frustrar e desistir de comprar na loja.
Problemas de reputação e confiabilidade da plataforma.
9. Fluxo de Atendimento ao Cliente
Por que é importante?

Durante a jornada de compra, o cliente pode ter dúvidas sobre o produto, pagamento ou entrega.
Se não houver um atendimento ágil e acessível, ele pode abandonar a compra.
Impacto:

Clientes desistem por falta de suporte.
Reclamações podem prejudicar a imagem da empresa.
10. Fluxo de Rastreamento e Pós-venda
Por que é importante?

Após a compra, o cliente espera atualizações sobre o status do pedido.
Se o rastreamento não for claro ou o pedido atrasar sem aviso, pode gerar insatisfação.
Impacto:

Perda de confiança na marca.
Clientes podem evitar compras futuras devido à experiência ruim.

Esses fluxos são essenciais porque impactam diretamente a conversão de vendas e a experiência do usuário. A falha em qualquer um deles pode significar uma grande perda de receita e confiança na marca, perda de vendas e impacto negativo na reputação da loja.

################################################################################################################################################################

Plano de Testes
Adicionar item ao carrinho (POST /carts/add)

Cenário 1: Adicionar um único item válido ao carrinho (esperado: sucesso).
Cenário 2: Adicionar múltiplos itens ao carrinho (esperado: sucesso).
Cenário 3: Tentar adicionar um item com quantidade inválida (esperado: erro).
Cenário 4: Adicionar um item inexistente (esperado: erro).
Atualizar carrinho (PUT /carts/{id})

Cenário 1: Atualizar a quantidade de um item existente no carrinho (esperado: sucesso).
Cenário 2: Reduzir a quantidade de um item até 0 (esperado: erro ou remoção).
Cenário 3: Atualizar um item inexistente (esperado: erro).
Remover item do carrinho (DELETE /carts/{id})

Cenário 1: Remover um item existente do carrinho (esperado: sucesso).
Cenário 2: Remover um item inexistente (esperado: erro).