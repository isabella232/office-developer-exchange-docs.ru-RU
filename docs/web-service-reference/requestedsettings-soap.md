---
title: Рекуестедсеттингс (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 8d713d22-580c-49a5-99f5-ee532443e89a
description: Элемент Рекуестедсеттингс содержит имена запрошенных параметров конфигурации.
ms.openlocfilehash: e94c02d8f92d7aaac619c58f093c536cc1a098bf
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465298"
---
# <a name="requestedsettings-soap"></a><span data-ttu-id="fa487-103">Рекуестедсеттингс (SOAP)</span><span class="sxs-lookup"><span data-stu-id="fa487-103">RequestedSettings (SOAP)</span></span>

<span data-ttu-id="fa487-104">Элемент **рекуестедсеттингс** содержит имена запрошенных параметров конфигурации.</span><span class="sxs-lookup"><span data-stu-id="fa487-104">The **RequestedSettings** element contains the names of the requested configuration settings.</span></span> 
  
```XML
<RequestedSettings>
   <Setting/>
</RequestedSettings>
```

 <span data-ttu-id="fa487-105">**рекуестедсеттингс**</span><span class="sxs-lookup"><span data-stu-id="fa487-105">**RequestedSettings**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fa487-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="fa487-106">Attributes and elements</span></span>

<span data-ttu-id="fa487-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="fa487-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fa487-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="fa487-108">Attributes</span></span>

<span data-ttu-id="fa487-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="fa487-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fa487-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="fa487-110">Child elements</span></span>

|<span data-ttu-id="fa487-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="fa487-111">**Element**</span></span>|<span data-ttu-id="fa487-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="fa487-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fa487-113">Параметр (SOAP)</span><span class="sxs-lookup"><span data-stu-id="fa487-113">Setting (SOAP)</span></span>](setting-soap.md) <br/> |<span data-ttu-id="fa487-114">Представляет параметр конфигурации, который необходимо вернуть.</span><span class="sxs-lookup"><span data-stu-id="fa487-114">Represents a configuration setting to be returned.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="fa487-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="fa487-115">Parent elements</span></span>

|<span data-ttu-id="fa487-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="fa487-116">**Element**</span></span>|<span data-ttu-id="fa487-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="fa487-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fa487-118">Жетусерсеттингсрекуест (SOAP)</span><span class="sxs-lookup"><span data-stu-id="fa487-118">GetUserSettingsRequest (SOAP)</span></span>](getusersettingsrequest-soap.md) <br/> |<span data-ttu-id="fa487-119">Представляет запрос на получение указанных параметров для одного или нескольких пользователей.</span><span class="sxs-lookup"><span data-stu-id="fa487-119">Represents a request to retrieve specified settings for one or more users.</span></span>  <br/> |
|[<span data-ttu-id="fa487-120">Запрос (SOAP)</span><span class="sxs-lookup"><span data-stu-id="fa487-120">Request (SOAP)</span></span>](request-soap.md) <br/> |<span data-ttu-id="fa487-121">Содержит запрошенные параметры конфигурации и конечных пользователей.</span><span class="sxs-lookup"><span data-stu-id="fa487-121">Contains the requested configuration settings and the target users.</span></span>  <br/> |
|[<span data-ttu-id="fa487-122">Жетдомаинсеттингсрекуест (SOAP)</span><span class="sxs-lookup"><span data-stu-id="fa487-122">GetDomainSettingsRequest (SOAP)</span></span>](getdomainsettingsrequest-soap.md) <br/> |<span data-ttu-id="fa487-123">Представляет запрос [операции жетдомаинсеттингс (SOAP)](getdomainsettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="fa487-123">Represents a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) request.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="fa487-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="fa487-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fa487-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="fa487-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="fa487-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="fa487-126">Schema Name</span></span>  <br/> |<span data-ttu-id="fa487-127">Схема автообнаружения</span><span class="sxs-lookup"><span data-stu-id="fa487-127">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="fa487-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="fa487-128">Validation File</span></span>  <br/> |<span data-ttu-id="fa487-129">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="fa487-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="fa487-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="fa487-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="fa487-131">True</span><span class="sxs-lookup"><span data-stu-id="fa487-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fa487-132">См. также</span><span class="sxs-lookup"><span data-stu-id="fa487-132">See also</span></span>



[<span data-ttu-id="fa487-133">Операция GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="fa487-133">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
  
[<span data-ttu-id="fa487-134">Операция Жетдомаинсеттингс (SOAP)</span><span class="sxs-lookup"><span data-stu-id="fa487-134">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

