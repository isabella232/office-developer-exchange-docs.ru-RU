---
title: SmtpAddress
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SmtpAddress
api_type:
- schema
ms.assetid: 779305a6-ad1e-424e-8a69-4e3bef61d787
description: Элемент SmtpAddress представляет SMTP-адрес учетной записи, используемой для олицетворения, или адрес получателя SMTP для запроса на общий доступ к календарю или контакту.
ms.openlocfilehash: 915ff328cc384c1f2884e9fbea8c10c1ebc79288
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466691"
---
# <a name="smtpaddress"></a>SmtpAddress

Элемент **SmtpAddress** представляет SMTP-адрес учетной записи, используемой для олицетворения, или адрес получателя SMTP для запроса на общий доступ к календарю или контакту. 
  
```xml
<SmtpAddress/>
```

**смтпаддресстипе**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[коннектингсид](connectingsid.md) <br/> |Представляет учетную запись для олицетворения при использовании заголовка SOAP Ексчанжеимперсонатион.  <br/> Ниже приведено выражение XPath для этого элемента:  <br/>  `/ExchangeImpersonation/ConnectingSID` <br/> |
|[инвалидреЦипиент](invalidrecipient.md) <br/> |Представляет недопустимый получатель сообщения общего доступа к календарю или обмена сообщениями.  <br/> |
|[Получатели (Аррайофсмтпаддресстипе)](recipients-arrayofsmtpaddresstype.md) <br/> |Представляет коллекцию получателей, которым будет предоставлен доступ к общей папке.  <br/> |
|[GetSharingFolder](getsharingfolder.md) <br/> |Определяет запрос на получение идентификатора локальной папки указанной общей папки.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Необходимо указать текстовое значение, представляющее SMTP-адрес.
  
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, на котором размещены веб-службы Exchange компьютера, на котором установлен сервер Microsoft Exchange, на котором установлена роль сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

