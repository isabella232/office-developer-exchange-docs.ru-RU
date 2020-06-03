---
title: Жетусерсеттингсреспонсе (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: e7cd470d-5861-41e7-9e66-73ef7a59700b
description: Элемент Жетусерсеттингсреспонсе представляет ответ на запрос операции GetUserSettings (SOAP).
ms.openlocfilehash: a41a195a003789ddaef81f844e47aad689df0937
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530150"
---
# <a name="getusersettingsresponse-soap"></a><span data-ttu-id="23e53-103">Жетусерсеттингсреспонсе (SOAP)</span><span class="sxs-lookup"><span data-stu-id="23e53-103">GetUserSettingsResponse (SOAP)</span></span>

<span data-ttu-id="23e53-104">Элемент **жетусерсеттингсреспонсе** представляет ответ на запрос [операции GetUserSettings (SOAP)](getusersettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="23e53-104">The **GetUserSettingsResponse** element represents a response to a [GetUserSettings operation (SOAP)](getusersettings-operation-soap.md) request.</span></span> 
  
```XML
<GetUserSettingsResponse>
   <ErrorCode/>
   <ErrorMessage/>
   <UserResponses/>
</GetUserSettingsResponse>
```

 <span data-ttu-id="23e53-105">**жетусерсеттингсреспонсе**</span><span class="sxs-lookup"><span data-stu-id="23e53-105">**GetUserSettingsResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="23e53-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="23e53-106">Attributes and elements</span></span>

<span data-ttu-id="23e53-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="23e53-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="23e53-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="23e53-108">Attributes</span></span>

<span data-ttu-id="23e53-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="23e53-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="23e53-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="23e53-110">Child elements</span></span>

|<span data-ttu-id="23e53-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="23e53-111">**Element**</span></span>|<span data-ttu-id="23e53-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="23e53-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="23e53-113">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="23e53-113">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="23e53-114">Представляет код ошибки, возвращенный службой автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="23e53-114">Represents an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="23e53-115">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="23e53-115">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="23e53-116">Представляет сообщение, связанное с кодом ошибки, возвращаемым службой автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="23e53-116">Represents a message that is associated with an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="23e53-117">Усерреспонсес (SOAP)</span><span class="sxs-lookup"><span data-stu-id="23e53-117">UserResponses (SOAP)</span></span>](userresponses-soap.md) <br/> |<span data-ttu-id="23e53-118">Содержит параметры конфигурации для каждого запрошенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="23e53-118">Contains the configuration settings for each requested user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="23e53-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="23e53-119">Parent elements</span></span>

<span data-ttu-id="23e53-120">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="23e53-120">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="23e53-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="23e53-121">Text value</span></span>

<span data-ttu-id="23e53-122">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="23e53-122">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="23e53-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="23e53-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="23e53-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="23e53-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="23e53-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="23e53-125">Schema Name</span></span>  <br/> |<span data-ttu-id="23e53-126">Схема автообнаружения</span><span class="sxs-lookup"><span data-stu-id="23e53-126">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="23e53-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="23e53-127">Validation File</span></span>  <br/> |<span data-ttu-id="23e53-128">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="23e53-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="23e53-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="23e53-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="23e53-130">True</span><span class="sxs-lookup"><span data-stu-id="23e53-130">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="23e53-131">См. также</span><span class="sxs-lookup"><span data-stu-id="23e53-131">See also</span></span>



[<span data-ttu-id="23e53-132">Операция GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="23e53-132">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)

