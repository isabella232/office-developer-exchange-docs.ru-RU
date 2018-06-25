---
title: Операция UpdateItem (задача)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateItem
api_type:
- schema
ms.assetid: b0a7f114-d040-40eb-a8f3-05ea6489e472
description: Операция UpdateItem используется для обновления свойств элемента задачи в хранилище Exchange.
ms.openlocfilehash: d6f966fa663300b476383a136d30cf611d6bfb9b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840352"
---
# <a name="updateitem-operation-task"></a>Операция UpdateItem (задача)

Операция UpdateItem используется для обновления свойств элемента задачи в хранилище Exchange.
  
## <a name="remarks"></a>Замечания

Веб-служб Exchange нельзя использовать для отправки запросов задач. Веб-служб Exchange может вернуть запросы задач, созданных с MicrosoftOfficeOutlook. Если уже был отправлен запрос задачи, запрос на обновление задачи возвращает ошибку.
  
## <a name="updating-the-current-occurrence-of-a-recurring-task"></a>Обновление текущей копии повторяющейся задачи

Результат операции UpdateItem на повторяющиеся задачи отличается от результат операции UpdateItem single, неповторяющейся задачи. Изменение вхождения повторяющейся задачи приводит одноразовых задач, создаваемых при вносятся следующие обновления:
  
1. Свойство status восстанавливаемой или nonregenerating Повторяющаяся задача задано значение **завершено**.
    
2. Изменить дату начала или дату окончания nonregenerating Повторяющаяся задача.
    
Например если запрос **UpdateItem** устанавливает значение завершено повторяющейся задачи в **значение true**, **UpdateItemResponse** будет включать новый идентификатор и ChangeKey, которые представляют только что созданный одноразовых задач. Идентификатор, который был включен в запрос действителен и повторяющейся задачи, представленного этот идентификатор Id был обновлен для представления следующее вхождение. ChangeKey, который был включен в запросе больше не является допустимым, поскольку обновлена повторяющейся задачи. 
  
[Операции GetItem](getitem-operation.md) можно использовать для получения последних **ChangeKey** для повторяющейся задачи. 
  
Неповторяющейся задачи или последнего вхождения повторяющейся задачи ответа UpdateItem возвращает тот же **идентификатор** , переданным в него и возвращается связанный с ним обновленных **ChangeKey**.
  
## <a name="see-also"></a>См. также



[UpdateItem Operation](updateitem-operation.md)

