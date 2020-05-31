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
ms.openlocfilehash: f35b84d7a8a37c7a57b58c97fd0d37318bb50a33
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354269"
---
# <a name="outofoffice"></a><span data-ttu-id="77254-103">аутофоффице</span><span class="sxs-lookup"><span data-stu-id="77254-103">OutOfOffice</span></span>

<span data-ttu-id="77254-104">Элемент **аутофоффице** представляет ответное сообщение и время для отправки ответного сообщения.</span><span class="sxs-lookup"><span data-stu-id="77254-104">The **OutOfOffice** element represents the response message and a duration time for sending the response message.</span></span> 
  
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

<span data-ttu-id="77254-105">**аутофоффицемаилтип**</span><span class="sxs-lookup"><span data-stu-id="77254-105">**OutOfOfficeMailTip**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="77254-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="77254-106">Attributes and elements</span></span>

<span data-ttu-id="77254-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="77254-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="77254-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="77254-108">Attributes</span></span>

<span data-ttu-id="77254-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="77254-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="77254-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="77254-110">Child elements</span></span>

|<span data-ttu-id="77254-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="77254-111">**Element**</span></span>|<span data-ttu-id="77254-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="77254-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="77254-113">реплибоди</span><span class="sxs-lookup"><span data-stu-id="77254-113">ReplyBody</span></span>](replybody.md) <br/> |<span data-ttu-id="77254-114">Содержит сообщение об отсутствии на работе (отсутствие на работе) и язык, используемый для сообщения.</span><span class="sxs-lookup"><span data-stu-id="77254-114">Contains an Out of Office (OOF) message and the language used for the message.</span></span>  <br/> |
|[<span data-ttu-id="77254-115">Продолжительность (Усеруфсеттингс)</span><span class="sxs-lookup"><span data-stu-id="77254-115">Duration (UserOofSettings)</span></span>](duration-useroofsettings.md) <br/> |<span data-ttu-id="77254-116">Содержит время, в течение которого состояние отсутствия на работе включено, если для элемента [уфстате](oofstate.md) задано значение Scheduled.</span><span class="sxs-lookup"><span data-stu-id="77254-116">Contains the duration that the OOF status is enabled if the [OofState](oofstate.md) element is set to Scheduled.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="77254-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="77254-117">Parent elements</span></span>

|<span data-ttu-id="77254-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="77254-118">**Element**</span></span>|<span data-ttu-id="77254-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="77254-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="77254-120">Подсказки</span><span class="sxs-lookup"><span data-stu-id="77254-120">MailTips</span></span>](mailtips.md) <br/> |<span data-ttu-id="77254-121">Представляет значения для различных типов советов по использованию электронной почты.</span><span class="sxs-lookup"><span data-stu-id="77254-121">Represents values for various types of mail tips.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="77254-122">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="77254-122">Text value</span></span>

<span data-ttu-id="77254-123">Нет.</span><span class="sxs-lookup"><span data-stu-id="77254-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="77254-124">Примечания</span><span class="sxs-lookup"><span data-stu-id="77254-124">Remarks</span></span>

<span data-ttu-id="77254-125">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="77254-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="77254-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="77254-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="77254-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="77254-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="77254-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="77254-128">Schema Name</span></span>  <br/> |<span data-ttu-id="77254-129">Схема Types</span><span class="sxs-lookup"><span data-stu-id="77254-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="77254-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="77254-130">Validation File</span></span>  <br/> |<span data-ttu-id="77254-131">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="77254-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="77254-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="77254-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="77254-133">False</span><span class="sxs-lookup"><span data-stu-id="77254-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="77254-134">См. также</span><span class="sxs-lookup"><span data-stu-id="77254-134">See also</span></span>

- [<span data-ttu-id="77254-135">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="77254-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

