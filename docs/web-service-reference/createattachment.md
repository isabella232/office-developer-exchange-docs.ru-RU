---
title: CreateAttachment
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateAttachment
api_type:
- schema
ms.assetid: e33b403a-b7d3-48ee-8d24-6b7abf0d70bc
description: Элемент CreateAttachment определяет запрос на создание вложения для элемента в хранилище Exchange.
ms.openlocfilehash: 4cba1b8865dae5da58b9617b249a29314c67331a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466439"
---
# <a name="createattachment"></a>CreateAttachment

Элемент **CreateAttachment** определяет запрос на создание вложения для элемента в хранилище Exchange. 
  
```xml
<CreateAttachment>
   <ParentItemId/>
   <Attachments/>
</CreateAttachment>
```

 **креатеаттачменттипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[парентитемид](parentitemid.md) <br/> |Определяет родительский элемент хранилища Exchange, который содержит созданное вложение. Элемент [парентитемид](parentitemid.md) должен предоставлять идентификатор реального элемента хранилища Exchange. Элементы реального хранилища можно получить с помощью [операции GetItem](getitem-operation.md); вложения извлекаются с помощью [операции GetAttachment](getattachment-operation.md). Если [парентитемид](parentitemid.md) передается идентификатор вложенного файла, возникает ошибка. Если [парентитемид](parentitemid.md) представляет идентификатор существующего вложения элемента, [Операция CreateAttachment](createattachment-operation.md) добавляет новое вложение в существующее вложение.  <br/> Этот элемент является обязательным для [операции CreateAttachment](createattachment-operation.md).  <br/> |
|[Вложения](attachments-ex15websvcsotherref.md) <br/> |Содержит элементы или файлы, которые необходимо присоединить к элементу в хранилище Exchange.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="remarks"></a>Примечания

Вложение элемента не существует как элемент хранилища. Он существует только в виде вложения в элемент или другое вложение. Вложения элементов можно получить только с помощью запроса [GetAttachment](getattachment.md) . 
  
Можно создавать следующие вложения элементов:
  
- Элемент
    
- Сообщение
    
- календаритем
    
- Контакт
    
- Задача
    
- митингмессаже
    
- Свойство meetingrequest
    
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="example"></a>Пример

В приведенном ниже примере показано, как создать элемент и прикрепить его к другому элементу в хранилище Exchange.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateAttachment xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" 
                  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <ParentItemId Id="ASkAS"/>
      <Attachments>
        <t:ItemAttachment>
          <t:Name>MyAttachment</t:Name>
          <t:Message>
            <t:ItemClass>IPM>Note</t:ItemClass>
            <t:Subject>My attachment subject</t:Subject>
            <t:Body BodyType="Text">My attachment body</t:Body>
          </t:Message>
        </t:ItemAttachment>
      </Attachments>
    </CreateAttachment>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция CreateAttachment](createattachment-operation.md)
  
[Операция DeleteAttachment](deleteattachment-operation.md)
  
[Операция GetAttachment](getattachment-operation.md)

