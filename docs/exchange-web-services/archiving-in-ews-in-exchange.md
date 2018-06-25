---
title: Архивация в веб-служб Exchange в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 78ae179b-ae4f-4f64-911a-e0c70e0fa314
description: Сведения об архивации в веб-служб Exchange в Exchange.
ms.openlocfilehash: bc282a7774bb74e57550bc663512987839324b83
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760929"
---
# <a name="archiving-in-ews-in-exchange"></a>Архивация в веб-служб Exchange в Exchange

Сведения об архивации в веб-служб Exchange в Exchange.
  
Архивные почтовые ящики, дополнительного почтовые ящики, связанные с пользователем. Архивные почтовые ящики обычно используются для управления ограничениями на размер хранилища электронной почты. Например старые элементы электронной почты могут периодически перемещены из папки «Входящие» в архивный почтовый ящик. 
  
Exchange Online, Exchange Online в составе Office 365 и Exchange Server 2013 представлены два новых операций веб-служб Exchange (EWS), которые можно использовать для архивирования набор почтовых элементов от основного почтового ящика. Архивация элементов папки "Входящие" таким образом сохраняет иерархии папок, вложенных элементов. Кроме того архивные почтовые ящики можно хранить теперь локально на клиенте, либо удаленно, в результате которого большей части прозрачно для пользователей, используя путь к папке для указания на содержимого архива.
  
## <a name="archiving-operations-in-ews"></a>Архивация операций в веб-служб Exchange

В следующей таблице перечислены архивации операций, которые были представлены в Exchange 2013. 
  
|**Имя операции**|**Описание**|
|:-----|:-----|
|[ArchiveItem](http://msdn.microsoft.com/library/1af216b3-13ea-498e-b4fc-23513755d731%28Office.15%29.aspx) <br/> |Перемещает элемент из основного почтового ящика в архивный почтовый ящик.  <br/> |
|[CreateFolderPath](http://msdn.microsoft.com/library/5a10aa5e-3f25-4ec3-a0b9-284c30918a1f%28Office.15%29.aspx) <br/> |Создает URI, указывающий на место хранения для архивного почтового ящика.  <br/> |
   
## <a name="see-also"></a>См. также

- [Разработка клиентов веб-служб для Exchange](develop-web-service-clients-for-exchange.md)
    
- [Начать работу с использованием веб-служб Exchange](start-using-web-services-in-exchange.md)
    
- [Общие сведения о разработке клиента EWS для Exchange](ews-client-design-overview-for-exchange.md)
    

