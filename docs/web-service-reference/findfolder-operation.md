---
title: Операция FindFolder
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
description: Операция FindFolder использует веб-службы Exchange для поиска вложенных папок в определенной папке и возвращает набор свойств, описывающих набор вложенных папок.
ms.openlocfilehash: f1cc199bdaf684d8d74687ed7f064eb66fee48ff
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462586"
---
# <a name="findfolder-operation"></a>Операция FindFolder

Операция **FindFolder** использует веб-службы Exchange для поиска вложенных папок в определенной папке и возвращает набор свойств, описывающих набор вложенных папок. 
  
## <a name="remarks"></a>Примечания

FindFolder возвращает только первые 512 байт любого потокового свойства. Для Юникода он возвращает первые 255 символов, используя строку Юникода с завершающим нулем.
  
Запросы с глубоким обходом не могут выполняться в общедоступных папках.
  
Ограничения разрешены и должны использовать только свойства папки, а не свойства элемента. Функция сортировки недоступна для ответов **FindFolder** . Сгруппированные запросы недоступны для запросов **FindFolder** . 
  
 **Note (Примечание** ) Операция **FindFolder** также используется для поиска управляемых папок. 
  
### <a name="soap-headers"></a>Заголовки SOAP

В операции **FindFolder** могут использоваться заголовки SOAP, указанные в приведенной ниже таблице. 
  
|**Header**|**Элемент**|**Описание**|
|:-----|:-----|:-----|
|Олицетворение  <br/> |[ексчанжеимперсонатион](exchangeimpersonation.md) <br/> |Идентифицирует пользователя, который олицетворяет клиентское приложение.  <br/> |
|маилбокскултуре  <br/> |[маилбокскултуре](mailboxculture.md) <br/> |Определяет язык и региональные параметры RFC3066, которые будут использоваться для доступа к почтовому ящику.  <br/> |
|рекуестверсион  <br/> |[рекуестсерверверсион](requestserverversion.md) <br/> |Определяет версию схемы для запроса операции.  <br/> |
|серверверсион  <br/> |[серверверсионинфо](serverversioninfo.md) <br/> |Определяет версию сервера, который ответил на запрос.  <br/> |
|тимезонеконтекст  <br/> |[тимезонеконтекст](timezonecontext.md) <br/> |Определяет часовой пояс, который будет использоваться для всех ответов сервера.  <br/> |
   
## <a name="findfolder-request-example"></a>Пример запроса FindFolder

### <a name="description"></a>Описание

В следующем примере запроса **FindFolder** показано, как сформировать запрос на поиск всех папок, расположенных в папке "Входящие". 
  
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

При использовании значения по умолчанию для [басешапе](baseshape.md), ответ возвращает имя папки, идентификатор папки, количество вложенных папок, количество вложенных папок в папке и количество непрочитанных элементов.
  
### <a name="request-elements"></a>Элементы Request

Этот запрос **FindFolder** включает следующие элементы: 
  
- [FindFolder](findfolder.md)
    
- [фолдершапе](foldershape.md)
    
- [басешапе](baseshape.md)
    
- [парентфолдеридс](parentfolderids.md)
    
- [дистингуишедфолдерид](distinguishedfolderid.md)
    
 Дополнительные элементы запроса **FindFolder** приведены в схеме. 
  
## <a name="findfolder-response-example"></a>Пример отклика FindFolder

### <a name="description"></a>Описание

В приведенном ниже примере кода для протокола SOAP показан успешный ответ на запрос **FindFolder** . Ответ содержит элементы, которые возвращаются при использовании значения по умолчанию для [басешапе](baseshape.md) . 
  
> [!NOTE]
> Идентификатор папки и ключ изменения были сокращены, чтобы сохранить удобочитаемость. 
  
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

### <a name="response-elements"></a>Элементы Response

Свойства, возвращаемые в ответе, определяются [басешапе](baseshape.md) и [аддитионалпропертиес](additionalproperties.md) , если они используются. Успешный отклик **FindFolder** содержит следующие элементы: 
  
- [серверверсионинфо](serverversioninfo.md)
    
- [финдфолдерреспонсе](findfolderresponse.md)
    
- [респонсемессажес](responsemessages.md)
    
- [финдфолдерреспонсемессаже](findfolderresponsemessage.md)
    
- [респонсекоде](responsecode.md)
    
- [Рутфолдер (Финдитемреспонсемессаже)](rootfolder-finditemresponsemessage.md)
    
- [Folders](folders-ex15websvcsotherref.md)
    
- [Folder](folder.md)
    
- [FolderId](folderid.md)
    
- [DisplayName (строка)](displayname-string.md)
    
- [тоталкаунт](totalcount.md)
    
- [чилдфолдеркаунт](childfoldercount.md)
    
- [унреадкаунт](unreadcount.md)
    
### <a name="comments"></a>Комментарии

 Элементы **FindFolder** отклика на запрос с фигурой ответа **аллпропертиес** не возвращают элементы [тоталкаунт](totalcount.md) и [унреадкаунт](unreadcount.md) для поиска в общедоступных папках. 
  
## <a name="findfolder-error-response-example"></a>Пример отклика на сообщение об ошибке FindFolder

### <a name="description"></a>Описание

В следующем примере сообщения SOAP показан ответ об ошибке, возникающий при поиске папки, которая определяется с помощью искаженного идентификатора папки.
  
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

### <a name="error-response-elements"></a>Элементы ошибочного ответа

Ответ об ошибке **FindFolder** содержит следующие элементы: 
  
- [финдфолдерреспонсе](findfolderresponse.md)
    
- [респонсемессажес](responsemessages.md)
    
- [мессажетекст](messagetext.md)
    
- [респонсекоде](responsecode.md)
    
- [дескриптивелинккэй](descriptivelinkkey.md)
    
## <a name="additional-information"></a>Дополнительные сведения

- Элемент [DisplayName (строка)](displayname-string.md) папки всегда включается в фигуру по умолчанию. 
    
- Элемент [унреадкаунт](unreadcount.md) включается в папки "задачи" и "Заметки". 
    
- Используйте значение **пропертитаг** для 0x672D с типом свойства **Integer** , чтобы определить управляемую папку с помощью элемента [екстендедфиелдури](extendedfielduri.md) . 
    
## <a name="see-also"></a>См. также



[Поиск папок](https://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)

