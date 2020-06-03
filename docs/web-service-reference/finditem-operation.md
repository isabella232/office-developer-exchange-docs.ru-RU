---
title: Операция FindItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
api_name:
- FindItem
api_type:
- schema
ms.assetid: ebad6aae-16e7-44de-ae63-a95b24539729
description: Найдите сведения о операции FindItem EWS.
localization_priority: Priority
ms.openlocfilehash: 499d1ee80ef323c883fa86eb125d8c037fb37d4e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462558"
---
# <a name="finditem-operation"></a>Операция FindItem

Найдите сведения о операции **FindItem** EWS. 
  
Операция **FindItem** выполняет поиск элементов, расположенных в почтовом ящике пользователя. Эта операция предоставляет множество способов фильтрации и форматирования результатов поиска для вызывающего абонента. 
  
## <a name="using-the-finditem-operation"></a>Использование операции FindItem

Запрос операции **FindItem** предоставляет множество способов поиска в почтовом ящике и форматирования данных, возвращаемых в ответе. В запросе **FindItem** можно указать следующее: 
  
- Указывает, является ли поиск неповерхностным или обратимо удаленным. Указание этого параметра является обязательным. Обратите внимание на то, что обратимо удаленный обход с ограничением поиска приведет к возвращению нулевых элементов, даже если имеются элементы, которые удовлетворяют условиям поиска.
    
- Форма ответа элементов. Определяет свойства, возвращаемые в ответе. Указание этого параметра является обязательным.
    
- Папки, из которых выполняется поиск. Указание этого параметра является обязательным.
    
- Механизм разбиения по страницам и типы представлений для возвращения данных представления на страницах. Указание этого параметра необязательно.
    
- Параметры для группировки и сортировки возвращаемых элементов. Указание этого параметра необязательно.
    
- Поисковые ограничения или строки расширенного синтаксиса запросов (AQS) для фильтрации возвращаемых элементов. Дополнительные сведения об использовании AQS для поиска по индексу содержимого: [QueryString (String)](querystring-string.md). Указание этого параметра необязательно.
    
- Порядок сортировки элементов, возвращаемых в ответе. Указание этого параметра необязательно.
    
Операция **FindItem** возвращает только первые 512 байт любого потокового свойства. Для Юникода он возвращает первые 255 символов, используя строку Юникода с завершающим нулем. Он не возвращает ни одного из форматов текста сообщения или списков получателей. В **FindItem** будет возвращена сводка по получателю. Вы можете использовать [операцию GetItem](getitem-operation.md) для получения сведений об элементе. 
  
 **FindItem** возвращает только элемент [Name (EmailAddressType)](name-emailaddresstype.md) и не возвращает элемент [EmailAddress (нонемптистрингтипе)](emailaddress-nonemptystringtype.md) в элементе [Mailbox](mailbox.md) для следующих полей: 
  
- Поле " [от](from.md) " для сообщений 
    
- Поле " [отправитель](sender.md) " для сообщений 
    
- Поле " [Организатор](organizer.md) " для элементов календаря 
    
> [!NOTE]
> Операция **FindItem** может возвращать результаты в элементе [CalendarView](calendarview.md) . Элемент **CalendarView** возвращает один и тот же элемент календаря и все экземпляры повторяющихся собраний. Если элемент **CalendarView** не используется, возвращаются элементы с одним календарем и повторяющиеся элементы основного календаря. Если элемент **CalendarView** не используется, эти экземпляры необходимо развернуть из повторяющейся основной реплики. 
  
Операция **FindItem** может использовать заголовки SOAP, указанные в приведенной ниже таблице. 
  
**Таблица 1. Заголовки SOAP для операций FindItem**

