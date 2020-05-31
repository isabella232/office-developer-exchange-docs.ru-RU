---
title: Усерсеттинжеррор (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: abb175c5-4f38-4dcc-81e3-b511686862eb
description: Элемент Усерсеттинжеррор представляет ошибку, которая возвращается в результате попытки получить параметр пользователя.
ms.openlocfilehash: 886e0be0aa900ce3a00902c21cc115e866d0cd99
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840442"
---
# <a name="usersettingerror-soap"></a><span data-ttu-id="1ebe4-103">Усерсеттинжеррор (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1ebe4-103">UserSettingError (SOAP)</span></span>

<span data-ttu-id="1ebe4-104">Элемент **усерсеттинжеррор** представляет ошибку, которая возвращается в результате попытки получить параметр пользователя.</span><span class="sxs-lookup"><span data-stu-id="1ebe4-104">The **UserSettingError** element represents an error that is returned as a result of an attempt to get a user setting.</span></span> 
  
```XML
<UserSettingError>
    <ErrorCode/>
    <ErrorMessage/>
    <SettingName/>
</UserSettingError>
```

 <span data-ttu-id="1ebe4-105">**усерсеттинжеррор**</span><span class="sxs-lookup"><span data-stu-id="1ebe4-105">**UserSettingError**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1ebe4-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="1ebe4-106">Attributes and elements</span></span>

<span data-ttu-id="1ebe4-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="1ebe4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1ebe4-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="1ebe4-108">Attributes</span></span>

<span data-ttu-id="1ebe4-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="1ebe4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1ebe4-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="1ebe4-110">Child elements</span></span>

|<span data-ttu-id="1ebe4-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="1ebe4-111">**Element**</span></span>|<span data-ttu-id="1ebe4-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1ebe4-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1ebe4-113">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1ebe4-113">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="1ebe4-114">Представляет код ошибки, возвращенный службой автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="1ebe4-114">Represents an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="1ebe4-115">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1ebe4-115">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="1ebe4-116">Респресентс сообщение, связанное с кодом ошибки, возвращаемым службой автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="1ebe4-116">Respresents a message associated with an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="1ebe4-117">Свойства settingname (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1ebe4-117">SettingName (SOAP)</span></span>](settingname-soap.md) <br/> |<span data-ttu-id="1ebe4-118">Представляет имя параметра пользователя.</span><span class="sxs-lookup"><span data-stu-id="1ebe4-118">Represents the name of a user setting.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1ebe4-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="1ebe4-119">Parent elements</span></span>

|<span data-ttu-id="1ebe4-120">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="1ebe4-120">**Element**</span></span>|<span data-ttu-id="1ebe4-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1ebe4-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1ebe4-122">Усерсеттинжеррорс (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1ebe4-122">UserSettingErrors (SOAP)</span></span>](usersettingerrors-soap.md) <br/> |<span data-ttu-id="1ebe4-123">Представляет коллекцию сведений о параметрах, которые не удалось вернуть.</span><span class="sxs-lookup"><span data-stu-id="1ebe4-123">Represents a collection of information about settings that could not be returned.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1ebe4-124">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="1ebe4-124">Text value</span></span>

<span data-ttu-id="1ebe4-125">Нет.</span><span class="sxs-lookup"><span data-stu-id="1ebe4-125">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1ebe4-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="1ebe4-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1ebe4-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="1ebe4-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="1ebe4-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="1ebe4-128">Schema Name</span></span>  <br/> |<span data-ttu-id="1ebe4-129">Схема автообнаружения</span><span class="sxs-lookup"><span data-stu-id="1ebe4-129">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="1ebe4-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="1ebe4-130">Validation File</span></span>  <br/> |<span data-ttu-id="1ebe4-131">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="1ebe4-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1ebe4-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="1ebe4-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="1ebe4-133">True</span><span class="sxs-lookup"><span data-stu-id="1ebe4-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1ebe4-134">См. также</span><span class="sxs-lookup"><span data-stu-id="1ebe4-134">See also</span></span>



[<span data-ttu-id="1ebe4-135">XML-элементы автообнаружения SOAP для Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="1ebe4-135">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)

