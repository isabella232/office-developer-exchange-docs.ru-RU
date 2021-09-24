---
title: Архивация в веб-служб Exchange в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: 78ae179b-ae4f-4f64-911a-e0c70e0fa314
description: Узнайте об архивах в EWS в Exchange.
ms.openlocfilehash: f2ca4cc783556b089b732c75d166b77c0dcd891c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59520229"
---
# <a name="archiving-in-ews-in-exchange"></a>Архивация в веб-служб Exchange в Exchange

Узнайте об архивах в EWS в Exchange.
  
Архивные почтовые ящики — это вторичные почтовые ящики, связанные с пользователем. Архивные почтовые ящики обычно используются для управления ограничениями хранения электронной почты. Например, старые элементы электронной почты могут периодически перемещаться из почтового ящика в архив. 
  
Exchange Online Exchange Online в Office 365 и Exchange Server 2013 г. вводится две новые операции Exchange Web Services (EWS), которые можно использовать для архивации набора почтовых элементов из основного почтового ящика. Архивавка элементов "Входящие" таким образом сохраняет иерархию папок элементов. Кроме того, архивные почтовые ящики теперь можно хранить локально на клиенте или удаленно, в основном непрозрачной для пользователя, используя путь папки, чтобы указать на содержимое архива.
  
## <a name="archiving-operations-in-ews"></a>Операции архивации в EWS

В следующей таблице перечислены операции архивации, введенные в Exchange 2013 г. 
  
|**Имя операции**|**Описание**|
|:-----|:-----|
|[ArchiveItem](https://msdn.microsoft.com/library/1af216b3-13ea-498e-b4fc-23513755d731%28Office.15%29.aspx) <br/> |Перемещает элемент из основного почтового ящика в архивный почтовый ящик.  <br/> |
|[CreateFolderPath](https://msdn.microsoft.com/library/5a10aa5e-3f25-4ec3-a0b9-284c30918a1f%28Office.15%29.aspx) <br/> |Создает URI, который указывает на расположение хранилища для архивного почтового ящика.  <br/> |
   
## <a name="see-also"></a>См. также

- [Разработка клиентов веб-служб для Exchange](develop-web-service-clients-for-exchange.md)
    
- [Начало работы с веб-службами Exchange](start-using-web-services-in-exchange.md)
    
- [Общие сведения о разработке клиента EWS для Exchange](ews-client-design-overview-for-exchange.md)
    

