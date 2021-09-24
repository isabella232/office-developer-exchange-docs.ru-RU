---
title: Обработка ошибок, связанных с синхронизацией в EWS в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: a0807b90-645a-4ea6-aee1-96828df14be0
description: Узнайте, как обрабатывать ошибки, связанные с синхронизацией, в приложениях, которые разрабатываются с помощью управляемого API EWS или EWS в Exchange.
ms.openlocfilehash: fd52b54413c6fc791132fb01b47bc9077d0266b2
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513250"
---
# <a name="handling-synchronization-related-errors-in-ews-in-exchange"></a>Обработка ошибок, связанных с синхронизацией в EWS в Exchange

Узнайте, как обрабатывать ошибки, связанные с синхронизацией, в приложениях, которые разрабатываются с помощью управляемого API EWS или EWS в Exchange.
  
Если приложение синхронизирует элементы и папки, возможно, придется обрабатывать ошибки, связанные с синхронизацией. Вы можете обрабатывать эти ошибки во время работы или во время разработки приложения EWS. Большинство из этих ошибок определяются переумежением [ResponseCodeType](https://msdn.microsoft.com/library/exchangewebservices.responsecodetype%28v=exchg.80%29.aspx) в управляемом API EWS и элементом [ResponseCode](https://msdn.microsoft.com/library/aa580757%28v=exchg.150%29.aspx) в Exchange Веб-служб (EWS). 
  
**Таблица 1. Ошибки, связанные с синхронизацией, и их обработка**

|**Ошибка**|**Возникает при попытке...**|**Обработать его...**|
|:-----|:-----|:-----|
|ErrorInvalidSyncStateData  <br/> | Синхронизируйте элементы или папки с помощью недействительных значений состояния синхронизации.  <br/>  Исключите корневую папку в первоначальном запросе SyncFolderHierarchy, если в последующем запросе содержится корневая папка.  <br/>  Используйте различные корневые папки в последующих запросах.  <br/> | Обеспечение того, чтобы значение состояния синхронизации, которое вы отправляете, совпадает со значением состояния синхронизации, возвращенным во время предыдущей синхронизации.  <br/>  Обеспечение того, чтобы при попытке синхронизации элементов не отправляли состояние синхронизации для иерархии папок, и наоборот.  <br/>  Обеспечение отправки состояния синхронизации для правильной корневой папки.  <br/>  Обеспечение того, чтобы в каждом запросе была указана та же корневая папка.  <br/>  Обеспечение того, чтобы в предыдущем запросе не была указана корневая папка null, в то время как текущий запрос включает корневую папку корневого. Null и root не обрабатываются одинаково.  <br/> |
|ErrorSyncFolderNotFound  <br/> |Синхронизировать подмостки или элементы в папке, которую невозможно найти на сервере.  <br/> |Обеспечение того, чтобы указанный в запросе ИД папки совпадал с ИД папки, возвращаемой с сервера в предыдущем ответе на синхронизацию.  <br/> |
|ErrorTimeoutExpired  <br/> |Отправить слишком много запросов.  <br/> |Ограничение пакетов до 10 элементов на одну партию, чтобы избежать [регулирования.](ews-throttling-in-exchange.md)  <br/> |
|[ServiceResponseException](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponseexception%28v=exchg.80%29.aspx) <br/> |Подключение EWS, когда сервер отключен или существует проблема с подключением.  <br/> |Проверка подключения к серверу и повторное обращение к запросу позднее. Это, скорее всего, переходная ошибка службы или ошибка сети.  <br/> |
   
## <a name="see-also"></a>См. также


- [Синхронизация почтового ящика и веб-службах Exchange](mailbox-synchronization-and-ews-in-exchange.md)
    
- [Синхронизация папок с помощью EWS в Exchange](how-to-synchronize-folders-by-using-ews-in-exchange.md)
    
- [Синхронизация элементов с помощью EWS в Exchange](how-to-synchronize-items-by-using-ews-in-exchange.md)
    
- [ServiceResponseException](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponseexception%28v=exchg.80%29.aspx)
    

