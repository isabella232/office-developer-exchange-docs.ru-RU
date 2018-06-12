---
title: FindFolder Operation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FindFolder
api_type:
- schema
ms.assetid: 7a9855aa-06cc-45ba-ad2a-645c15b7d031
description: Операция FindFolder использует веб-служб Exchange, чтобы найти вложенные папки заданной папки и возвращает набор свойств, описывающих вложенные папки.
ms.openlocfilehash: 655455b46d4a3192b294bee9d85352d95ded49ae
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762560"
---
# <a name="findfolder-operation"></a>FindFolder Operation

Операция **FindFolder** использует веб-служб Exchange, чтобы найти вложенные папки заданной папки и возвращает набор свойств, описывающих вложенные папки. 
  
## <a name="remarks"></a>Замечания

FindFolder возвращает только первые 512 байт поддерживающего потоковую передачу свойства. Для Юникод возвращает первые 255 символов, используя строку Юникода символом null.
  
Запросы глубокий обзор не может быть выполнена для общедоступных папок.
  
Ограничения разрешены и следует использовать только свойства папки, но не свойства элемента. Функциональные возможности сортировки для ответов **FindFolder** недоступен. Сгруппированные запросы недоступны для **FindFolder** запросов. 
  
 **Примечание** Операция **FindFolder** также используется для управляемых папок поиска. 
  
### <a name="soap-headers"></a>Заголовки SOAP

Операция **FindFolder** можно использовать заголовки SOAP, которые перечислены и описаны в следующей таблице. 
  
|**Header**|**Элемент**|**Описание**|
|:-----|:-----|:-----|
|Олицетворение  <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Идентифицирует пользователя, которого олицетворения в клиентском приложении.  <br/> |
|MailboxCulture  <br/> |[MailboxCulture](mailboxculture.md) <br/> |Идентифицирует культуры RFC3066, которые будут использоваться для доступа к почтовому ящику.  <br/> |
|RequestVersion  <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Определяет версию схемы для операции запроса.  <br/> |
|ServerVersion  <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Определяет версию сервера, ответившего на запрос.  <br/> |
|TimeZoneContext  <br/> |[TimeZoneContext](timezonecontext.md) <br/> |Определяет часовой пояс, который будет использоваться для всех ответов с сервера.  <br/> |
   
## <a name="findfolder-request-example"></a>Пример запроса FindFolder

### <a name="description"></a>Описание

Пример запроса **FindFolder** показано, как для формирования запроса, чтобы найти все папки, расположенной в папке "Входящие". 
  
### <a name="code"></a>Программа

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindFolder Traversal="Shallow" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <FolderShape>
        <t:BaseShape>Default</t:BaseShape>
      </FolderShape>
      <ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox"/>
      </ParentFolderIds>
    </FindFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Комментарии

Используется значение по умолчанию для [BaseShape](baseshape.md), ответ возвращает имя папки, идентификатор папки количество вложенных папок, количество вложенных папок в папке и количество непрочитанных элементов.
  
### <a name="request-elements"></a>Элементы запроса

В этом запросе **FindFolder** содержит следующие элементы: 
  
- [FindFolder](findfolder.md)
    
- [FolderShape](foldershape.md)
    
- [BaseShape](baseshape.md)
    
- [ParentFolderIds](parentfolderids.md)
    
- [DistinguishedFolderId](distinguishedfolderid.md)
    
 Дополнительные элементы запроса **FindFolder** см. 
  
## <a name="findfolder-response-example"></a>Пример ответа FindFolder

### <a name="description"></a>Описание

В следующем примере тело Simple Object Access Protocol (SOAP) показано успешного ответа на запрос **FindFolder** . Ответ содержит элементы, которые возвращаются при используется значение по умолчанию для [BaseShape](baseshape.md) . 
  
> [!NOTE]
> Идентификатор папки и изменить ключ URL были сокращены, чтобы сохранить удобочитаемость. 
  
### <a name="code"></a>Программа

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="652" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <FindFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:FindFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder TotalItemsInView="1" IncludesLastItemInRange="true">
            <t:Folders>
              <t:Folder>
                <t:FolderId Id="AQAnAH" ChangeKey="AQAAABY" />
                <t:DisplayName>TestFolder</t:DisplayName>
                <t:TotalCount>0</t:TotalCount>
                <t:ChildFolderCount>0</t:ChildFolderCount>
                <t:UnreadCount>0</t:UnreadCount>
              </t:Folder>
            </t:Folders>
          </m:RootFolder>
        </m:FindFolderResponseMessage>
      </m:ResponseMessages>
    </FindFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="response-elements"></a>Элементы ответа

Свойства, возвращаемого в ответе определяются [BaseShape](baseshape.md) и [AdditionalProperties](additionalproperties.md) , если они используются. Успешного ответа **FindFolder** содержит следующие элементы: 
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [FindFolderResponse](findfolderresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [FindFolderResponseMessage](findfolderresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [RootFolder (FindItemResponseMessage)](rootfolder-finditemresponsemessage.md)
    
- [Папки](folders-ex15websvcsotherref.md)
    
- [Folder](folder.md)
    
- [FolderId](folderid.md)
    
- [Отображаемое имя (строка)](displayname-string.md)
    
- [TotalCount](totalcount.md)
    
- [ChildFolderCount](childfoldercount.md)
    
- [UnreadCount](unreadcount.md)
    
### <a name="comments"></a>Комментарии

 **FindFolder** ответы на запрос с фигурой ответа **AllProperties** не возвращает [TotalCount](totalcount.md) и элементы [UnreadCount](unreadcount.md) для общедоступных папок поиска. 
  
## <a name="findfolder-error-response-example"></a>Пример ответа об ошибке FindFolder

### <a name="description"></a>Описание

В следующем примере тело SOAP показано возврату ошибки, возникающих при выполнении поиска для папки, который идентифицируется по идентификатору неверно сформированные папки.
  
### <a name="code"></a>Программа

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
                 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                 xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="652" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <FindFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:FindFolderResponseMessage ResponseClass="Error">
          <m:MessageText>Id is malformed.</m:MessageText>
          <m:ResponseCode>ErrorInvalidIdMalformed</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:FindFolderResponseMessage>
      </m:ResponseMessages>
    </FindFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a>Элементы ответа об ошибках

Отклик **FindFolder** содержит следующие элементы: 
  
- [FindFolderResponse](findfolderresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
## <a name="additional-information"></a>Дополнительные сведения

- Элемент [DisplayName (string)](displayname-string.md) папки всегда включается в форме по умолчанию. 
    
- Элемент [UnreadCount](unreadcount.md) входит в папках задач и заметок. 
    
- Используйте значение **PropertyTag** 0x672D с типом свойства **целого числа со знаком** для определения управляемых папок с помощью элемента [ExtendedFieldURI](extendedfielduri.md) . 
    
## <a name="see-also"></a>См. также



[Поиск папок](http://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)

