---
title: Обработка ошибок, связанных с синхронизации в веб-служб Exchange в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: a0807b90-645a-4ea6-aee1-96828df14be0
description: Узнайте, как обрабатывать ошибки, связанные с синхронизации в приложениях, разработка с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.
ms.openlocfilehash: 6de27d585e467d900941f34b2210877d17205502
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760952"
---
# <a name="handling-synchronization-related-errors-in-ews-in-exchange"></a>Обработка ошибок, связанных с синхронизации в веб-служб Exchange в Exchange

Узнайте, как обрабатывать ошибки, связанные с синхронизации в приложениях, разработка с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.
  
Если приложение синхронизирует элементов и папок, может потребоваться обрабатывать ошибки, связанные с синхронизации. Может обрабатывать эти ошибки во время выполнения или при разработке приложения веб-служб Exchange. Большая часть этих ошибок определены в перечислении [ResponseCodeType](http://msdn.microsoft.com/en-us/library/exchangewebservices.responsecodetype%28v=exchg.80%29.aspx) в управляемый API веб-служб Exchange и элемент [ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) веб-служб Exchange (EWS). 
  
**В таблице 1. Ошибки, связанные с синхронизации и порядок их обработки**

|**Error**|**Происходит при попытке...**|**Обработать его с...**|
|:-----|:-----|:-----|
|ErrorInvalidSyncStateData  <br/> | Синхронизация элементов или папок с помощью значение состояния недопустимый синхронизации.  <br/>  Исключение корневой папки в вашей начального запроса SyncFolderHierarchy при последующих запросов включают корневую папку.  <br/>  Используйте другой корневой папки в последующие запросы.  <br/> | Проверка того, что значение состояния синхронизации, отправляемого совпадения значение состояния синхронизации возвращаются во время предыдущей синхронизации.  <br/>  Проверка того, что не отправке состояние синхронизации для иерархии папок при попытке синхронизации элементов и наоборот.  <br/>  Проверка того, что вы отправляете состояние синхронизации для правильного корневую папку.  <br/>  Проверка того, что же корневую папку указан в каждого запроса.  <br/>  Проверка того, что предыдущего запроса не указана в корневой папке null, во время текущего запроса включает в себя корневую папку корневой. NULL и корневые не обрабатывается так же.  <br/> |
|ErrorSyncFolderNotFound  <br/> |Синхронизируйте вложенных папок или элементов в папке, которая не удается найти на сервере.  <br/> |Проверка того, что к папке идентификатор, указанный в запросе сопоставляет идентификатор папки, возвращенный сервером в ответ на предыдущей синхронизации.  <br/> |
|ErrorTimeoutExpired  <br/> |Отправьте слишком много запросов.  <br/> |Ограничение пакетов 10 элементов в пакете избежать [регулирование](ews-throttling-in-exchange.md).  <br/> |
|[ServiceResponseException](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponseexception%28v=exchg.80%29.aspx) <br/> |Если сервер недоступен или проблемы с подключением подключиться веб-служб Exchange.  <br/> |Проверка возможности подключения к серверу и более поздних версий Повтор запроса. Это ошибка временные службы или ошибка сети.  <br/> |
   
## <a name="see-also"></a>См. также


- [Синхронизация почтового ящика и веб-службах Exchange](mailbox-synchronization-and-ews-in-exchange.md)
    
- [Синхронизация папок с помощью веб-служб Exchange в Exchange](how-to-synchronize-folders-by-using-ews-in-exchange.md)
    
- [Синхронизация элементов с помощью веб-служб Exchange в Exchange](how-to-synchronize-items-by-using-ews-in-exchange.md)
    
- [ServiceResponseException](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponseexception%28v=exchg.80%29.aspx)
    

