---
title: ConnectingSID
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ConnectingSID
api_type:
- schema
ms.assetid: 56d6aa52-8fa6-4773-9046-44a6f4f5d97c
description: Элемент ConnectingSID представляет учетную запись для олицетворения при использовании загона SOAP ExchangeImpersonation.
ms.openlocfilehash: 21cfcfc3590ea5a8b8ca5b53dfdb403e108e37f7
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59515973"
---
# <a name="connectingsid"></a>ConnectingSID

Элемент **ConnectingSID** представляет учетную запись для олицетворения при использовании загона SOAP ExchangeImpersonation. 
  
- [ExchangeImpersonation](exchangeimpersonation.md) 
- [ConnectingSID](connectingsid.md)
  
```xml
<ConnectingSID>
   <PrincipalName/>
</ConnectingSID>
```

```xml
<ConnectingSID>
   <SmtpAddress/>
</ConnectingSID>
```

```xml
<ConnectingSID>
    <SID/> 
</ConnectingSID>
```

```xml
<ConnectingSID>
   <PrimarySmtpAddress/>
</ConnectingSID>
```

**ConnectingSIDType**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[PrincipalName](principalname.md) <br/> |Представляет основное имя пользователя (UPN) учетной записи, используемой для олицетворения. Это должен быть upN для домена, в котором существует учетная запись пользователя.  <br/> |
|[SID](sid.md) <br/> |Представляет язык определения дескриптора безопасности (SDDL) идентификатора безопасности (SID) для учетной записи, используемой для олицетворения.  <br/> |
|[PrimarySmtpAddress](primarysmtpaddress.md) <br/> |Представляет основной простой адрес протокола передачи почты (SMTP) учетной записи, используемой для Exchange олицетворения. Если основной SMTP-адрес будет предоставлен, это будет стоить дополнительных дополнительных служб каталогов Active Directory, чтобы получить SID пользователя. Мы рекомендуем использовать SID или UPN, если они доступны.  <br/> |
|[SmtpAddress](smtpaddress.md) <br/> |Представляет простой адрес протокола передачи почты (SMTP) учетной записи для использования Exchange олицетворения. Если адрес SMTP будет предоставлен, это будет стоить дополнительного смотра Active Directory, чтобы получить SID пользователя. Мы рекомендуем использовать SID или UPN, если они доступны.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Используется в заглавной части SOAP запроса. Когда этот элемент присутствует, вызываемая пытается представить учетную запись, которая содержится в **элементе ExchangeImpersonation.**  <br/> Ниже приводится выражение XPath к этому элементу:  <br/>  `/ExchangeImpersonation` <br/> |
   
## <a name="remarks"></a>Заметки

Учетная запись вызова должна иметь право на **ms-exch-impersonation** прямо на сервере клиентского доступа и **на ms-exch-MayImpersonate** прямо на базе данных почтовых ящиков, содержащем почтовый ящик, который должен выдать себя за пользователя Active Directory или контактного объекта. 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Авторизация от сервера до сервера в EWS](https://msdn.microsoft.com/library/f1610a20-672d-448b-8c00-5b0fbcaf31cb%28Office.15%29.aspx)

