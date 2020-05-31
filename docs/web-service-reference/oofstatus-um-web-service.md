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
ms.openlocfilehash: 1fe358a8bfea3c509220d6705a238ae832de37e8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834650"
---
# <a name="oofstatus-um-web-service"></a><span data-ttu-id="98475-103">Уфстатус (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="98475-103">OofStatus (UM web service)</span></span>

<span data-ttu-id="98475-104">Элемент **уфстатус** содержит значение, указывающее состояние выхода из системы для пользователя, который выполняет [операцию GetUMProperties (веб-служба единой системы обмена](getumproperties-operation-um-web-service.md) сообщениями).</span><span class="sxs-lookup"><span data-stu-id="98475-104">The **OofStatus** element contains a value that indicaties the Unified Messaging Out of Office status for the user who is making a [GetUMProperties operation (UM web service)](getumproperties-operation-um-web-service.md) request.</span></span> 
  
[<span data-ttu-id="98475-105">Жетумпропертиесреспонсе (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="98475-105">GetUMPropertiesResponse (UM web service)</span></span>](getumpropertiesresponse-um-web-service.md)
  
[<span data-ttu-id="98475-106">Уфстатус (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="98475-106">OofStatus (UM web service)</span></span>](oofstatus-um-web-service.md)
  
```xml
<GetUMPropertiesResponse>
    <OofStatus/>
  <MissedCallNotificationEnabled/>
  <PlayOnPhoneDialString/>
  <TelephoneAccessNumbers/>
  <TelephoneAccessFolderEmail/>
</GetUMPropertiesResponse>
```

 <span data-ttu-id="98475-107">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="98475-107">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="98475-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="98475-108">Attributes and elements</span></span>

<span data-ttu-id="98475-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="98475-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="98475-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="98475-110">Attributes</span></span>

<span data-ttu-id="98475-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="98475-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="98475-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="98475-112">Child elements</span></span>

<span data-ttu-id="98475-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="98475-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="98475-114">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="98475-114">Parent elements</span></span>

|<span data-ttu-id="98475-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="98475-115">**Element**</span></span>|<span data-ttu-id="98475-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="98475-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="98475-117">Жетумпропертиесреспонсе (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="98475-117">GetUMPropertiesResponse (UM web service)</span></span>](getumpropertiesresponse-um-web-service.md) <br/> |<span data-ttu-id="98475-118">Определяет ответ на запрос [GetUMPropertiesной операции (веб-службы единой системы обмена сообщениями)](getumproperties-operation-um-web-service.md) .</span><span class="sxs-lookup"><span data-stu-id="98475-118">Defines a response to a [GetUMProperties operation (UM web service)](getumproperties-operation-um-web-service.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="98475-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="98475-119">Text value</span></span>

<span data-ttu-id="98475-120">Необходимо указать текстовое значение Boolean.</span><span class="sxs-lookup"><span data-stu-id="98475-120">A Boolean text value is required.</span></span> <span data-ttu-id="98475-121">Ниже перечислены возможные значения.</span><span class="sxs-lookup"><span data-stu-id="98475-121">The following are the possible values:</span></span>
  
- <span data-ttu-id="98475-122">Верно.</span><span class="sxs-lookup"><span data-stu-id="98475-122">True</span></span>
    
- <span data-ttu-id="98475-123">False</span><span class="sxs-lookup"><span data-stu-id="98475-123">False</span></span>
    
## <a name="element-information"></a><span data-ttu-id="98475-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="98475-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="98475-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="98475-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="98475-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="98475-126">Schema Name</span></span>  <br/> |<span data-ttu-id="98475-127">Сообщения</span><span class="sxs-lookup"><span data-stu-id="98475-127">Messages</span></span>  <br/> |
|<span data-ttu-id="98475-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="98475-128">Validation File</span></span>  <br/> |<span data-ttu-id="98475-129">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="98475-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="98475-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="98475-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="98475-131">False</span><span class="sxs-lookup"><span data-stu-id="98475-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="98475-132">См. также</span><span class="sxs-lookup"><span data-stu-id="98475-132">See also</span></span>



[<span data-ttu-id="98475-133">Операция GetUMProperties (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="98475-133">GetUMProperties operation (UM web service)</span></span>](getumproperties-operation-um-web-service.md)
  
[<span data-ttu-id="98475-134">Жетумпропертиесреспонсе (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="98475-134">GetUMPropertiesResponse (UM web service)</span></span>](getumpropertiesresponse-um-web-service.md)

