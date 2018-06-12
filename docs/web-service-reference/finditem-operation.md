---
title: FindItem Operation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FindItem
api_type:
- schema
ms.assetid: ebad6aae-16e7-44de-ae63-a95b24539729
description: Найдите сведения о веб-служб Exchange FindItem операции.
ms.openlocfilehash: b033ac2930981819a20f1336d40058a5f7c03b89
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762579"
---
# <a name="finditem-operation"></a>FindItem Operation

Найдите сведения о операции **FindItem** веб-служб Exchange. 
  
Операция **FindItem** выполняет поиск элементов, которые расположены в почтовом ящике пользователя. Эта операция предоставляет множество способов для фильтрации и формат возвращения результатов поиска с абонентом. 
  
## <a name="using-the-finditem-operation"></a>С помощью операции FindItem

Операция запроса **FindItem** предоставляет функциональные возможности для поиска почтовых ящиков и формат, как данные возвращаются в ответе. В запросе **FindItem** можно указать следующее: 
  
- Является ли поиск частичного или удаленные обхода. Это задание не требуется. Обратите внимание, что удаленные обхода, в сочетании с ограничения поиска приведет к нулю, найденном даже в том случае, если существуют элементы, соответствующие условиям поиска.
    
- Форма ответа элементов. Определяет свойства, возвращаемого в ответе. Это задание не требуется.
    
- Папки, из которого требуется выполнить поиск. Это задание не требуется.
    
- Подкачки механизм и Просмотр типов для возврата просматривать данные на страницах. Это задание не является обязательным.
    
- Параметры для группировки и сортировки элементов, которые будут возвращены. Это задание не является обязательным.
    
- Ограничения поиска или расширенный синтаксис запроса (AQS) строки для фильтрации элементов, которые будут возвращены. Дополнительные сведения об использовании AQS для поиска контента индекса [строки запроса (String)](querystring-string.md)см. Это задание не является обязательным.
    
- Порядок сортировки для элементов, возвращаемого в ответе. Это задание не является обязательным.
    
Операция **FindItem** возвращает только первые 512 байт поддерживающего потоковую передачу свойства. Для Юникод возвращает первые 255 символов, используя строку Юникода символом null. Он не возвращает какие-либо форматы текста сообщения или получателей списков. **FindItem** возвращает получателя сводки. Можно использовать [операции GetItem](getitem-operation.md) , чтобы получить дополнительные сведения об элементе. 
  
 **FindItem** возвращает только элемент [Name (EmailAddressType)](name-emailaddresstype.md) и не возвращает элемент [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) в элементе [почтовых ящиков](mailbox.md) для следующих полей: 
  
- Поля [из](from.md) сообщений 
    
- Поле [отправителя](sender.md) для сообщений 
    
- Поле [Организатор](organizer.md) для элементов календаря 
    
> [!NOTE]
> Операция **FindItem** может возвращать результаты в элементе [представления календаря](calendarview.md) . Элемент **представления календаря** возвращает элементы одного календаря и все вхождения повторяющиеся собрания. Если элемент **представления календаря** не используется, возвращаются элементы одного календаря и повторяющихся элементов главного календаря. Необходимо развернуть вхождения из образца повторения, если не используется элемент **представления календаря** . 
  
Операция **FindItem** можно использовать заголовки SOAP, которые перечислены в следующей таблице. 
  
**В таблице 1. Заголовки SOAP FindItem операции**

|**Header**|**Элемент**|**Описание**|
|:-----|:-----|:-----|
|**DateTimePrecision** <br/> |[DateTimePrecision](datetimeprecision.md) <br/> |Указывает разрешение значения времени и данных в ответов с сервера, в секундах или в миллисекундах. Это применимо к запросу.  <br/> |
|**Олицетворение** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Идентифицирует пользователя, которого олицетворения в клиентском приложении. Это применимо к запросу.  <br/> |
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |Идентифицирует культуры RFC3066, которые будут использоваться для доступа к почтовому ящику. Это применимо к запросу.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Определяет версию схемы для операции запроса. Это применимо к запросу.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Определяет версию сервера, ответившего на запрос. Это применимо для ответа.  <br/> |
|**TimeZoneContext** <br/> |[TimeZoneContext](timezonecontext.md) <br/> |Определяет часовой пояс, который будет использоваться для всех ответов с сервера. Это применимо к запросу.  <br/> |
   
