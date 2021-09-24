---
title: Операция FindFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- FindFolder
api_type:
- schema
ms.assetid: 7a9855aa-06cc-45ba-ad2a-645c15b7d031
description: Операция FindFolder использует Exchange веб-службы для поиска подвещений идентифицированной папки и возвращает набор свойств, описывающих набор подмостков.
ms.openlocfilehash: 8c2776a9d60244fe77b6012a09ffbad230d86f63
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59518472"
---
# <a name="findfolder-operation"></a>Операция FindFolder

Операция **FindFolder** использует Exchange веб-службы для поиска подмостков идентифицированной папки и возвращает набор свойств, описывающих набор подмостков. 
  
## <a name="remarks"></a>Заметки

FindFolder возвращает только первые 512 bytes любого потокового свойства. Для Unicode он возвращает первые 255 символов с помощью строки Юникод с null-terminated.
  
Глубокие обходные запросы не могут выполняться в общедоступных папках.
  
Ограничения разрешены и должны использовать только свойства папок, а не свойства элемента. Функции сортировки недоступны для ответов **FindFolder.** Групповые запросы недоступны для **запросов FindFolder.** 
  
 **Примечание** Операция **FindFolder** также используется для поиска управляемых папок. 
  
### <a name="soap-headers"></a>Заготчики SOAP

Операция **FindFolder может** использовать заглавные таблицы SOAP, которые перечислены и описаны в следующей таблице. 
  
|**Header**|**Элемент**|**Описание**|
|:-----|:-----|:-----|
|Олицетворение  <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Определяет пользователя, которого клиентская заявка выдвигает.  <br/> |
|MailboxCulture  <br/> |[MailboxCulture](mailboxculture.md) <br/> |Определяет культуру RFC3066, которая будет использоваться для доступа к почтовому ящику.  <br/> |
|RequestVersion  <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Определяет версию схемы для запроса на операцию.  <br/> |
|ServerVersion  <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Определяет версию сервера, отвечаемого на запрос.  <br/> |
|TimeZoneContext  <br/> |[TimeZoneContext](timezonecontext.md) <br/> |Определяет часовой пояс, который будет использоваться для всех ответов с сервера.  <br/> |
   
## <a name="findfolder-request-example"></a>Пример запроса FindFolder

### <a name="description"></a>Описание

В следующем примере **запроса FindFolder** показано, как сформировать запрос, чтобы найти все папки, расположенные в папке "Входящие". 
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindFolder Traversal="Shallow" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

С помощью значения по умолчанию [для BaseShape](baseshape.md)ответ возвращает имя папки, ID папки, количество подмостков, количество детских папок, найденных в папке, и количество непрочитанные элементы.
  
### <a name="request-elements"></a>Элементы запроса

Этот **запрос FindFolder** содержит следующие элементы: 
  
- [FindFolder](findfolder.md)
    
- [FolderShape](foldershape.md)
    
- [BaseShape](baseshape.md)
    
- [ParentFolderIds](parentfolderids.md)
    
- [DistinguishedFolderId](distinguishedfolderid.md)
    
 Дополнительные **элементы запроса FindFolder** см. в схеме. 
  
## <a name="findfolder-response-example"></a>Пример ответа FindFolder

### <a name="description"></a>Описание

В следующем примере Протокол SOAP (SOAP) показан успешный ответ на запрос **FindFolder.** Ответ содержит элементы, возвращаемые при добавлении значения По умолчанию [для BaseShape.](baseshape.md) 
  
> [!NOTE]
> ID папки и ключ изменения были сокращены для сохранения читаемости. 
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="652" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <FindFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

Свойства, возвращаемые в ответе, определяются [BaseShape](baseshape.md) и [AdditionalProperties,](additionalproperties.md) если они используются. Успешный **ответ FindFolder** включает следующие элементы: 
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [FindFolderResponse](findfolderresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [FindFolderResponseMessage](findfolderresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [RootFolder (FindItemResponseMessage)](rootfolder-finditemresponsemessage.md)
    
- [Folders](folders-ex15websvcsotherref.md)
    
- [Folder](folder.md)
    
- [FolderId](folderid.md)
    
- [DisplayName (string)](displayname-string.md)
    
- [TotalCount](totalcount.md)
    
- [ChildFolderCount](childfoldercount.md)
    
- [UnreadCount](unreadcount.md)
    
### <a name="comments"></a>Комментарии

 **Ответы FindFolder** на запрос с помощью формы ответа **AllProperties** не возвращают элементы [TotalCount](totalcount.md) и [UnreadCount](unreadcount.md) для поиска общедоступных папок. 
  
## <a name="findfolder-error-response-example"></a>Пример ответа на ошибку FindFolder

### <a name="description"></a>Описание

В следующем примере тела SOAP показан ответ на ошибку, которая возникает при поиске папки, идентифицированной идентификатором неправильной папки.
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
                 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                 xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="652" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <FindFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="error-response-elements"></a>Элементы ответа на ошибки

Ответ **на ошибку FindFolder** включает следующие элементы: 
  
- [FindFolderResponse](findfolderresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
## <a name="additional-information"></a>Дополнительные сведения

- Элемент [DisplayName (string)](displayname-string.md) папки всегда включен в форму по умолчанию. 
    
- Элемент [UnreadCount](unreadcount.md) включен в папки Задачи и Заметки. 
    
- Для определения управляемой папки с помощью элемента [ExtendedFieldURI](extendedfielduri.md) используйте значение **PropertyTag** 0x672D типа свойства **Integer.** 
    
## <a name="see-also"></a>См. также



[Поиск папок](https://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)

