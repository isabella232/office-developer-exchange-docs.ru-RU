---
title: Действие (SetClientExtensionActionType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c5624a87-3436-40ce-8d6b-cc01eecab64d
description: Элемент Action содержит действие, которое следует выполнять на сервере Exchange на приложения.
ms.openlocfilehash: a231cedfa6e4759dabfcbecfbe9a9b851f834247
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761331"
---
# <a name="action-setclientextensionactiontype"></a><span data-ttu-id="51f20-103">Действие (SetClientExtensionActionType)</span><span class="sxs-lookup"><span data-stu-id="51f20-103">Action (SetClientExtensionActionType)</span></span>

<span data-ttu-id="51f20-104">Элемент **Action** содержит действие, которое следует выполнять на сервере Exchange на приложения.</span><span class="sxs-lookup"><span data-stu-id="51f20-104">The **Action** element contains the action that the Exchange server should take on an app.</span></span> 
  
```XML
<Action ActionId="" ExtensionId="">
   <ClientExtension/>
</Action>
```

 <span data-ttu-id="51f20-105">**SetClientExtensionActionType**</span><span class="sxs-lookup"><span data-stu-id="51f20-105">**SetClientExtensionActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="51f20-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="51f20-106">Attributes and elements</span></span>

<span data-ttu-id="51f20-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="51f20-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="51f20-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="51f20-108">Attributes</span></span>

|<span data-ttu-id="51f20-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="51f20-109">**Attribute**</span></span>|<span data-ttu-id="51f20-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="51f20-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="51f20-111">ActionId</span><span class="sxs-lookup"><span data-stu-id="51f20-111">ActionId</span></span>  <br/> |<span data-ttu-id="51f20-112">Задает идентификатор действия.</span><span class="sxs-lookup"><span data-stu-id="51f20-112">Specifies the identifier of the action.</span></span> <span data-ttu-id="51f20-113">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="51f20-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="51f20-114">ExtensionId</span><span class="sxs-lookup"><span data-stu-id="51f20-114">ExtensionId</span></span>  <br/> |<span data-ttu-id="51f20-115">Задает идентификатор данное расширение имени файла.</span><span class="sxs-lookup"><span data-stu-id="51f20-115">Specifies the identifier of the extension.</span></span> <span data-ttu-id="51f20-116">Этот атрибут является необязательным.</span><span class="sxs-lookup"><span data-stu-id="51f20-116">This attribute is optional.</span></span>  <br/> |
   
#### <a name="actionid"></a><span data-ttu-id="51f20-117">ActionId</span><span class="sxs-lookup"><span data-stu-id="51f20-117">ActionId</span></span>

|<span data-ttu-id="51f20-118">**Значение**</span><span class="sxs-lookup"><span data-stu-id="51f20-118">**Value**</span></span>|<span data-ttu-id="51f20-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="51f20-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="51f20-120">Настройка</span><span class="sxs-lookup"><span data-stu-id="51f20-120">Configure</span></span>  <br/> |<span data-ttu-id="51f20-121">Указывает действие конфигурации.</span><span class="sxs-lookup"><span data-stu-id="51f20-121">Indicates a configuration action.</span></span>  <br/> |
|<span data-ttu-id="51f20-122">Установка</span><span class="sxs-lookup"><span data-stu-id="51f20-122">Install</span></span>  <br/> |<span data-ttu-id="51f20-123">Указывает действие установки.</span><span class="sxs-lookup"><span data-stu-id="51f20-123">Indicates an installation action.</span></span>  <br/> |
|<span data-ttu-id="51f20-124">Удаление</span><span class="sxs-lookup"><span data-stu-id="51f20-124">Uninstall</span></span>  <br/> |<span data-ttu-id="51f20-125">Указывает действие удаления.</span><span class="sxs-lookup"><span data-stu-id="51f20-125">Indicates an uninstallation action.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="51f20-126">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="51f20-126">Child elements</span></span>

|<span data-ttu-id="51f20-127">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="51f20-127">**Element**</span></span>|<span data-ttu-id="51f20-128">**Описание**</span><span class="sxs-lookup"><span data-stu-id="51f20-128">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="51f20-129">ClientExtension</span><span class="sxs-lookup"><span data-stu-id="51f20-129">ClientExtension</span></span>](clientextension.md) <br/> |<span data-ttu-id="51f20-130">Содержит пользователей и конфигурации сведения о приложении.</span><span class="sxs-lookup"><span data-stu-id="51f20-130">Contains user and configuration information about an app.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="51f20-131">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="51f20-131">Parent elements</span></span>

|<span data-ttu-id="51f20-132">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="51f20-132">**Element**</span></span>|<span data-ttu-id="51f20-133">**Описание**</span><span class="sxs-lookup"><span data-stu-id="51f20-133">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="51f20-134">Действия (ArrayOfSetClientExtensionActionsType)</span><span class="sxs-lookup"><span data-stu-id="51f20-134">Actions (ArrayOfSetClientExtensionActionsType)</span></span>](actions-arrayofsetclientextensionactionstype.md) <br/> |<span data-ttu-id="51f20-135">Указывает массив элементов **Действие** .</span><span class="sxs-lookup"><span data-stu-id="51f20-135">Specifies an array of **Action** elements.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="51f20-136">Замечания</span><span class="sxs-lookup"><span data-stu-id="51f20-136">Remarks</span></span>

<span data-ttu-id="51f20-137">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="51f20-137">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="51f20-138">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="51f20-138">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="51f20-139">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="51f20-139">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="51f20-140">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="51f20-140">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="51f20-141">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="51f20-141">Schema Name</span></span>  <br/> |<span data-ttu-id="51f20-142">Схема типа</span><span class="sxs-lookup"><span data-stu-id="51f20-142">Type schema</span></span>  <br/> |
|<span data-ttu-id="51f20-143">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="51f20-143">Validation File</span></span>  <br/> |<span data-ttu-id="51f20-144">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="51f20-144">types.xsd</span></span>  <br/> |
|<span data-ttu-id="51f20-145">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="51f20-145">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="51f20-146">См. также</span><span class="sxs-lookup"><span data-stu-id="51f20-146">See also</span></span>

- [<span data-ttu-id="51f20-147">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="51f20-147">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
