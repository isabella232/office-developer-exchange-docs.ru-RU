---
title: аутофоффице
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- OutOfOffice
api_type:
- schema
ms.assetid: fe1256ab-5c0f-467d-abb3-b38a2dc312ae
description: Элемент Аутофоффице представляет ответное сообщение и время для отправки ответного сообщения.
ms.openlocfilehash: 082a81b62e2b783b302b3e749e0066131a46d73e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456901"
---
# <a name="outofoffice"></a><span data-ttu-id="a1201-103">аутофоффице</span><span class="sxs-lookup"><span data-stu-id="a1201-103">OutOfOffice</span></span>

<span data-ttu-id="a1201-104">Элемент **аутофоффице** представляет ответное сообщение и время для отправки ответного сообщения.</span><span class="sxs-lookup"><span data-stu-id="a1201-104">The **OutOfOffice** element represents the response message and a duration time for sending the response message.</span></span> 
  
```XML
<OutOfOffice>
   <ReplyBody/>
   <Duration/>
</OutOfOffice>
```

```XML
<OutOfOffice>
   <ReplyBody/>
</OutOfOffice>
```

<span data-ttu-id="a1201-105">**аутофоффицемаилтип**</span><span class="sxs-lookup"><span data-stu-id="a1201-105">**OutOfOfficeMailTip**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="a1201-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="a1201-106">Attributes and elements</span></span>

<span data-ttu-id="a1201-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="a1201-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a1201-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="a1201-108">Attributes</span></span>

<span data-ttu-id="a1201-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="a1201-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a1201-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="a1201-110">Child elements</span></span>

|<span data-ttu-id="a1201-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a1201-111">**Element**</span></span>|<span data-ttu-id="a1201-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a1201-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a1201-113">реплибоди</span><span class="sxs-lookup"><span data-stu-id="a1201-113">ReplyBody</span></span>](replybody.md) <br/> |<span data-ttu-id="a1201-114">Содержит сообщение об отсутствии на работе (отсутствие на работе) и язык, используемый для сообщения.</span><span class="sxs-lookup"><span data-stu-id="a1201-114">Contains an Out of Office (OOF) message and the language used for the message.</span></span>  <br/> |
|[<span data-ttu-id="a1201-115">Продолжительность (Усеруфсеттингс)</span><span class="sxs-lookup"><span data-stu-id="a1201-115">Duration (UserOofSettings)</span></span>](duration-useroofsettings.md) <br/> |<span data-ttu-id="a1201-116">Содержит время, в течение которого состояние отсутствия на работе включено, если для элемента [уфстате](oofstate.md) задано значение Scheduled.</span><span class="sxs-lookup"><span data-stu-id="a1201-116">Contains the duration that the OOF status is enabled if the [OofState](oofstate.md) element is set to Scheduled.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a1201-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="a1201-117">Parent elements</span></span>

|<span data-ttu-id="a1201-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a1201-118">**Element**</span></span>|<span data-ttu-id="a1201-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a1201-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a1201-120">Подсказки</span><span class="sxs-lookup"><span data-stu-id="a1201-120">MailTips</span></span>](mailtips.md) <br/> |<span data-ttu-id="a1201-121">Представляет значения для различных типов советов по использованию электронной почты.</span><span class="sxs-lookup"><span data-stu-id="a1201-121">Represents values for various types of mail tips.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a1201-122">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="a1201-122">Text value</span></span>

<span data-ttu-id="a1201-123">Нет.</span><span class="sxs-lookup"><span data-stu-id="a1201-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a1201-124">Примечания</span><span class="sxs-lookup"><span data-stu-id="a1201-124">Remarks</span></span>

<span data-ttu-id="a1201-125">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="a1201-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a1201-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="a1201-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a1201-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="a1201-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a1201-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="a1201-128">Schema Name</span></span>  <br/> |<span data-ttu-id="a1201-129">Схема Types</span><span class="sxs-lookup"><span data-stu-id="a1201-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="a1201-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="a1201-130">Validation File</span></span>  <br/> |<span data-ttu-id="a1201-131">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="a1201-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a1201-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="a1201-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="a1201-133">False</span><span class="sxs-lookup"><span data-stu-id="a1201-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a1201-134">См. также</span><span class="sxs-lookup"><span data-stu-id="a1201-134">See also</span></span>

- [<span data-ttu-id="a1201-135">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="a1201-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

