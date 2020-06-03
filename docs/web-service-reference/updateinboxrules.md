---
title: UpdateInboxRules
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateInboxRules
api_type:
- schema
ms.assetid: d220064f-ff4d-4537-8077-adf94f2cbdbd
description: Элемент UpdateInboxRules определяет запрос на обновление правил папкиВходящиепочтового ящика в хранилище сервера.
ms.openlocfilehash: d604604d582d28c07eaa75d3239082d1b6735e65
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456362"
---
# <a name="updateinboxrules"></a>UpdateInboxRules

Информация, содержащаяся в этом документе, может относиться к функциям и продуктам предварительной версии и может претерпеть значительные изменения до окончательного коммерческого выпуска. Настоящий документ предоставляется "как есть" и служит только для информационных целей. Корпорация Майкрософт не предоставляет никаких гарантий, явных или подразумеваемых, в связи с этим документом Элемент **UpdateInboxRules** определяет запрос на обновление правил папки "Входящие" почтового ящика в хранилище сервера. 
  
```XML
<UpdateInboxRules>
   <MailboxSmtpAddress/>
   <RemoveOutlookRuleBlob/>
   <Operations/>
</UpdateInboxRules>
```

 **упдатеинбоксрулесрекуесттипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[маилбокссмтпаддресс](mailboxsmtpaddress.md) <br/> |Представляет SMTP-адрес пользователя, чьи правила папки «Входящие», для создания, изменения или удаления.  <br/> |
|[ремовеаутлукрулеблоб](removeoutlookruleblob.md) <br/> |Указывает, следует ли удалять больших двоичных объектов Microsoft Outlook правило.  <br/> |
|[Операции](operations.md) <br/> |Содержит набор операций правила, которые могут выполняться в папке "Входящие".  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Отсутствуют.
  
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также



[Операция UpdateInboxRules](updateinboxrules-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

