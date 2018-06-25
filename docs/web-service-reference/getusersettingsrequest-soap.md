---
title: GetUserSettingsRequest (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 832a9211-d2d5-4a49-bcb3-1dc6dc3904ed
description: Элемент GetUserSettingsRequest представляет запрос для получения параметров указанного для одного или нескольких пользователей.
ms.openlocfilehash: dc22570144a6947dc6e7042326c7416422680cc1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833702"
---
# <a name="getusersettingsrequest-soap"></a><span data-ttu-id="74f91-103">GetUserSettingsRequest (SOAP)</span><span class="sxs-lookup"><span data-stu-id="74f91-103">GetUserSettingsRequest (SOAP)</span></span>

<span data-ttu-id="74f91-104">Элемент **GetUserSettingsRequest** представляет запрос для получения параметров указанного для одного или нескольких пользователей.</span><span class="sxs-lookup"><span data-stu-id="74f91-104">The **GetUserSettingsRequest** element represents a request to retrieve specified settings for one or more users.</span></span> 
  
```XML
<GetUserSettingsRequest>
   <Users/>
   <RequestedSettings/>
   <RequestedVersion/>
</GetUserSettingsRequest>
```

 <span data-ttu-id="74f91-105">**GetUserSettingsRequest**</span><span class="sxs-lookup"><span data-stu-id="74f91-105">**GetUserSettingsRequest**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="74f91-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="74f91-106">Attributes and elements</span></span>

<span data-ttu-id="74f91-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="74f91-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="74f91-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="74f91-108">Attributes</span></span>

<span data-ttu-id="74f91-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="74f91-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="74f91-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="74f91-110">Child elements</span></span>

|<span data-ttu-id="74f91-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="74f91-111">**Element**</span></span>|<span data-ttu-id="74f91-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="74f91-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="74f91-113">Пользователи (SOAP)</span><span class="sxs-lookup"><span data-stu-id="74f91-113">Users (SOAP)</span></span>](users-soap.md) <br/> |<span data-ttu-id="74f91-114">Представляет коллекцию адреса электронной почты пользователей, для которых требуется извлечь параметры.</span><span class="sxs-lookup"><span data-stu-id="74f91-114">Represents a collection of e-mail addresses of the users for whom settings should be retrieved.</span></span>  <br/> |
|[<span data-ttu-id="74f91-115">RequestedSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="74f91-115">RequestedSettings (SOAP)</span></span>](requestedsettings-soap.md) <br/> |<span data-ttu-id="74f91-116">Содержит имена параметров запрошенные конфигурации.</span><span class="sxs-lookup"><span data-stu-id="74f91-116">Contains the names of the requested configuration settings.</span></span>  <br/> |
|[<span data-ttu-id="74f91-117">RequestedVersion (SOAP)</span><span class="sxs-lookup"><span data-stu-id="74f91-117">RequestedVersion (SOAP)</span></span>](requestedversion-soap.md) <br/> |<span data-ttu-id="74f91-118">Указывает версию определенного сервера, который хотите использовать поставщик.</span><span class="sxs-lookup"><span data-stu-id="74f91-118">Specifies the specific server version that the provider would like to use.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="74f91-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="74f91-119">Parent elements</span></span>

<span data-ttu-id="74f91-120">Нет.</span><span class="sxs-lookup"><span data-stu-id="74f91-120">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="74f91-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="74f91-121">Text value</span></span>

<span data-ttu-id="74f91-122">Нет.</span><span class="sxs-lookup"><span data-stu-id="74f91-122">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="74f91-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="74f91-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="74f91-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="74f91-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="74f91-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="74f91-125">Schema Name</span></span>  <br/> |<span data-ttu-id="74f91-126">Схема службы автообнаружения</span><span class="sxs-lookup"><span data-stu-id="74f91-126">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="74f91-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="74f91-127">Validation File</span></span>  <br/> |<span data-ttu-id="74f91-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="74f91-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="74f91-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="74f91-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="74f91-130">True</span><span class="sxs-lookup"><span data-stu-id="74f91-130">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="74f91-131">См. также</span><span class="sxs-lookup"><span data-stu-id="74f91-131">See also</span></span>



[<span data-ttu-id="74f91-132">Операция GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="74f91-132">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)

