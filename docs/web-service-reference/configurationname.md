---
title: Указав
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConfigurationName
api_type:
- schema
ms.assetid: 3b524a2f-9c6b-4550-9f3d-f78d176b0f7b
description: Элемент ConfigurationName указывает запрошенные конфигурации службы по имени.
ms.openlocfilehash: a03a0bc0ab7ecbc1c2aec31f864503ee0f560908
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761709"
---
# <a name="configurationname"></a><span data-ttu-id="505d4-103">Указав</span><span class="sxs-lookup"><span data-stu-id="505d4-103">ConfigurationName</span></span>

<span data-ttu-id="505d4-104">Элемент **configurationName** указывает запрошенные конфигурации службы по имени.</span><span class="sxs-lookup"><span data-stu-id="505d4-104">The **ConfigurationName** element specifies the requested service configurations by name.</span></span> 
  
```xml
<ConfigurationName>MailTips or UnifiedMessagingConfiguration or ProtectionRules</ConfigurationName>
```

 <span data-ttu-id="505d4-105">**сервицеконфигуратионтипе**</span><span class="sxs-lookup"><span data-stu-id="505d4-105">**ServiceConfigurationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="505d4-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="505d4-106">Attributes and elements</span></span>

<span data-ttu-id="505d4-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="505d4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="505d4-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="505d4-108">Attributes</span></span>

<span data-ttu-id="505d4-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="505d4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="505d4-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="505d4-110">Child elements</span></span>

<span data-ttu-id="505d4-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="505d4-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="505d4-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="505d4-112">Parent elements</span></span>

|<span data-ttu-id="505d4-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="505d4-113">**Element**</span></span>|<span data-ttu-id="505d4-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="505d4-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="505d4-115">рекуестедконфигуратион</span><span class="sxs-lookup"><span data-stu-id="505d4-115">RequestedConfiguration</span></span>](requestedconfiguration.md) <br/> |<span data-ttu-id="505d4-116">Содержит требуемые конфигурации службы.</span><span class="sxs-lookup"><span data-stu-id="505d4-116">Contains the requested service configurations.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="505d4-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="505d4-117">Text value</span></span>

<span data-ttu-id="505d4-118">В следующей таблице приведены возможные значения для элемента **configurationName** .</span><span class="sxs-lookup"><span data-stu-id="505d4-118">The following table lists the possible values for the **ConfigurationName** element.</span></span> 
  
<span data-ttu-id="505d4-119">**Значения элементов ConfigurationName**</span><span class="sxs-lookup"><span data-stu-id="505d4-119">**ConfigurationName element values**</span></span>

|<span data-ttu-id="505d4-120">**Значение**</span><span class="sxs-lookup"><span data-stu-id="505d4-120">**Value**</span></span>|<span data-ttu-id="505d4-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="505d4-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="505d4-122">Подсказки</span><span class="sxs-lookup"><span data-stu-id="505d4-122">MailTips</span></span>  <br/> |<span data-ttu-id="505d4-123">Определяет конфигурацию службы почтовых подсказок.</span><span class="sxs-lookup"><span data-stu-id="505d4-123">Identifies the MailTips service configuration.</span></span>  <br/> |
|<span data-ttu-id="505d4-124">унифиедмессагингконфигуратион</span><span class="sxs-lookup"><span data-stu-id="505d4-124">UnifiedMessagingConfiguration</span></span>  <br/> |<span data-ttu-id="505d4-125">Определяет конфигурацию службы единой системы обмена сообщениями.</span><span class="sxs-lookup"><span data-stu-id="505d4-125">Identifies the Unified Messaging service configuration.</span></span>  <br/> |
|<span data-ttu-id="505d4-126">протектионрулес</span><span class="sxs-lookup"><span data-stu-id="505d4-126">ProtectionRules</span></span>  <br/> |<span data-ttu-id="505d4-127">Определяет конфигурацию службы правил защиты.</span><span class="sxs-lookup"><span data-stu-id="505d4-127">Identifies the Protection Rules service configuration.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="505d4-128">Примечания</span><span class="sxs-lookup"><span data-stu-id="505d4-128">Remarks</span></span>

<span data-ttu-id="505d4-129">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="505d4-129">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="505d4-130">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="505d4-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="505d4-131">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="505d4-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="505d4-132">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="505d4-132">Schema Name</span></span>  <br/> |<span data-ttu-id="505d4-133">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="505d4-133">Messages schema</span></span>  <br/> |
|<span data-ttu-id="505d4-134">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="505d4-134">Validation File</span></span>  <br/> |<span data-ttu-id="505d4-135">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="505d4-135">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="505d4-136">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="505d4-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="505d4-137">False</span><span class="sxs-lookup"><span data-stu-id="505d4-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="505d4-138">См. также</span><span class="sxs-lookup"><span data-stu-id="505d4-138">See also</span></span>



- [<span data-ttu-id="505d4-139">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="505d4-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

