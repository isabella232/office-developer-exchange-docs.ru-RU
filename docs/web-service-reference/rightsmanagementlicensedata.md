---
title: RightsManagementLicenseData
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 38f0b7f4-2338-4e90-af67-e0951e8edfa3
description: Элемент RightsManagementLicenseData указывает сведения о лицензии на управление правами для элемента.
ms.openlocfilehash: 8875e9bad425224f86b6de5149f87a36c2a2581e
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59523470"
---
# <a name="rightsmanagementlicensedata"></a>RightsManagementLicenseData

Элемент **RightsManagementLicenseData** указывает сведения о лицензии на управление правами для элемента. 
  
```XML
<RightsManagementLicenseData>
   <RightsManagedMessageDecryptionStatus/>
   <RmsTemplateId/>
   <TemplateName/>
   <TemplateDescription/>
   <EditAllowed/>
   <ReplyAllowed/>
   <ReplyAllAllowed/>
   <ForwardAllowed/>
   <ModifyRecipientsAllowed/>
   <ExtractAllowed/>
   <PrintAllowed/>
   <ExportAllowed/>
   <ProgrammaticAccessAllowed/>
   <IsOwner/>
   <ContentOwner/>
   <ContentExpiryDate/>
</RightsManagementLicenseData>
```

 **RightsManagementLicenseDataType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

[RightsManagedMessageDecryptionStatus](rightsmanagedmessagedecryptionstatus.md)  |  [RMSTemplateId](rmstemplateid.md)  |  [TemplateName](templatename.md)  |  [TemplateDescription](templatedescription.md)  |  [EditAllowed](editallowed.md)  |  [ReplyAllowed](replyallowed.md)  |  [ReplyAllAllowed](replyallallowed.md)  |  [ForwardAllowed](forwardallowed.md)  |  [ModifyRecipientsAllowed](modifyrecipientsallowed.md)  |  [ExtractAllowed](extractallowed.md)  |  [PrintAllowed](printallowed.md)  |  [ExportAllowed](exportallowed.md)  |  [ProgrammaticAccessAllowed](programmaticaccessallowed.md)  |  [IsOwner](isowner.md)  |  [ContentOwner](contentowner.md)  |  [ContentExpiryDate](contentexpirydate.md)
  
### <a name="parent-elements"></a>Родительские элементы

[Item](item.md)  |  [Сообщение](message-ex15websvcsotherref.md)  |  [MeetingMessage](meetingmessage.md)  |  [MeetingRequest](meetingrequest.md)  |  [MeetingResponse](meetingresponse.md)  |  [MeetingCancellation](meetingcancellation.md)  |  [Задача](task.md)  |  [PostItem](postitem.md)  |  [CalendarItem](calendaritem.md)  |  [Контакт](contact.md)  |  [DistributionList](distributionlist.md)
  
## <a name="remarks"></a>Заметки

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> ||
   

