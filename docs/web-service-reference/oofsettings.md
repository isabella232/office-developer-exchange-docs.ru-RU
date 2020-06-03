---
title: уфсеттингс
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
description: Элемент Уфсеттингс содержит параметры заместителя (отсутствие на работе).
ms.openlocfilehash: c1b214fd8bfab5b7a82d41a5187cf6e0fc4ba79c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467195"
---
# <a name="oofsettings"></a><span data-ttu-id="1f1a7-103">уфсеттингс</span><span class="sxs-lookup"><span data-stu-id="1f1a7-103">OofSettings</span></span>

<span data-ttu-id="1f1a7-104">Элемент **уфсеттингс** содержит параметры заместителя (отсутствие на работе).</span><span class="sxs-lookup"><span data-stu-id="1f1a7-104">The **OofSettings** element contains the Out of Office (OOF) settings.</span></span> 
  
[<span data-ttu-id="1f1a7-105">жетусеруфсеттингсреспонсе</span><span class="sxs-lookup"><span data-stu-id="1f1a7-105">GetUserOofSettingsResponse</span></span>](getuseroofsettingsresponse.md)
  
[<span data-ttu-id="1f1a7-106">уфсеттингс</span><span class="sxs-lookup"><span data-stu-id="1f1a7-106">OofSettings</span></span>](oofsettings.md)
  
```xml
<OofSettings>
   <OofState>...</OofState>
   <ExternalAudience>...</ExternalAudience>
   <Duration>...</Duration>
   <InternalReply>...</InternalReply>
   <ExternalReply>...</ExternalReply>
</OofSettings>
```

 <span data-ttu-id="1f1a7-107">**усеруфсеттингс**</span><span class="sxs-lookup"><span data-stu-id="1f1a7-107">**UserOofSettings**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1f1a7-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="1f1a7-108">Attributes and elements</span></span>

<span data-ttu-id="1f1a7-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="1f1a7-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1f1a7-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="1f1a7-110">Attributes</span></span>

<span data-ttu-id="1f1a7-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="1f1a7-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1f1a7-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="1f1a7-112">Child elements</span></span>

|<span data-ttu-id="1f1a7-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="1f1a7-113">**Element**</span></span>|<span data-ttu-id="1f1a7-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1f1a7-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1f1a7-115">уфстате</span><span class="sxs-lookup"><span data-stu-id="1f1a7-115">OofState</span></span>](oofstate.md) <br/> |<span data-ttu-id="1f1a7-116">Содержит состояние отсутствия на работе пользователя.</span><span class="sxs-lookup"><span data-stu-id="1f1a7-116">Contains the user's OOF state.</span></span>  <br/> |
|[<span data-ttu-id="1f1a7-117">екстерналаудиенце</span><span class="sxs-lookup"><span data-stu-id="1f1a7-117">ExternalAudience</span></span>](externalaudience.md) <br/> |<span data-ttu-id="1f1a7-118">Содержит значение, определяющее, кому отправляются внешние сообщения об отсутствии на работе.</span><span class="sxs-lookup"><span data-stu-id="1f1a7-118">Contains a value that determines to whom external OOF messages are sent.</span></span>  <br/> |
|[<span data-ttu-id="1f1a7-119">Продолжительность (Усеруфсеттингс)</span><span class="sxs-lookup"><span data-stu-id="1f1a7-119">Duration (UserOofSettings)</span></span>](duration-useroofsettings.md) <br/> |<span data-ttu-id="1f1a7-120">Содержит время, в течение которого состояние отсутствия на работе включено, если для элемента [уфстате](oofstate.md) задано значение " **запланировано**".</span><span class="sxs-lookup"><span data-stu-id="1f1a7-120">Contains the duration for which the OOF status is enabled if the [OofState](oofstate.md) element is set to **Scheduled**.</span></span> <span data-ttu-id="1f1a7-121">Если для элемента [уфстате](oofstate.md) задано значение **Enabled** или **disabled**, значение этого элемента игнорируется.</span><span class="sxs-lookup"><span data-stu-id="1f1a7-121">If the [OofState](oofstate.md) element is set to **Enabled** or **Disabled**, the value of this element is ignored.</span></span>  <br/> |
|[<span data-ttu-id="1f1a7-122">интерналрепли</span><span class="sxs-lookup"><span data-stu-id="1f1a7-122">InternalReply</span></span>](internalreply.md) <br/> |<span data-ttu-id="1f1a7-123">Содержит ответ о нерабочем месте, отправленный другим пользователям в домене пользователя или доверенном домене.</span><span class="sxs-lookup"><span data-stu-id="1f1a7-123">Contains the OOF response sent to other users in the user's domain or trusted domain.</span></span>  <br/> |
|[<span data-ttu-id="1f1a7-124">екстерналрепли</span><span class="sxs-lookup"><span data-stu-id="1f1a7-124">ExternalReply</span></span>](externalreply.md) <br/> |<span data-ttu-id="1f1a7-125">Содержит ответ о нерабочем месте, отправленный на адреса, не входящие в домен получателя или доверенные домены.</span><span class="sxs-lookup"><span data-stu-id="1f1a7-125">Contains the OOF response sent to addresses outside the recipient's domain or trusted domains.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1f1a7-126">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="1f1a7-126">Parent elements</span></span>

|<span data-ttu-id="1f1a7-127">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="1f1a7-127">**Element**</span></span>|<span data-ttu-id="1f1a7-128">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1f1a7-128">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1f1a7-129">жетусеруфсеттингсреспонсе</span><span class="sxs-lookup"><span data-stu-id="1f1a7-129">GetUserOofSettingsResponse</span></span>](getuseroofsettingsresponse.md) <br/> |<span data-ttu-id="1f1a7-130">Содержит результаты ответа и параметры отсутствия на отсутствие для пользователя.</span><span class="sxs-lookup"><span data-stu-id="1f1a7-130">Contains the response results and the OOF settings for a user.</span></span>  <br/> <span data-ttu-id="1f1a7-131">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="1f1a7-131">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserOofSettingsResponse` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="1f1a7-132">Примечания</span><span class="sxs-lookup"><span data-stu-id="1f1a7-132">Remarks</span></span>

<span data-ttu-id="1f1a7-133">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="1f1a7-133">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1f1a7-134">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="1f1a7-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1f1a7-135">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="1f1a7-135">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1f1a7-136">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="1f1a7-136">Schema Name</span></span>  <br/> |<span data-ttu-id="1f1a7-137">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="1f1a7-137">Messages schema</span></span>  <br/> |
|<span data-ttu-id="1f1a7-138">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="1f1a7-138">Validation File</span></span>  <br/> |<span data-ttu-id="1f1a7-139">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="1f1a7-139">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1f1a7-140">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="1f1a7-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="1f1a7-141">False</span><span class="sxs-lookup"><span data-stu-id="1f1a7-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1f1a7-142">См. также</span><span class="sxs-lookup"><span data-stu-id="1f1a7-142">See also</span></span>



[<span data-ttu-id="1f1a7-143">Операция GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="1f1a7-143">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md)
  
[<span data-ttu-id="1f1a7-144">Операция SetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="1f1a7-144">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)

