---
title: Пользователи (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 4e051617-4eea-47d0-871a-ea1f17a0f711
description: Элемент Users представляет коллекцию адресов электронной почты пользователей, для которых необходимо извлечь параметры.
ms.openlocfilehash: 851447a2918e365b7c5d8812a61c9d425d26ffa2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461900"
---
# <a name="users-soap"></a><span data-ttu-id="175de-103">Пользователи (SOAP)</span><span class="sxs-lookup"><span data-stu-id="175de-103">Users (SOAP)</span></span>

<span data-ttu-id="175de-104">Элемент **Users** представляет коллекцию адресов электронной почты пользователей, для которых необходимо извлечь параметры.</span><span class="sxs-lookup"><span data-stu-id="175de-104">The **Users** element represents a collection of e-mail addresses of the users for whom settings should be retrieved.</span></span> 
  
```XML
<Users>
   <User/>
</Users>
```

 <span data-ttu-id="175de-105">**Пользовательские**</span><span class="sxs-lookup"><span data-stu-id="175de-105">**Users**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="175de-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="175de-106">Attributes and elements</span></span>

<span data-ttu-id="175de-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="175de-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="175de-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="175de-108">Attributes</span></span>

<span data-ttu-id="175de-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="175de-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="175de-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="175de-110">Child elements</span></span>

|<span data-ttu-id="175de-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="175de-111">**Element**</span></span>|<span data-ttu-id="175de-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="175de-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="175de-113">Пользователь (SOAP)</span><span class="sxs-lookup"><span data-stu-id="175de-113">User (SOAP)</span></span>](user-soap.md) <br/> |<span data-ttu-id="175de-114">Представляет адрес электронной почты пользователя.</span><span class="sxs-lookup"><span data-stu-id="175de-114">Represents the e-mail address of a user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="175de-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="175de-115">Parent elements</span></span>

|<span data-ttu-id="175de-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="175de-116">**Element**</span></span>|<span data-ttu-id="175de-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="175de-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="175de-118">Жетусерсеттингсрекуест (SOAP)</span><span class="sxs-lookup"><span data-stu-id="175de-118">GetUserSettingsRequest (SOAP)</span></span>](getusersettingsrequest-soap.md) <br/> |<span data-ttu-id="175de-119">Представляет запрос на получение указанных параметров для одного или нескольких пользователей.</span><span class="sxs-lookup"><span data-stu-id="175de-119">Represents a request to retrieve specified settings for one or more users.</span></span>  <br/> |
|[<span data-ttu-id="175de-120">Запрос (SOAP)</span><span class="sxs-lookup"><span data-stu-id="175de-120">Request (SOAP)</span></span>](request-soap.md) <br/> |<span data-ttu-id="175de-121">Содержит запрошенные параметры конфигурации и конечных пользователей.</span><span class="sxs-lookup"><span data-stu-id="175de-121">Contains the requested configuration settings and the target users.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="175de-122">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="175de-122">Text value</span></span>

<span data-ttu-id="175de-123">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="175de-123">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="175de-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="175de-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="175de-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="175de-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="175de-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="175de-126">Schema Name</span></span>  <br/> |<span data-ttu-id="175de-127">Схема автообнаружения</span><span class="sxs-lookup"><span data-stu-id="175de-127">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="175de-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="175de-128">Validation File</span></span>  <br/> |<span data-ttu-id="175de-129">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="175de-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="175de-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="175de-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="175de-131">True</span><span class="sxs-lookup"><span data-stu-id="175de-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="175de-132">См. также</span><span class="sxs-lookup"><span data-stu-id="175de-132">See also</span></span>



[<span data-ttu-id="175de-133">Операция GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="175de-133">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)

