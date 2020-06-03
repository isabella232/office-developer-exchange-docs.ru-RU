---
title: Action (Сетклиентекстенсионактионтипе)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c5624a87-3436-40ce-8d6b-cc01eecab64d
description: Элемент Action содержит действие, которое сервер Exchange должен выполнить в приложении.
ms.openlocfilehash: 29579e26377edacb5fb0bb8406144eeb116b8d15
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529688"
---
# <a name="action-setclientextensionactiontype"></a><span data-ttu-id="be686-103">Action (Сетклиентекстенсионактионтипе)</span><span class="sxs-lookup"><span data-stu-id="be686-103">Action (SetClientExtensionActionType)</span></span>

<span data-ttu-id="be686-104">Элемент **Action** содержит действие, которое сервер Exchange должен выполнить в приложении.</span><span class="sxs-lookup"><span data-stu-id="be686-104">The **Action** element contains the action that the Exchange server should take on an app.</span></span> 
  
```XML
<Action ActionId="" ExtensionId="">
   <ClientExtension/>
</Action>
```

 <span data-ttu-id="be686-105">**сетклиентекстенсионактионтипе**</span><span class="sxs-lookup"><span data-stu-id="be686-105">**SetClientExtensionActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="be686-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="be686-106">Attributes and elements</span></span>

<span data-ttu-id="be686-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="be686-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="be686-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="be686-108">Attributes</span></span>

|<span data-ttu-id="be686-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="be686-109">**Attribute**</span></span>|<span data-ttu-id="be686-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="be686-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="be686-111">ActionId</span><span class="sxs-lookup"><span data-stu-id="be686-111">ActionId</span></span>  <br/> |<span data-ttu-id="be686-112">Задает идентификатор действия.</span><span class="sxs-lookup"><span data-stu-id="be686-112">Specifies the identifier of the action.</span></span> <span data-ttu-id="be686-113">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="be686-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="be686-114">екстенсионид</span><span class="sxs-lookup"><span data-stu-id="be686-114">ExtensionId</span></span>  <br/> |<span data-ttu-id="be686-115">Задает идентификатор расширения.</span><span class="sxs-lookup"><span data-stu-id="be686-115">Specifies the identifier of the extension.</span></span> <span data-ttu-id="be686-116">Этот атрибут является необязательным.</span><span class="sxs-lookup"><span data-stu-id="be686-116">This attribute is optional.</span></span>  <br/> |
   
#### <a name="actionid"></a><span data-ttu-id="be686-117">ActionId</span><span class="sxs-lookup"><span data-stu-id="be686-117">ActionId</span></span>

|<span data-ttu-id="be686-118">**Значение**</span><span class="sxs-lookup"><span data-stu-id="be686-118">**Value**</span></span>|<span data-ttu-id="be686-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="be686-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="be686-120">Configure (Настроить)</span><span class="sxs-lookup"><span data-stu-id="be686-120">Configure</span></span>  <br/> |<span data-ttu-id="be686-121">Указывает действие конфигурации.</span><span class="sxs-lookup"><span data-stu-id="be686-121">Indicates a configuration action.</span></span>  <br/> |
|<span data-ttu-id="be686-122">Установка</span><span class="sxs-lookup"><span data-stu-id="be686-122">Install</span></span>  <br/> |<span data-ttu-id="be686-123">Указывает действие установки.</span><span class="sxs-lookup"><span data-stu-id="be686-123">Indicates an installation action.</span></span>  <br/> |
|<span data-ttu-id="be686-124">Uninstall</span><span class="sxs-lookup"><span data-stu-id="be686-124">Uninstall</span></span>  <br/> |<span data-ttu-id="be686-125">Указывает действие по удалению.</span><span class="sxs-lookup"><span data-stu-id="be686-125">Indicates an uninstallation action.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="be686-126">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="be686-126">Child elements</span></span>

|<span data-ttu-id="be686-127">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="be686-127">**Element**</span></span>|<span data-ttu-id="be686-128">**Описание**</span><span class="sxs-lookup"><span data-stu-id="be686-128">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="be686-129">клиентекстенсион</span><span class="sxs-lookup"><span data-stu-id="be686-129">ClientExtension</span></span>](clientextension.md) <br/> |<span data-ttu-id="be686-130">Содержит сведения о пользователях и конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="be686-130">Contains user and configuration information about an app.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="be686-131">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="be686-131">Parent elements</span></span>

|<span data-ttu-id="be686-132">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="be686-132">**Element**</span></span>|<span data-ttu-id="be686-133">**Описание**</span><span class="sxs-lookup"><span data-stu-id="be686-133">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="be686-134">Actions (Аррайофсетклиентекстенсионактионстипе)</span><span class="sxs-lookup"><span data-stu-id="be686-134">Actions (ArrayOfSetClientExtensionActionsType)</span></span>](actions-arrayofsetclientextensionactionstype.md) <br/> |<span data-ttu-id="be686-135">Указывает массив элементов **Action** .</span><span class="sxs-lookup"><span data-stu-id="be686-135">Specifies an array of **Action** elements.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="be686-136">Примечания</span><span class="sxs-lookup"><span data-stu-id="be686-136">Remarks</span></span>

<span data-ttu-id="be686-137">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="be686-137">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="be686-138">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="be686-138">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="be686-139">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="be686-139">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="be686-140">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="be686-140">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="be686-141">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="be686-141">Schema Name</span></span>  <br/> |<span data-ttu-id="be686-142">Схема типа</span><span class="sxs-lookup"><span data-stu-id="be686-142">Type schema</span></span>  <br/> |
|<span data-ttu-id="be686-143">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="be686-143">Validation File</span></span>  <br/> |<span data-ttu-id="be686-144">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="be686-144">types.xsd</span></span>  <br/> |
|<span data-ttu-id="be686-145">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="be686-145">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="be686-146">См. также</span><span class="sxs-lookup"><span data-stu-id="be686-146">See also</span></span>

- [<span data-ttu-id="be686-147">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="be686-147">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

