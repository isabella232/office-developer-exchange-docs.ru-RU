---
title: OofSettings
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- OofSettings
api_type:
- schema
ms.assetid: 8f37d174-db11-427c-bbed-fdde754a60c7
description: Элемент OofSettings содержит параметры об отсутствии на работе Office (отсутствие на работе).
ms.openlocfilehash: d71f068ff24af22da98b6b4de090ab26d3f74f26
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834649"
---
# <a name="oofsettings"></a><span data-ttu-id="26789-103">OofSettings</span><span class="sxs-lookup"><span data-stu-id="26789-103">OofSettings</span></span>

<span data-ttu-id="26789-104">Элемент **OofSettings** содержит параметры об отсутствии на работе Office (отсутствие на работе).</span><span class="sxs-lookup"><span data-stu-id="26789-104">The **OofSettings** element contains the Out of Office (OOF) settings.</span></span> 
  
[<span data-ttu-id="26789-105">GetUserOofSettingsResponse</span><span class="sxs-lookup"><span data-stu-id="26789-105">GetUserOofSettingsResponse</span></span>](getuseroofsettingsresponse.md)
  
[<span data-ttu-id="26789-106">OofSettings</span><span class="sxs-lookup"><span data-stu-id="26789-106">OofSettings</span></span>](oofsettings.md)
  
```xml
<OofSettings>
   <OofState>...</OofState>
   <ExternalAudience>...</ExternalAudience>
   <Duration>...</Duration>
   <InternalReply>...</InternalReply>
   <ExternalReply>...</ExternalReply>
</OofSettings>
```

 <span data-ttu-id="26789-107">**UserOofSettings**</span><span class="sxs-lookup"><span data-stu-id="26789-107">**UserOofSettings**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="26789-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="26789-108">Attributes and elements</span></span>

<span data-ttu-id="26789-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="26789-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="26789-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="26789-110">Attributes</span></span>

<span data-ttu-id="26789-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="26789-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="26789-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="26789-112">Child elements</span></span>

|<span data-ttu-id="26789-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="26789-113">**Element**</span></span>|<span data-ttu-id="26789-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="26789-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="26789-115">OofState</span><span class="sxs-lookup"><span data-stu-id="26789-115">OofState</span></span>](oofstate.md) <br/> |<span data-ttu-id="26789-116">Содержит состояние пользователя об отсутствии на работе.</span><span class="sxs-lookup"><span data-stu-id="26789-116">Contains the user's OOF state.</span></span>  <br/> |
|[<span data-ttu-id="26789-117">ExternalAudience</span><span class="sxs-lookup"><span data-stu-id="26789-117">ExternalAudience</span></span>](externalaudience.md) <br/> |<span data-ttu-id="26789-118">Содержит значение, определяющее, которому отправляются внешних сообщений об отсутствии на работе.</span><span class="sxs-lookup"><span data-stu-id="26789-118">Contains a value that determines to whom external OOF messages are sent.</span></span>  <br/> |
|[<span data-ttu-id="26789-119">Продолжительность (UserOofSettings)</span><span class="sxs-lookup"><span data-stu-id="26789-119">Duration (UserOofSettings)</span></span>](duration-useroofsettings.md) <br/> |<span data-ttu-id="26789-120">Содержит во время выполнения, для которого включен состояние об отсутствии на работе, если элемент [OofState](oofstate.md) задано значение **Запланировано**.</span><span class="sxs-lookup"><span data-stu-id="26789-120">Contains the duration for which the OOF status is enabled if the [OofState](oofstate.md) element is set to **Scheduled**.</span></span> <span data-ttu-id="26789-121">Если элемент [OofState](oofstate.md) — это значение **включено** или **отключено**, значение этого элемента игнорируется.</span><span class="sxs-lookup"><span data-stu-id="26789-121">If the [OofState](oofstate.md) element is set to **Enabled** or **Disabled**, the value of this element is ignored.</span></span>  <br/> |
|[<span data-ttu-id="26789-122">InternalReply</span><span class="sxs-lookup"><span data-stu-id="26789-122">InternalReply</span></span>](internalreply.md) <br/> |<span data-ttu-id="26789-123">Содержит ответа об отсутствии на работе, для других пользователей в домене или доверенном домене пользователя.</span><span class="sxs-lookup"><span data-stu-id="26789-123">Contains the OOF response sent to other users in the user's domain or trusted domain.</span></span>  <br/> |
|[<span data-ttu-id="26789-124">ExternalReply</span><span class="sxs-lookup"><span data-stu-id="26789-124">ExternalReply</span></span>](externalreply.md) <br/> |<span data-ttu-id="26789-125">Содержит отправлено адресам за пределами домена или доверенных доменов получателя ответов об отсутствии на работе.</span><span class="sxs-lookup"><span data-stu-id="26789-125">Contains the OOF response sent to addresses outside the recipient's domain or trusted domains.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="26789-126">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="26789-126">Parent elements</span></span>

|<span data-ttu-id="26789-127">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="26789-127">**Element**</span></span>|<span data-ttu-id="26789-128">**Описание**</span><span class="sxs-lookup"><span data-stu-id="26789-128">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="26789-129">GetUserOofSettingsResponse</span><span class="sxs-lookup"><span data-stu-id="26789-129">GetUserOofSettingsResponse</span></span>](getuseroofsettingsresponse.md) <br/> |<span data-ttu-id="26789-130">Содержит параметры об отсутствии на работе для пользователя и результатов ответа.</span><span class="sxs-lookup"><span data-stu-id="26789-130">Contains the response results and the OOF settings for a user.</span></span>  <br/> <span data-ttu-id="26789-131">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="26789-131">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserOofSettingsResponse` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="26789-132">Замечания</span><span class="sxs-lookup"><span data-stu-id="26789-132">Remarks</span></span>

<span data-ttu-id="26789-133">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="26789-133">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="26789-134">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="26789-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="26789-135">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="26789-135">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="26789-136">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="26789-136">Schema Name</span></span>  <br/> |<span data-ttu-id="26789-137">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="26789-137">Messages schema</span></span>  <br/> |
|<span data-ttu-id="26789-138">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="26789-138">Validation File</span></span>  <br/> |<span data-ttu-id="26789-139">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="26789-139">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="26789-140">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="26789-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="26789-141">False</span><span class="sxs-lookup"><span data-stu-id="26789-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="26789-142">См. также</span><span class="sxs-lookup"><span data-stu-id="26789-142">See also</span></span>



[<span data-ttu-id="26789-143">Операция GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="26789-143">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md)
  
[<span data-ttu-id="26789-144">Операция SetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="26789-144">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)

