| Этап | Тип события | Название|
|---|---|---|
Добавление товара в корзину | domain | ProductAdd
Подтверждение заказа  | domain  | GoodsVerify
Отсутствие товара на складе  | failure | GoodsVerifyException
Удаление товара из корзины  | compensation | ProductRemove
Отсутствие ответа по таймауту  | Timeout | GoodsVerifyTimeout
Успешная Оплата | domain | PurchaseSuccess
Ошибка при оплате | failure | PurchaseError
Таймаут оплаты | Timeout | PurchaseTimeout
Очистка корзины | compensation | BasketCancel
Заявка на доставку | domain | DeliveryOrder
Уведомление о необходимости подготовить товар | domain | DeliveryNotification