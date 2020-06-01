---
title: Подсказки
manager: sethgros
ms.date: 09/17/2015
ms.audience: ITPro
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MailTips
api_type:
- schema
ms.assetid: c1cba493-bccc-4b8e-be8e-bfa8a8b10882
description: Элемент подсказки представляет значения для различных типов советов по использованию электронной почты.
ms.openlocfilehash: 9bacdea7b4f3108f700ed102025445e01a73e69d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44447598"
---
# <a name="mailtips"></a>Подсказки

Элемент **подсказки** представляет значения для различных типов советов по использованию электронной почты. 
  
```XML
<MailTips>
   <RecipientAddress/>
   <PendingMailTips/>
   <OutOfOffice/>
   <MailboxFull/>
   <CustomMailTip/>
   <TotalMemberCount/>
   <ExternalMemberCount/>
   <MaxMessageSize/>
   <DeliveryRestricted/>
   <IsModerated/>
   <InvalidRecipient/>
</MailTips>
```

 **Подсказки**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[RecipientAddress](recipientaddress.md) <br/> |Представляет почтовый ящик получателя.  <br/> |
|[пендингмаилтипс](pendingmailtips.md) <br/> |Указывает, что советы по использованию электронной почты в этом элементе невозможно оценить до истечения времени ожидания обработки на сервере.  <br/> |
|[аутофоффице](outofoffice.md) <br/> |Представляет ответное сообщение и время для отправки ответного сообщения.  <br/> |
|[маилбоксфулл](mailboxfull.md) <br/> |Указывает, заполнен ли почтовый ящик получателя.  <br/> |
|[кустоммаилтип](custommailtip.md) <br/> |Представляет настраиваемое сообщение подсказки.  <br/> |
|[тоталмемберкаунт](totalmembercount.md) <br/> |Представляет количество всех элементов в группе.  <br/> |
|[екстерналмемберкаунт](externalmembercount.md) <br/> |Представляет количество внешних элементов в группе.  <br/> |
|[MaxMessageSize](maxmessagesize.md) <br/> |Представляет максимальный размер сообщения, которое может принимать получатель.  <br/> |
|[деливерирестриктед](deliveryrestricted.md) <br/> |Указывает, будут ли ограничения доставки допустить достижение получателю сообщения отправителя.  <br/> |
|[Модератор](ismoderated.md) <br/> |Указывает, является ли почтовый ящик получателя ведущим.  <br/> |
|[ИнвалидреЦипиент (подсказки)](invalidrecipient-mailtips.md) <br/> |Указывает, является ли получатель недопустимым.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[маилтипсреспонсемессажетипе](mailtipsresponsemessagetype.md) <br/> |Представляет параметры почтовых подсказок.  <br/> |
   
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
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

