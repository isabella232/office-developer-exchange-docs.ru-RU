---
title: Жетусерсеттингсрекуест (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 832a9211-d2d5-4a49-bcb3-1dc6dc3904ed
description: Элемент Жетусерсеттингсрекуест представляет запрос на получение указанных параметров для одного или нескольких пользователей.
ms.openlocfilehash: 353facb5d0bbf922a23b33cbaf6f9d2e7d82bd6b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530164"
---
# <a name="getusersettingsrequest-soap"></a><span data-ttu-id="1826d-103">Жетусерсеттингсрекуест (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1826d-103">GetUserSettingsRequest (SOAP)</span></span>

<span data-ttu-id="1826d-104">Элемент **жетусерсеттингсрекуест** представляет запрос на получение указанных параметров для одного или нескольких пользователей.</span><span class="sxs-lookup"><span data-stu-id="1826d-104">The **GetUserSettingsRequest** element represents a request to retrieve specified settings for one or more users.</span></span> 
  
```XML
<GetUserSettingsRequest>
   <Users/>
   <RequestedSettings/>
   <RequestedVersion/>
</GetUserSettingsRequest>
```

 <span data-ttu-id="1826d-105">**жетусерсеттингсрекуест**</span><span class="sxs-lookup"><span data-stu-id="1826d-105">**GetUserSettingsRequest**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1826d-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="1826d-106">Attributes and elements</span></span>

<span data-ttu-id="1826d-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="1826d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1826d-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="1826d-108">Attributes</span></span>

<span data-ttu-id="1826d-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="1826d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1826d-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="1826d-110">Child elements</span></span>

|<span data-ttu-id="1826d-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="1826d-111">**Element**</span></span>|<span data-ttu-id="1826d-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1826d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1826d-113">Пользователи (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1826d-113">Users (SOAP)</span></span>](users-soap.md) <br/> |<span data-ttu-id="1826d-114">Представляет коллекцию адресов электронной почты пользователей, для которых необходимо извлечь параметры.</span><span class="sxs-lookup"><span data-stu-id="1826d-114">Represents a collection of e-mail addresses of the users for whom settings should be retrieved.</span></span>  <br/> |
|[<span data-ttu-id="1826d-115">Рекуестедсеттингс (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1826d-115">RequestedSettings (SOAP)</span></span>](requestedsettings-soap.md) <br/> |<span data-ttu-id="1826d-116">Содержит имена запрошенных параметров конфигурации.</span><span class="sxs-lookup"><span data-stu-id="1826d-116">Contains the names of the requested configuration settings.</span></span>  <br/> |
|[<span data-ttu-id="1826d-117">Рекуестедверсион (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1826d-117">RequestedVersion (SOAP)</span></span>](requestedversion-soap.md) <br/> |<span data-ttu-id="1826d-118">Указывает конкретную версию сервера, которую необходимо использовать поставщику.</span><span class="sxs-lookup"><span data-stu-id="1826d-118">Specifies the specific server version that the provider would like to use.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1826d-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="1826d-119">Parent elements</span></span>

<span data-ttu-id="1826d-120">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="1826d-120">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="1826d-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="1826d-121">Text value</span></span>

<span data-ttu-id="1826d-122">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="1826d-122">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1826d-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="1826d-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1826d-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="1826d-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="1826d-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="1826d-125">Schema Name</span></span>  <br/> |<span data-ttu-id="1826d-126">Схема автообнаружения</span><span class="sxs-lookup"><span data-stu-id="1826d-126">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="1826d-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="1826d-127">Validation File</span></span>  <br/> |<span data-ttu-id="1826d-128">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="1826d-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1826d-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="1826d-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="1826d-130">True</span><span class="sxs-lookup"><span data-stu-id="1826d-130">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1826d-131">См. также</span><span class="sxs-lookup"><span data-stu-id="1826d-131">See also</span></span>



[<span data-ttu-id="1826d-132">Операция GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1826d-132">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)

