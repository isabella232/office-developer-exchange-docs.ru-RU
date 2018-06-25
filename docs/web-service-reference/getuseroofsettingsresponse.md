---
title: GetUserOofSettingsResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetUserOofSettingsResponse
api_type:
- schema
ms.assetid: 011cb38b-da3c-4b1b-8836-a6b212b511f6
description: Элемент GetUserOofSettingsResponse содержит параметры об отсутствии на работе Office (OOF) для пользователя и ответное сообщение.
ms.openlocfilehash: dc63b6d54471973ce5961a5a5ad6a23f6521fc0e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833693"
---
# <a name="getuseroofsettingsresponse"></a><span data-ttu-id="4b6f9-103">GetUserOofSettingsResponse</span><span class="sxs-lookup"><span data-stu-id="4b6f9-103">GetUserOofSettingsResponse</span></span>

<span data-ttu-id="4b6f9-104">Элемент **GetUserOofSettingsResponse** содержит параметры об отсутствии на работе Office (OOF) для пользователя и ответное сообщение.</span><span class="sxs-lookup"><span data-stu-id="4b6f9-104">The **GetUserOofSettingsResponse** element contains the response message and the Out of Office (OOF) settings for a user.</span></span> 
  
```xml
<GetUserOofSettingsResponse>
   <ResponseMessage>...</ResponseMessage>
   <OofSettings>...</OofSettings>
   <AllowExternalOof>...</AllowExternalOof>
</GetUserOofSettingsResponse>
```

 <span data-ttu-id="4b6f9-105">**GetUserOofSettingsResponse**</span><span class="sxs-lookup"><span data-stu-id="4b6f9-105">**GetUserOofSettingsResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4b6f9-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="4b6f9-106">Attributes and elements</span></span>

<span data-ttu-id="4b6f9-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="4b6f9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4b6f9-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="4b6f9-108">Attributes</span></span>

<span data-ttu-id="4b6f9-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="4b6f9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4b6f9-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="4b6f9-110">Child elements</span></span>

|<span data-ttu-id="4b6f9-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4b6f9-111">**Element**</span></span>|<span data-ttu-id="4b6f9-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4b6f9-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4b6f9-113">ResponseMessage</span><span class="sxs-lookup"><span data-stu-id="4b6f9-113">ResponseMessage</span></span>](responsemessage.md) <br/> |<span data-ttu-id="4b6f9-114">Содержит описательные сведения о состоянии ответа.</span><span class="sxs-lookup"><span data-stu-id="4b6f9-114">Provides descriptive information about the response status.</span></span>  <br/> |
|[<span data-ttu-id="4b6f9-115">OofSettings</span><span class="sxs-lookup"><span data-stu-id="4b6f9-115">OofSettings</span></span>](oofsettings.md) <br/> |<span data-ttu-id="4b6f9-116">Содержит параметры об отсутствии на работе.</span><span class="sxs-lookup"><span data-stu-id="4b6f9-116">Contains the OOF settings.</span></span>  <br/> |
|[<span data-ttu-id="4b6f9-117">AllowExternalOof</span><span class="sxs-lookup"><span data-stu-id="4b6f9-117">AllowExternalOof</span></span>](allowexternaloof.md) <br/> |<span data-ttu-id="4b6f9-118">Содержит значение, указывающее которому отправляются внешних сообщений об отсутствии на работе.</span><span class="sxs-lookup"><span data-stu-id="4b6f9-118">Contains a value that identifies to whom external OOF messages are sent.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4b6f9-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="4b6f9-119">Parent elements</span></span>

<span data-ttu-id="4b6f9-120">Нет.</span><span class="sxs-lookup"><span data-stu-id="4b6f9-120">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="4b6f9-121">Замечания</span><span class="sxs-lookup"><span data-stu-id="4b6f9-121">Remarks</span></span>

<span data-ttu-id="4b6f9-122">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="4b6f9-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4b6f9-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="4b6f9-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4b6f9-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="4b6f9-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4b6f9-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="4b6f9-125">Schema Name</span></span>  <br/> |<span data-ttu-id="4b6f9-126">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="4b6f9-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="4b6f9-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="4b6f9-127">Validation File</span></span>  <br/> |<span data-ttu-id="4b6f9-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="4b6f9-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4b6f9-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="4b6f9-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="4b6f9-130">False</span><span class="sxs-lookup"><span data-stu-id="4b6f9-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4b6f9-131">См. также</span><span class="sxs-lookup"><span data-stu-id="4b6f9-131">See also</span></span>



[<span data-ttu-id="4b6f9-132">Операция GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="4b6f9-132">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md)
  
[<span data-ttu-id="4b6f9-133">Операция SetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="4b6f9-133">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)

