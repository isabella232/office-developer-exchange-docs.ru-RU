---
title: Архивация в веб-служб Exchange в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 78ae179b-ae4f-4f64-911a-e0c70e0fa314
description: Сведения о том, как архивировать в EWS в Exchange.
ms.openlocfilehash: b433b9f88905ee255720e8b341d560fa0e464975
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456215"
---
# <a name="archiving-in-ews-in-exchange"></a>Архивация в веб-служб Exchange в Exchange

Сведения о том, как архивировать в EWS в Exchange.
  
Архивные почтовые ящики это дополнительные почтовые ящики, связанные с пользователем. Архивные почтовые ящики обычно используются для управления пределами хранилища электронной почты. Например, старые элементы электронной почты можно периодически перемещать из папки "Входящие" в архивный почтовый ящик. 
  
Exchange Online, Exchange Online в составе Office 365, а Exchange Server 2013 — это две новые операции веб-служб Exchange (EWS), которые можно использовать для архивации набора почтовых элементов из основного почтового ящика. Архивирование элементов папки "Входящие" таким способом сохраняет иерархию папок для элементов. Кроме того, архивные почтовые ящики теперь можно хранить локально на клиенте или удаленно, как правило, как правило, непрозрачным для пользователя, используя путь к папке для ссылки на содержимое архива.
  
## <a name="archiving-operations-in-ews"></a>Операции архивирования в EWS

В следующей таблице перечислены операции архивирования, которые были представлены в Exchange 2013. 
  
|**Имя операции**|**Описание**|
|:-----|:-----|
|[ArchiveItem](https://msdn.microsoft.com/library/1af216b3-13ea-498e-b4fc-23513755d731%28Office.15%29.aspx) <br/> |Перемещает элемент из основного почтового ящика в архивный.  <br/> |
|[CreateFolderPath](https://msdn.microsoft.com/library/5a10aa5e-3f25-4ec3-a0b9-284c30918a1f%28Office.15%29.aspx) <br/> |Создает URI, указывающий на место хранения архивного почтового ящика.  <br/> |
   
## <a name="see-also"></a>См. также

- [Разработка клиентов веб-служб для Exchange](develop-web-service-clients-for-exchange.md)
    
- [Начало работы с веб-службами Exchange](start-using-web-services-in-exchange.md)
    
- [Общие сведения о разработке клиента EWS для Exchange](ews-client-design-overview-for-exchange.md)
    

