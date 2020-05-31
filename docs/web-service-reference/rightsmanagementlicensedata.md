---
title: ригхтсманажементлиценседата
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 38f0b7f4-2338-4e90-af67-e0951e8edfa3
description: Элемент Ригхтсманажементлиценседата указывает сведения о лицензии на управление правами для элемента.
ms.openlocfilehash: ec2ba1dc155afe239c499246095f86fc621910a9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835234"
---
# <a name="rightsmanagementlicensedata"></a>ригхтсманажементлиценседата

Элемент **ригхтсманажементлиценседата** указывает сведения о лицензии на управление правами для элемента. 
  
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

 **ригхтсманажементлиценседататипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

[Ригхтсманажедмессажедекриптионстатус](rightsmanagedmessagedecryptionstatus.md) | [рмстемплатеид](rmstemplateid.md) | [TemplateDescription](templatedescription.md) | [ProgrammaticAccessAllowed](programmaticaccessallowed.md)[PrintAllowed](printallowed.md)[TemplateName](templatename.md) | [ForwardAllowed](forwardallowed.md) | [ContentExpiryDate](contentexpirydate.md) [ReplyAllAllowed](replyallallowed.md) | [ContentOwner](contentowner.md)[ReplyAllowed](replyallowed.md) | [IsOwner](isowner.md)[EditAllowed](editallowed.md) | [ExportAllowed](exportallowed.md)[ExtractAllowed](extractallowed.md)[ModifyRecipientsAllowed](modifyrecipientsallowed.md)TemplateName темплатедескриптион | едиталловед ReplyAllowed ReplyAllAllowed ForwardAllowed | ModifyRecipientsAllowed ExtractAllowed | PrintAllowed ExportAllowed ProgrammaticAccessAllowed Owner ContentOwner ContentExpiryDate |  |  |  | 
  
### <a name="parent-elements"></a>Родительские элементы

[Item](item.md) | [Сообщение](message-ex15websvcsotherref.md) | [MeetingResponse](meetingresponse.md) | [Contact](contact.md)[MeetingMessage](meetingmessage.md) | [MeetingCancellation](meetingcancellation.md)[MeetingRequest](meetingrequest.md) | [DistributionList](distributionlist.md) [Task](task.md)[PostItem](postitem.md)[CalendarItem](calendaritem.md)элемента митингмессаже | свойство meetingrequest митингреспонсе митингканцеллатион | Task | Item | календаритем Contact дистрибутионлист | 
  
## <a name="remarks"></a>Примечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> ||
   

