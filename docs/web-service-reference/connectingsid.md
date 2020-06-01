---
title: коннектингсид
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConnectingSID
api_type:
- schema
ms.assetid: 56d6aa52-8fa6-4773-9046-44a6f4f5d97c
description: Элемент Коннектингсид представляет учетную запись для олицетворения при использовании заголовка SOAP Ексчанжеимперсонатион.
ms.openlocfilehash: f4edf63f129fc769f4a2d710a505b40da4057fab
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459281"
---
# <a name="connectingsid"></a>коннектингсид

Элемент **коннектингсид** представляет учетную запись для олицетворения при использовании заголовка SOAP ексчанжеимперсонатион. 
  
- [ексчанжеимперсонатион](exchangeimpersonation.md) 
- [коннектингсид](connectingsid.md)
  
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

**коннектингсидтипе**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Имя участника-](principalname.md) <br/> |Представляет имя участника-пользователя (UPN) учетной записи, используемой для олицетворения. Это должно быть имя участника-пользователя для домена, в котором находится учетная запись пользователя.  <br/> |
|[SID](sid.md) <br/> |Представляет форму идентификатора безопасности (SID) для учетной записи, используемой для олицетворения, на языке определения дескрипторов безопасности (SDDL).  <br/> |
|[PrimarySmtpAddress](primarysmtpaddress.md) <br/> |Представляет основной SMTP-адрес учетной записи, используемой для олицетворения Exchange. Если указан основной SMTP-адрес, будет стоить дополнительное средство поиска службы каталогов Active Directory, чтобы получить идентификатор SID пользователя. Рекомендуется использовать SID или UPN, если они доступны.  <br/> |
|[SmtpAddress](smtpaddress.md) <br/> |Представляет SMTP-адрес учетной записи, используемой для олицетворения Exchange. Если указан SMTP-адрес, будет стоить дополнительный поиск в Active Directory, чтобы получить идентификатор SID пользователя. Рекомендуется использовать SID или UPN, если они доступны.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ексчанжеимперсонатион](exchangeimpersonation.md) <br/> |Используется в заголовке SOAP запроса. Когда этот элемент присутствует, вызывающий абонент пытается олицетворить учетную запись, содержащуюся в элементе **ексчанжеимперсонатион** .  <br/> Ниже приведено выражение XPath для этого элемента:  <br/>  `/ExchangeImpersonation` <br/> |
   
## <a name="remarks"></a>Примечания

У вызывающей учетной записи должно быть право **MS – дов** на сервере клиентского доступа и в учетной записи **MS майимперсонате** в базе данных почтовых ящиков, которая содержит почтовый ящик для олицетворения или пользователя Active Directory или объекта Contact. 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Авторизация между серверами в EWS](https://msdn.microsoft.com/library/f1610a20-672d-448b-8c00-5b0fbcaf31cb%28Office.15%29.aspx)