## <a name="finditem-operation-request-example"></a>Пример запроса FindItem операции

В следующем примере запроса **FindItem** показано, как получить идентификатор элемента, определенного в перечислении **IdOnly** [BaseShape](baseshape.md) элемента для элементов, которые находятся в папке «Удаленные». 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
              Traversal="Shallow">
      <ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
      </ItemShape>
      <ParentFolderIds>
        <t:DistinguishedFolderId Id="deleteditems"/>
      </ParentFolderIds>
    </FindItem>
  </soap:Body>
</soap:Envelope>
```

В запросе используются следующие элементы: 
  
- [FindItem](finditem.md)
    
- [ItemShape](itemshape.md)
    
- [BaseShape](baseshape.md)
    
- [ParentFolderIds](parentfolderids.md)
    
- [DistinguishedFolderId](distinguishedfolderid.md)
    
Дополнительные параметры для сообщения запроса **FindItem** изучите иерархия схемы. Начать с [FindItem](finditem.md) элемента. 
  
## <a name="successful-finditem-operation-response"></a>Успешные операции ответа FindItem

В следующем примере показано успешного ответа на запрос **FindItem** . 
  
Элементы [сообщения](message-ex15websvcsotherref.md) представляют сообщения электронной почты и другие элементы, которые не строго типизированные схемой веб-служб Exchange. Элементы, такие как IPM. Общий доступ и IPM.InfoPath возвращаются в виде элементы [сообщения](message-ex15websvcsotherref.md) . Exchange не возвращает [базовый элемент](item.md) в ответы. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <FindItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder TotalItemsInView="10" IncludesLastItemInRange="true">
            <t:Items>
              <t:Message>
                <t:ItemId Id="AS4AUn=" ChangeKey="fsVU4==" />
              </t:Message>
              <t:Message>
                <t:ItemId Id="AS4AUM=" ChangeKey="fsVUA==" />
              </t:Message>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </FindItemResponse>
  </soap:Body>
</soap:Envelope>
```

В ответе используются следующие элементы:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [FindItemResponse](finditemresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [FindItemResponseMessage](finditemresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [RootFolder (FindItemResponseMessage)](rootfolder-finditemresponsemessage.md)
    
- [Элементы](items.md)
    
- [Message](message-ex15websvcsotherref.md)
    
- [Идентификатор элемента](itemid.md)
    
Дополнительные параметры для сообщения ответа **FindItem** изучите иерархия схемы. Запустите в элементе [FindItemResponse](finditemresponse.md) . 
  
## <a name="finditem-operation-error-response"></a>Ошибка операции FindItem ответа

В следующем примере показано возврату ошибки **FindItem** запрос. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <FindItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Error">
          <m:MessageText>Id is malformed.</m:MessageText>
          <m:ResponseCode>ErrorInvalidIdMalformed</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </FindItemResponse>
  </soap:Body>
</soap:Envelope>
```

В ответ на ошибку используются следующие элементы:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [FindItemResponse](finditemresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [FindItemResponseMessage](finditemresponsemessage.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
Дополнительные параметры для ответное сообщение об ошибке **FindItem** изучите иерархия схемы. Запустите в элементе [FindItemResponse](finditemresponse.md) . 
  
## <a name="version-differences"></a>Различия версий

Версии Exchange, начиная с версии 15 и выполните построение 15.0.898.11 возвращаемое значение ErrorInvalidOperation в элементе [ResponseCode](responsecode.md) при использовании операции **FindItem** для нескольких папки поиска в архивный почтовый ящик. 
  
## <a name="see-also"></a>См. также

- [Поиск элементов](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)
    
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)
    
- **FindItemType**
    

