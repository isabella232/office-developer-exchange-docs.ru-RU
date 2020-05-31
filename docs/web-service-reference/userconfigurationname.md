---
title: усерконфигуратионнаме
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UserConfigurationName
api_type:
- schema
ms.assetid: 6947dd03-9727-4379-9b9d-42373fa120c7
description: Элемент Усерконфигуратионнаме представляет имя объекта пользовательской конфигурации. Имя объекта конфигурации пользователя — это идентификатор объекта конфигурации пользователя.
ms.openlocfilehash: 33b3fc316a06b8088eb20a71788a9e6a3394d0d4
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354304"
---
# <a name="userconfigurationname"></a><span data-ttu-id="7cc04-104">усерконфигуратионнаме</span><span class="sxs-lookup"><span data-stu-id="7cc04-104">UserConfigurationName</span></span>

<span data-ttu-id="7cc04-105">Элемент **усерконфигуратионнаме** представляет имя объекта пользовательской конфигурации.</span><span class="sxs-lookup"><span data-stu-id="7cc04-105">The **UserConfigurationName** element represents the name of a user configuration object.</span></span> <span data-ttu-id="7cc04-106">Имя объекта конфигурации пользователя — это идентификатор объекта конфигурации пользователя.</span><span class="sxs-lookup"><span data-stu-id="7cc04-106">The user configuration object name is the identifier for a user configuration object.</span></span> 
  
```XML
<UserConfigurationName Name="">
   <FolderId/>
</UserConfigurationName>
```

```XML
<UserConfigurationName Name="">
   <DistinguishedFolderId/> 
</UserConfigurationName>
```

<span data-ttu-id="7cc04-107">**усерконфигуратионнаметипе**</span><span class="sxs-lookup"><span data-stu-id="7cc04-107">**UserConfigurationNameType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="7cc04-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="7cc04-108">Attributes and elements</span></span>

<span data-ttu-id="7cc04-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="7cc04-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7cc04-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="7cc04-110">Attributes</span></span>

|<span data-ttu-id="7cc04-111">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="7cc04-111">**Attribute**</span></span>|<span data-ttu-id="7cc04-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7cc04-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7cc04-113">**Name**</span><span class="sxs-lookup"><span data-stu-id="7cc04-113">**Name**</span></span> <br/> |<span data-ttu-id="7cc04-114">Содержит строковое значение, представляющее имя объекта конфигурации пользователя.</span><span class="sxs-lookup"><span data-stu-id="7cc04-114">Contains a string value that represents the name of a user configuration object.</span></span> <span data-ttu-id="7cc04-115">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="7cc04-115">This attribute is required.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="7cc04-116">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="7cc04-116">Child elements</span></span>

|<span data-ttu-id="7cc04-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7cc04-117">**Element**</span></span>|<span data-ttu-id="7cc04-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7cc04-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7cc04-119">FolderId</span><span class="sxs-lookup"><span data-stu-id="7cc04-119">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="7cc04-120">Представляет идентификатор папки, содержащей объект конфигурации пользователя.</span><span class="sxs-lookup"><span data-stu-id="7cc04-120">Represents the folder identifier of the folder that contains the user configuration object.</span></span>  <br/> |
|[<span data-ttu-id="7cc04-121">дистингуишедфолдерид</span><span class="sxs-lookup"><span data-stu-id="7cc04-121">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="7cc04-122">Представляет имя папки, содержащей объект конфигурации пользователя.</span><span class="sxs-lookup"><span data-stu-id="7cc04-122">Represents a distinguished folder name of the folder that contains the user configuration object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7cc04-123">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="7cc04-123">Parent elements</span></span>

|<span data-ttu-id="7cc04-124">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7cc04-124">**Element**</span></span>|<span data-ttu-id="7cc04-125">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7cc04-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7cc04-126">DeleteUserConfiguration</span><span class="sxs-lookup"><span data-stu-id="7cc04-126">DeleteUserConfiguration</span></span>](deleteuserconfiguration.md) <br/> |<span data-ttu-id="7cc04-127">Представляет запрос на удаление объекта конфигурации пользователя.</span><span class="sxs-lookup"><span data-stu-id="7cc04-127">Represents a request to delete a user configuration object.</span></span>  <br/> |
|[<span data-ttu-id="7cc04-128">GetUserConfiguration</span><span class="sxs-lookup"><span data-stu-id="7cc04-128">GetUserConfiguration</span></span>](getuserconfiguration.md) <br/> |<span data-ttu-id="7cc04-129">Представляет запрос на получение объекта конфигурации пользователя.</span><span class="sxs-lookup"><span data-stu-id="7cc04-129">Represents a request to get a user configuration object.</span></span>  <br/> |
|[<span data-ttu-id="7cc04-130">усерконфигуратион</span><span class="sxs-lookup"><span data-stu-id="7cc04-130">UserConfiguration</span></span>](userconfiguration.md) <br/> |<span data-ttu-id="7cc04-131">Определяет один объект конфигурации пользователя.</span><span class="sxs-lookup"><span data-stu-id="7cc04-131">Defines a single user configuration object.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7cc04-132">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="7cc04-132">Text value</span></span>

<span data-ttu-id="7cc04-133">Нет.</span><span class="sxs-lookup"><span data-stu-id="7cc04-133">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7cc04-134">Примечания</span><span class="sxs-lookup"><span data-stu-id="7cc04-134">Remarks</span></span>

<span data-ttu-id="7cc04-135">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="7cc04-135">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7cc04-136">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="7cc04-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7cc04-137">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="7cc04-137">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7cc04-138">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="7cc04-138">Schema Name</span></span>  <br/> |<span data-ttu-id="7cc04-139">Схема Types</span><span class="sxs-lookup"><span data-stu-id="7cc04-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="7cc04-140">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="7cc04-140">Validation File</span></span>  <br/> |<span data-ttu-id="7cc04-141">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="7cc04-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7cc04-142">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="7cc04-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="7cc04-143">False</span><span class="sxs-lookup"><span data-stu-id="7cc04-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7cc04-144">См. также</span><span class="sxs-lookup"><span data-stu-id="7cc04-144">See also</span></span>

- [<span data-ttu-id="7cc04-145">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="7cc04-145">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