|**Header**|**Элемент**|**Описание**|
|:-----|:-----|:-----|
|**датетимепреЦисион** <br/> |[датетимепреЦисион](datetimeprecision.md) <br/> |Задает разрешение значений данных и времени в ответах от сервера: в секундах или в миллисекундах. Это относится к запросу.  <br/> |
|**Олицетворение** <br/> |[ексчанжеимперсонатион](exchangeimpersonation.md) <br/> |Идентифицирует пользователя, который олицетворяет клиентское приложение. Это относится к запросу.  <br/> |
|**маилбокскултуре** <br/> |[маилбокскултуре](mailboxculture.md) <br/> |Определяет язык и региональные параметры RFC3066, которые будут использоваться для доступа к почтовому ящику. Это относится к запросу.  <br/> |
|**рекуестверсион** <br/> |[рекуестсерверверсион](requestserverversion.md) <br/> |Определяет версию схемы для запроса операции. Это относится к запросу.  <br/> |
|**серверверсион** <br/> |[серверверсионинфо](serverversioninfo.md) <br/> |Определяет версию сервера, который ответил на запрос. Это относится к отклику.  <br/> |
|**тимезонеконтекст** <br/> |[тимезонеконтекст](timezonecontext.md) <br/> |Определяет часовой пояс, который будет использоваться для всех ответов сервера. Это относится к запросу.  <br/> |
   
## <a name="finditem-operation-request-example"></a>Пример запроса операции FindItem

В приведенном ниже примере запроса **FindItem** показано, как получить идентификатор элемента, определенный перечислением **идонли** элемента [басешапе](baseshape.md) для элементов, которые находятся в папке "Удаленные". 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindItem xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
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
    
- [итемшапе](itemshape.md)
    
- [басешапе](baseshape.md)
    
- [парентфолдеридс](parentfolderids.md)
    
- [дистингуишедфолдерид](distinguishedfolderid.md)
    
Чтобы получить дополнительные параметры для сообщения запроса **FindItem** , изучите иерархию схемы. Начните с элемента [FindItem](finditem.md) . 
  
## <a name="successful-finditem-operation-response"></a>Успешный отклик операции FindItem

В следующем примере показан успешный ответ на запрос **FindItem** . 
  
Элементы [Message](message-ex15websvcsotherref.md) представляют сообщения электронной почты и все остальные элементы, которые не являются строго типизированными схемой EWS. Элементы, такие как IPM. Общий доступ и IPM. InfoPath возвращаются в виде элементов [Message](message-ex15websvcsotherref.md) . Exchange не возвращает элемент базового [элемента](item.md) в ответах. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <FindItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

В отклике используются следующие элементы:
  
- [серверверсионинфо](serverversioninfo.md)
    
- [финдитемреспонсе](finditemresponse.md)
    
- [респонсемессажес](responsemessages.md)
    
- [финдитемреспонсемессаже](finditemresponsemessage.md)
    
- [респонсекоде](responsecode.md)
    
- [Рутфолдер (Финдитемреспонсемессаже)](rootfolder-finditemresponsemessage.md)
    
- [Items](items.md)
    
- [Сообщение](message-ex15websvcsotherref.md)
    
- [Идентификатор](itemid.md)
    
Для получения дополнительных параметров для ответного сообщения **FindItem** изучите иерархию схемы. Начните с элемента [финдитемреспонсе](finditemresponse.md) . 
  
## <a name="finditem-operation-error-response"></a>Ответ об ошибке операции FindItem

В следующем примере показан ответ об ошибке для запроса **FindItem** . 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <FindItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

В ответе на сообщение об ошибке используются следующие элементы:
  
- [серверверсионинфо](serverversioninfo.md)
    
- [финдитемреспонсе](finditemresponse.md)
    
- [респонсемессажес](responsemessages.md)
    
- [финдитемреспонсемессаже](finditemresponsemessage.md)
    
- [мессажетекст](messagetext.md)
    
- [респонсекоде](responsecode.md)
    
- [дескриптивелинккэй](descriptivelinkkey.md)
    
Чтобы получить дополнительные параметры для сообщения об ответе на ошибку **FindItem** , изучите иерархию схемы. Начните с элемента [финдитемреспонсе](finditemresponse.md) . 
  
## <a name="version-differences"></a>Различия версий

Версии Exchange, начиная с основной версии 15 и заканчивая сборкой 15.0.898.11, возвращают значение Ерроринвалидоператион в элементе [респонсекоде](responsecode.md) , когда операция **FindItem** используется для поиска в нескольких папках в архивном почтовом ящике. 
  
## <a name="see-also"></a>См. также

- [Поиск элементов](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)
    
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)
    
- **финдитемтипе**
    

