---
title: Уфстатус (веб-служба единой системы обмена сообщениями)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- OofStatus
api_type:
- schema
ms.assetid: 0ba4225a-784e-4e6e-bd20-be45f0f7597c
description: Элемент Уфстатус содержит значение, указывающее состояние выхода из системы для пользователя, который выполняет операцию GetUMProperties (веб-служба единой системы обмена сообщениями).
ms.openlocfilehash: 80b1d5aa508579eec14637ed10c322b5fbb670da
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460577"
---
# <a name="oofstatus-um-web-service"></a><span data-ttu-id="f13e6-103">Уфстатус (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="f13e6-103">OofStatus (UM web service)</span></span>

<span data-ttu-id="f13e6-104">Элемент **уфстатус** содержит значение, указывающее состояние выхода из системы для пользователя, который выполняет [операцию GetUMProperties (веб-служба единой системы обмена](getumproperties-operation-um-web-service.md) сообщениями).</span><span class="sxs-lookup"><span data-stu-id="f13e6-104">The **OofStatus** element contains a value that indicaties the Unified Messaging Out of Office status for the user who is making a [GetUMProperties operation (UM web service)](getumproperties-operation-um-web-service.md) request.</span></span> 
  
[<span data-ttu-id="f13e6-105">Жетумпропертиесреспонсе (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="f13e6-105">GetUMPropertiesResponse (UM web service)</span></span>](getumpropertiesresponse-um-web-service.md)
  
[<span data-ttu-id="f13e6-106">Уфстатус (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="f13e6-106">OofStatus (UM web service)</span></span>](oofstatus-um-web-service.md)
  
```xml
<GetUMPropertiesResponse>
    <OofStatus/>
  <MissedCallNotificationEnabled/>
  <PlayOnPhoneDialString/>
  <TelephoneAccessNumbers/>
  <TelephoneAccessFolderEmail/>
</GetUMPropertiesResponse>
```

 <span data-ttu-id="f13e6-107">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="f13e6-107">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f13e6-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f13e6-108">Attributes and elements</span></span>

<span data-ttu-id="f13e6-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="f13e6-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f13e6-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f13e6-110">Attributes</span></span>

<span data-ttu-id="f13e6-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f13e6-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f13e6-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f13e6-112">Child elements</span></span>

<span data-ttu-id="f13e6-113">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f13e6-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f13e6-114">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f13e6-114">Parent elements</span></span>

|<span data-ttu-id="f13e6-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f13e6-115">**Element**</span></span>|<span data-ttu-id="f13e6-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f13e6-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f13e6-117">Жетумпропертиесреспонсе (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="f13e6-117">GetUMPropertiesResponse (UM web service)</span></span>](getumpropertiesresponse-um-web-service.md) <br/> |<span data-ttu-id="f13e6-118">Определяет ответ на запрос [GetUMPropertiesной операции (веб-службы единой системы обмена сообщениями)](getumproperties-operation-um-web-service.md) .</span><span class="sxs-lookup"><span data-stu-id="f13e6-118">Defines a response to a [GetUMProperties operation (UM web service)](getumproperties-operation-um-web-service.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f13e6-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="f13e6-119">Text value</span></span>

<span data-ttu-id="f13e6-120">Необходимо указать текстовое значение Boolean.</span><span class="sxs-lookup"><span data-stu-id="f13e6-120">A Boolean text value is required.</span></span> <span data-ttu-id="f13e6-121">Ниже перечислены возможные значения.</span><span class="sxs-lookup"><span data-stu-id="f13e6-121">The following are the possible values:</span></span>
  
- <span data-ttu-id="f13e6-122">Верно.</span><span class="sxs-lookup"><span data-stu-id="f13e6-122">True</span></span>
    
- <span data-ttu-id="f13e6-123">False</span><span class="sxs-lookup"><span data-stu-id="f13e6-123">False</span></span>
    
## <a name="element-information"></a><span data-ttu-id="f13e6-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f13e6-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f13e6-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f13e6-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f13e6-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f13e6-126">Schema Name</span></span>  <br/> |<span data-ttu-id="f13e6-127">Сообщения</span><span class="sxs-lookup"><span data-stu-id="f13e6-127">Messages</span></span>  <br/> |
|<span data-ttu-id="f13e6-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f13e6-128">Validation File</span></span>  <br/> |<span data-ttu-id="f13e6-129">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="f13e6-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f13e6-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f13e6-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="f13e6-131">False</span><span class="sxs-lookup"><span data-stu-id="f13e6-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f13e6-132">См. также</span><span class="sxs-lookup"><span data-stu-id="f13e6-132">See also</span></span>



[<span data-ttu-id="f13e6-133">Операция GetUMProperties (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="f13e6-133">GetUMProperties operation (UM web service)</span></span>](getumproperties-operation-um-web-service.md)
  
[<span data-ttu-id="f13e6-134">Жетумпропертиесреспонсе (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="f13e6-134">GetUMPropertiesResponse (UM web service)</span></span>](getumpropertiesresponse-um-web-service.md)

