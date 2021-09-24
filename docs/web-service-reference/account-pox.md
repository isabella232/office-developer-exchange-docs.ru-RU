---
title: Account (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 488fdbdc-e9d9-4301-91ab-e22eb42e549e
description: Элемент Учетной записи указывает параметры учетной записи для пользователя или содержит ответы на ошибки.
ms.openlocfilehash: 89799ab62a2aa4945b0e8f3209ab1fbc7d2fa2e6
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59534055"
---
# <a name="account-pox"></a>Account (POX)

Элемент **Учетной** записи указывает параметры учетной записи для пользователя или содержит ответы на ошибки. 
  
- [AutoDiscover (POX)](autodiscover-pox.md)
- [Response (POX)](response-pox.md)
- [Account (POX)](account-pox.md)
  
```XML
<Account>
   <AccountType/>
   <Action/>
   <MicrosoftOnline/>
   <RedirectURL/>
   <RedirectAddr/>
   <Image/>
   <ServiceHome/>
   <Protocol/>
   <PublicFolderInformation/>
</Account>
```

<br/>

```XML
<Account> 
    <Error/> 
</Account>
```

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[AccountType (POX)](accounttype-pox.md) <br/> |Представляет тип учетной записи.  <br/> |
|[Action (POX)](action-pox.md) <br/> |Предоставляет сведения, которые используются для определения того, требуется ли другой запрос автооткрытия для возврата сведений о конфигурации пользователя.  <br/> |
|[MicrosoftOnline (POX)](microsoftonline-pox.md) <br/> |Содержит значение, которое указывает, размещен ли почтовый ящик пользователя в Exchange Online или Exchange Online в Office 365.  <br/> |
|[RedirectUrl (POX)](redirecturl-pox.md) <br/> |Содержит URL-адрес компьютера, на Exchange Server который установлена роль сервера клиентского доступа, который следует использовать для получения параметров автооткрытия.  <br/> |
|[RedirectAddr (POX)](redirectaddr-pox.md) <br/> |Указывает адрес электронной почты, который следует использовать для последующего запроса автооткрытия.  <br/> |
|[Image (POX)](image-pox.md) <br/> |Содержит путь изображения, используемого для брендинга работы конфигурации.  <br/> |
|[ServiceHome (POX)](servicehome-pox.md) <br/> |Содержит URL-адрес домашней страницы поставщика интернет-услуг (ISP).  <br/> |
|[Protocol (POX)](protocol-pox.md) <br/> |Содержит спецификации для подключения клиента к серверу клиентского доступа.  <br/> |
|[PublicFolderInformation (POX)](publicfolderinformation-pox.md) <br/> |Содержит сведения, которые клиенты могут использовать для отправки запроса автооткрытия для обнаружения общедоступных папок для пользователя.  <br/> |
|[Error (POX)](error-pox.md) <br/> |Содержит ответ на ошибку автонаруже.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Response (POX)](response-pox.md) <br/> |Содержит ответ от службы автооткрытия.  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML автооткрытия POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

