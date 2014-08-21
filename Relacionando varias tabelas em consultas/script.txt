select current_user()

select * from cliente
select * from pedido

insert into produto (nome, valor_unitario, quantidade_estoque) 
 values('Papel A4', 12.00, 100)

insert into pedido (data_criacao, data_entrega, valor_frete, valor_total, cliente_id)
 values ('2014-07-11 15:22:00', '2014-07-15', 33.00, 400.00, 2)

insert into item_pedido (pedido_id, produto_id, quantidade)
 values (4, 1, 4)

insert into item_pedido (pedido_id, produto_id, quantidade)
 values (4, 2, 2)

select * from pedido 

select p.*
  from pedido p
     , cliente c
  where p.cliente_id = c.id
    and c.nome = 'João Silva'
    
select * from cliente 
select * from pedido
select * from item_pedido
select * from produto

select pr.nome
     , i.quantidade
  from cliente c
     , pedido pe
     , item_pedido i
     , produto pr
  where c.id = pe.cliente_id
    and pe.id = i.pedido_id
    and i.produto_id = pr.id
    and c.nome = 'Maria Santos'     
 



 

 
