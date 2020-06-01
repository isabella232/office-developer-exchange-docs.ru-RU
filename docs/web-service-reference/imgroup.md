---
title: Группа
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ab7b884e-ecf1-4e58-86ec-856b13a95f2b
description: Элемент "Группа" представляет группу мгновенных сообщений.
ms.openlocfilehash: a0ff3fcb82e7f18837af5a6f5daa16e90043034d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460689"
---
# <a name="imgroup"></a><span data-ttu-id="35744-103">Группа</span><span class="sxs-lookup"><span data-stu-id="35744-103">ImGroup</span></span>

<span data-ttu-id="35744-104">Элемент " **Группа** " представляет группу мгновенных сообщений.</span><span class="sxs-lookup"><span data-stu-id="35744-104">The **ImGroup** element represents an instant messaging group.</span></span> 
  
```XML
<ImGroup>
   <DisplayName/>
   <GroupType/>
   <ExchangeStoreId/>
   <MemberCorrelationKey/>
   <ExtendedProperties/>
   <SmtpAddress/>
</ImGroup>
```

 <span data-ttu-id="35744-105">**имграуптипе**</span><span class="sxs-lookup"><span data-stu-id="35744-105">**ImGroupType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="35744-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="35744-106">Attributes and elements</span></span>

<span data-ttu-id="35744-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="35744-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="35744-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="35744-108">Attributes</span></span>

<span data-ttu-id="35744-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="35744-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="35744-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="35744-110">Child elements</span></span>

<span data-ttu-id="35744-111">[DisplayName (нонемптистрингтипе)](displayname-nonemptystringtype.md)  |  [GroupType](grouptype.md)  |  [Ексчанжестореид](exchangestoreid.md)  |  [Мемберкоррелатионкэй](membercorrelationkey.md)  |  [Екстендедпропертиес (нонемптяррайофекстендедпропертитипе)](extendedproperties-nonemptyarrayofextendedpropertytype.md)  |  [SmtpAddress](smtpaddress.md)</span><span class="sxs-lookup"><span data-stu-id="35744-111">[DisplayName (NonEmptyStringType)](displayname-nonemptystringtype.md) | [GroupType](grouptype.md) | [ExchangeStoreId](exchangestoreid.md) | [MemberCorrelationKey](membercorrelationkey.md) | [ExtendedProperties (NonEmptyArrayOfExtendedPropertyType)](extendedproperties-nonemptyarrayofextendedpropertytype.md) | [SmtpAddress](smtpaddress.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="35744-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="35744-112">Parent elements</span></span>

<span data-ttu-id="35744-113">[Groups (аррайофимграуптипе)](groups-arrayofimgrouptype.md)  |  [Адддистрибутионграуптоимлистреспонсе](adddistributiongrouptoimlistresponse.md)  |  [Аддимграупреспонсе](addimgroupresponse.md)</span><span class="sxs-lookup"><span data-stu-id="35744-113">[Groups (ArrayOfImGroupType)](groups-arrayofimgrouptype.md) | [AddDistributionGroupToImListResponse](adddistributiongrouptoimlistresponse.md) | [AddImGroupResponse](addimgroupresponse.md)</span></span>
  
## <a name="remarks"></a><span data-ttu-id="35744-114">Примечания</span><span class="sxs-lookup"><span data-stu-id="35744-114">Remarks</span></span>

<span data-ttu-id="35744-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="35744-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="35744-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="35744-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="35744-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="35744-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="35744-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="35744-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="35744-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="35744-119">Schema name</span></span>  <br/> |<span data-ttu-id="35744-120">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="35744-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="35744-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="35744-121">Validation file</span></span>  <br/> |<span data-ttu-id="35744-122">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="35744-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="35744-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="35744-123">Can be empty</span></span>  <br/> ||
   

