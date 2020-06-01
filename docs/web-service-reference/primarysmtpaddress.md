---
title: PrimarySmtpAddress
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PrimarySmtpAddress
api_type:
- schema
ms.assetid: eee79904-9412-4e61-b9b8-aff0ce25fade
description: Элемент PrimarySmtpAddress представляет основной SMTP-адрес учетной записи, которая будет использоваться для авторизации "сервер-сервер" или "делегированный доступ".
ms.openlocfilehash: eea995b3e546d7e94e65cf9b230b639a781c4928
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467965"
---
# <a name="primarysmtpaddress"></a>PrimarySmtpAddress

Элемент **PrimarySmtpAddress** представляет основной SMTP-адрес учетной записи, которая будет использоваться для авторизации "сервер-сервер" или "делегированный доступ". 
  
```xml
<PrimarySmtpAddress/>
```

 **примарисмтпаддресстипе**
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
|[сериализедсекуритиконтекст](serializedsecuritycontext.md) <br/> |Используется в заголовке SOAP для сериализации маркеров при проверке подлинности "сервер — сервер".  <br/> |
|[UserId](userid.md) <br/> |Определяет делегата или пользователя с разрешениями на доступ к папке.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Необходимо указать текстовое значение, представляющее SMTP-адрес.
  
## <a name="remarks"></a>Примечания

Веб-службы Exchange требуют, чтобы почтовые ящики определялись основным SMTP-адресом почтового ящика. Прокси-сервер или альтернативные адреса не принимаются.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера под управлением Microsoft Exchange Server 2010, на котором установлена роль сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)


[Авторизация между серверами в EWS](https://msdn.microsoft.com/library/f1610a20-672d-448b-8c00-5b0fbcaf31cb%28Office.15%29.aspx)
  
[Работа с делегированным доступом](https://msdn.microsoft.com/library/dfd6b4a3-8fd3-47ba-83c0-52465cb5f3f3%28Office.15%29.aspx)

