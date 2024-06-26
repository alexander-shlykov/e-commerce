### Задания на проект:
1. Ответить на следующие вопросы:

   1.1. Сколько у нас пользователей, которые совершили покупку только один раз?

   1.2. Сколько заказов в месяц в среднем не доставляется по разным причинам? Вывести детализацию по причинам.

   1.3. По каждому товару определить, в какой день недели товар чаще всего покупается.

   1.4. Сколько у каждого из пользователей в среднем покупок в неделю (по месяцам)?
   
2. Провести когортный анализ пользователей и определить когорту с самым высоким retention в период с января по декабрь 2017 года.

3. Построение RFM-сегментации пользователей.

________________________________________________________

Описание данных: 

**df_customers (таблица с уникальными идентификаторами пользователей):**  
*customer_id* — позаказный идентификатор пользователя  
*customer_unique_id* —  уникальный идентификатор пользователя  (аналог номера паспорта)  
*customer_zip_code_prefix* —  почтовый индекс пользователя  
*customer_city* —  город доставки пользователя  
*customer_state* —  штат доставки пользователя 

**df_order_items (товарные позиции, входящие в заказы):**  
*order_id* —  уникальный идентификатор заказа (номер чека)  
*order_item_id* —  идентификатор товара внутри одного заказа  
*product_id* —  ид товара (аналог штрихкода)  
*seller_id* — ид производителя товара  
*shipping_limit_date* —  максимальная дата доставки продавцом для передачи заказа партнеру по логистике  
*price* —  цена за единицу товара  
*freight_value* —  вес товара  

**df_orders (таблица заказов):**  
*order_id* —  уникальный идентификатор заказа (номер чека)  
*customer_id* —  позаказный идентификатор пользователя  
*order_status* —  статус заказа  
*order_purchase_timestamp* —  время создания заказа  
*order_approved_at* —  время подтверждения оплаты заказа  
*order_delivered_carrier_date* —  время передачи заказа в логистическую службу  
*order_delivered_customer_date* —  время доставки заказа  
*order_estimated_delivery_date* —  обещанная дата доставки
