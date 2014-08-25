select current_user()

select * from pedido

select status
     , sum(valor_total) total_vendas
 from pedido
 group by status

select date(data_criacao) 
     , sum(valor_total)
  from pedido
  where status = 'EMITIDO'
  group by date(data_criacao)
