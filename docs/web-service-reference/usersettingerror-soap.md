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
ms.openlocfilehash: 61603038ce93780f690d72226b1356b239d2002d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468609"
---
# <a name="usersettingerror-soap"></a><span data-ttu-id="d837c-103">Усерсеттинжеррор (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d837c-103">UserSettingError (SOAP)</span></span>

<span data-ttu-id="d837c-104">Элемент **усерсеттинжеррор** представляет ошибку, которая возвращается в результате попытки получить параметр пользователя.</span><span class="sxs-lookup"><span data-stu-id="d837c-104">The **UserSettingError** element represents an error that is returned as a result of an attempt to get a user setting.</span></span> 
  
```XML
<UserSettingError>
    <ErrorCode/>
    <ErrorMessage/>
    <SettingName/>
</UserSettingError>
```

 <span data-ttu-id="d837c-105">**усерсеттинжеррор**</span><span class="sxs-lookup"><span data-stu-id="d837c-105">**UserSettingError**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d837c-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d837c-106">Attributes and elements</span></span>

<span data-ttu-id="d837c-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="d837c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d837c-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d837c-108">Attributes</span></span>

<span data-ttu-id="d837c-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="d837c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d837c-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d837c-110">Child elements</span></span>

|<span data-ttu-id="d837c-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d837c-111">**Element**</span></span>|<span data-ttu-id="d837c-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d837c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d837c-113">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d837c-113">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="d837c-114">Представляет код ошибки, возвращенный службой автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="d837c-114">Represents an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="d837c-115">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d837c-115">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="d837c-116">Респресентс сообщение, связанное с кодом ошибки, возвращаемым службой автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="d837c-116">Respresents a message associated with an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="d837c-117">Свойства settingname (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d837c-117">SettingName (SOAP)</span></span>](settingname-soap.md) <br/> |<span data-ttu-id="d837c-118">Представляет имя параметра пользователя.</span><span class="sxs-lookup"><span data-stu-id="d837c-118">Represents the name of a user setting.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d837c-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d837c-119">Parent elements</span></span>

|<span data-ttu-id="d837c-120">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d837c-120">**Element**</span></span>|<span data-ttu-id="d837c-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d837c-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d837c-122">Усерсеттинжеррорс (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d837c-122">UserSettingErrors (SOAP)</span></span>](usersettingerrors-soap.md) <br/> |<span data-ttu-id="d837c-123">Представляет коллекцию сведений о параметрах, которые не удалось вернуть.</span><span class="sxs-lookup"><span data-stu-id="d837c-123">Represents a collection of information about settings that could not be returned.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d837c-124">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="d837c-124">Text value</span></span>

<span data-ttu-id="d837c-125">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="d837c-125">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d837c-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d837c-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d837c-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d837c-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="d837c-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d837c-128">Schema Name</span></span>  <br/> |<span data-ttu-id="d837c-129">Схема автообнаружения</span><span class="sxs-lookup"><span data-stu-id="d837c-129">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="d837c-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d837c-130">Validation File</span></span>  <br/> |<span data-ttu-id="d837c-131">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="d837c-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d837c-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d837c-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="d837c-133">True</span><span class="sxs-lookup"><span data-stu-id="d837c-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d837c-134">См. также</span><span class="sxs-lookup"><span data-stu-id="d837c-134">See also</span></span>



[<span data-ttu-id="d837c-135">XML-элементы автообнаружения SOAP для Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="d837c-135">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)

