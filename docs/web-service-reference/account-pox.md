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
description: Элемент учетной записи определяет параметры учетной записи пользователя или содержит сообщения об ошибках.
ms.openlocfilehash: 88911aad41816f7cefbffef151e066fe5d4da192
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762495"
---
# <a name="account-pox"></a>Учетная запись (POX)

Элемент **учетной записи** определяет параметры учетной записи пользователя или содержит сообщения об ошибках. 
  
- [Автообнаружение (POX)](autodiscover-pox.md)
  
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

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[AccountType (POX)](accounttype-pox.md) <br/> |Представляет тип учетной записи.  <br/> |
|[Действие (POX)](action-pox.md) <br/> |Предоставляет сведения, используемые для определения того, требуется ли другой запрос службы автообнаружения для возврата сведений о конфигурации пользователя.  <br/> |
|[MicrosoftOnline (POX)](microsoftonline-pox.md) <br/> |Содержит значение, которое указывает почтовый ящик пользователя размещается ли в Exchange Online или Exchange Online в составе Office 365.  <br/> |
|[RedirectUrl (POX)](redirecturl-pox.md) <br/> |Содержит URL-адрес компьютера, на котором работает Exchange Server, который имеет роль сервера клиентского доступа установлен, который следует использовать для получения параметров службы автообнаружения.  <br/> |
|[RedirectAddr (POX)](redirectaddr-pox.md) <br/> |Указывает адрес электронной почты, который следует использовать для последующего запроса службы автообнаружения.  <br/> |
|[Изображение (POX)](image-pox.md) <br/> |Содержит путь, используемый на отображение фирменной настройки качества изображения.  <br/> |
|[ServiceHome (POX)](servicehome-pox.md) <br/> |Содержит URL-адрес домашней страницы поставщика услуг Интернета (поставщика услуг Интернета).  <br/> |
|[Протокол (POX)](protocol-pox.md) <br/> |Содержит спецификации для подключения клиента к серверу клиентского доступа.  <br/> |
|[PublicFolderInformation (POX)](publicfolderinformation-pox.md) <br/> |Содержит сведения, которые клиенты могут использовать для отправки запроса службы автообнаружения для получения сведений о общей папки для пользователя.  <br/> |
|[Ошибка (POX)](error-pox.md) <br/> |Содержит возврату ошибки службы автообнаружения.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Ответ (POX)](response-pox.md) <br/> |Содержит ответ от службы автообнаружения.  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML автоматического обнаружения POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

