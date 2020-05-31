---
title: Учетная запись (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 488fdbdc-e9d9-4301-91ab-e22eb42e549e
description: Элемент Account указывает параметры учетной записи пользователя или содержит ошибочные ответы.
ms.openlocfilehash: 6cd87e678b3a524a69f6dca4d6999a3cff22fa57
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353345"
---
# <a name="account-pox"></a>Учетная запись (POX)

Элемент **Account** указывает параметры учетной записи пользователя или содержит ошибочные ответы. 
  
- [Служба автообнаружения (POX)](autodiscover-pox.md)
- [Ответ (POX)](response-pox.md)
- [Учетная запись (POX)](account-pox.md)
  
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

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[AccountType (POX)](accounttype-pox.md) <br/> |Представляет тип учетной записи.  <br/> |
|[Action (POX)](action-pox.md) <br/> |Предоставляет сведения, используемые, чтобы определить, требуется ли другой запрос автообнаружения для возврата сведений о конфигурации пользователя.  <br/> |
|[MicrosoftOnline (POX)](microsoftonline-pox.md) <br/> |Содержит значение, указывающее, размещается ли почтовый ящик пользователя в Exchange Online или Exchange Online в составе Office 365.  <br/> |
|[RedirectUrl адресом (POX)](redirecturl-pox.md) <br/> |Содержит URL-адрес компьютера, на котором установлен сервер Exchange с установленной ролью сервера клиентского доступа, который следует использовать для получения параметров автообнаружения.  <br/> |
|[Редиректаддр (POX)](redirectaddr-pox.md) <br/> |Указывает адрес электронной почты, который будет использоваться для последующего запроса автообнаружения.  <br/> |
|[Image (POX)](image-pox.md) <br/> |Содержит путь к изображению, используемому для фирменной настройки.  <br/> |
|[Сервицехоме (POX)](servicehome-pox.md) <br/> |Содержит URL-адрес домашней страницы поставщика услуг Интернета.  <br/> |
|[Протокол (POX)](protocol-pox.md) <br/> |Содержит спецификации для подключения клиента к серверу клиентского доступа.  <br/> |
|[Публикфолдеринформатион (POX)](publicfolderinformation-pox.md) <br/> |Содержит сведения, которые клиенты могут использовать для отправки запроса на автообнаружение для обнаружения сведений о общедоступных папках для пользователя.  <br/> |
|[Ошибка (POX)](error-pox.md) <br/> |Содержит ответ об ошибке автообнаружения.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Ответ (POX)](response-pox.md) <br/> |Содержит ответ от службы автообнаружения.  <br/> |
   
## <a name="see-also"></a>См. также

- [XML-элементы автообнаружения POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

