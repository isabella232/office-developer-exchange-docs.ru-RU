---
title: Усерсеттинжеррорс (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: a9b94bae-cab9-412d-a811-801e849ed6c5
description: Элемент Усерсеттинжеррорс представляет коллекцию сведений о параметрах, которые не удалось вернуть.
ms.openlocfilehash: a6cc0fe114bd511dc4136532986b552c28b0d5c2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467125"
---
# <a name="usersettingerrors-soap"></a><span data-ttu-id="47fb4-103">Усерсеттинжеррорс (SOAP)</span><span class="sxs-lookup"><span data-stu-id="47fb4-103">UserSettingErrors (SOAP)</span></span>

<span data-ttu-id="47fb4-104">Элемент **усерсеттинжеррорс** представляет коллекцию сведений о параметрах, которые не удалось вернуть.</span><span class="sxs-lookup"><span data-stu-id="47fb4-104">The **UserSettingErrors** element represents a collection of information about settings that could not be returned.</span></span> 
  
```XML
<UserSettingErrors>
    <UserSettingError/>
</UserSettingErrors>
```

 <span data-ttu-id="47fb4-105">**усерсеттинжеррорс**</span><span class="sxs-lookup"><span data-stu-id="47fb4-105">**UserSettingErrors**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="47fb4-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="47fb4-106">Attributes and elements</span></span>

<span data-ttu-id="47fb4-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="47fb4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="47fb4-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="47fb4-108">Attributes</span></span>

<span data-ttu-id="47fb4-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="47fb4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="47fb4-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="47fb4-110">Child elements</span></span>

|<span data-ttu-id="47fb4-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="47fb4-111">**Element**</span></span>|<span data-ttu-id="47fb4-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="47fb4-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="47fb4-113">Усерсеттинжеррор (SOAP)</span><span class="sxs-lookup"><span data-stu-id="47fb4-113">UserSettingError (SOAP)</span></span>](usersettingerror-soap.md) <br/> |<span data-ttu-id="47fb4-114">Представляет ошибку, возвращаемую при получении параметра пользователя.</span><span class="sxs-lookup"><span data-stu-id="47fb4-114">Represents an error that is returned while retrieving a user setting.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="47fb4-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="47fb4-115">Parent elements</span></span>

|<span data-ttu-id="47fb4-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="47fb4-116">**Element**</span></span>|<span data-ttu-id="47fb4-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="47fb4-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="47fb4-118">Усерреспонсе (SOAP)</span><span class="sxs-lookup"><span data-stu-id="47fb4-118">UserResponse (SOAP)</span></span>](userresponse-soap.md) <br/> |<span data-ttu-id="47fb4-119">Представляет ответ на запрос GetUserSettings для отдельного пользователя.</span><span class="sxs-lookup"><span data-stu-id="47fb4-119">Represents a response to a GetUserSettings request for an individual user.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="47fb4-120">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="47fb4-120">Text value</span></span>

<span data-ttu-id="47fb4-121">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="47fb4-121">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="47fb4-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="47fb4-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="47fb4-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="47fb4-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="47fb4-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="47fb4-124">Schema Name</span></span>  <br/> |<span data-ttu-id="47fb4-125">Схема автообнаружения</span><span class="sxs-lookup"><span data-stu-id="47fb4-125">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="47fb4-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="47fb4-126">Validation File</span></span>  <br/> |<span data-ttu-id="47fb4-127">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="47fb4-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="47fb4-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="47fb4-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="47fb4-129">True</span><span class="sxs-lookup"><span data-stu-id="47fb4-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="47fb4-130">См. также</span><span class="sxs-lookup"><span data-stu-id="47fb4-130">See also</span></span>



[<span data-ttu-id="47fb4-131">XML-элементы автообнаружения SOAP для Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="47fb4-131">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)

