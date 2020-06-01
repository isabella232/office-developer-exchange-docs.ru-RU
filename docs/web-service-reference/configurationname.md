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
ms.openlocfilehash: 5e1216253a633af643dbd276827842dbe2db5d5f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463925"
---
# <a name="configurationname"></a><span data-ttu-id="ff9b6-103">Указав</span><span class="sxs-lookup"><span data-stu-id="ff9b6-103">ConfigurationName</span></span>

<span data-ttu-id="ff9b6-104">Элемент **configurationName** указывает запрошенные конфигурации службы по имени.</span><span class="sxs-lookup"><span data-stu-id="ff9b6-104">The **ConfigurationName** element specifies the requested service configurations by name.</span></span> 
  
```xml
<ConfigurationName>MailTips or UnifiedMessagingConfiguration or ProtectionRules</ConfigurationName>
```

 <span data-ttu-id="ff9b6-105">**сервицеконфигуратионтипе**</span><span class="sxs-lookup"><span data-stu-id="ff9b6-105">**ServiceConfigurationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ff9b6-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="ff9b6-106">Attributes and elements</span></span>

<span data-ttu-id="ff9b6-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="ff9b6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ff9b6-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="ff9b6-108">Attributes</span></span>

<span data-ttu-id="ff9b6-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="ff9b6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ff9b6-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="ff9b6-110">Child elements</span></span>

<span data-ttu-id="ff9b6-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="ff9b6-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ff9b6-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="ff9b6-112">Parent elements</span></span>

|<span data-ttu-id="ff9b6-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ff9b6-113">**Element**</span></span>|<span data-ttu-id="ff9b6-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ff9b6-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ff9b6-115">рекуестедконфигуратион</span><span class="sxs-lookup"><span data-stu-id="ff9b6-115">RequestedConfiguration</span></span>](requestedconfiguration.md) <br/> |<span data-ttu-id="ff9b6-116">Содержит требуемые конфигурации службы.</span><span class="sxs-lookup"><span data-stu-id="ff9b6-116">Contains the requested service configurations.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ff9b6-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="ff9b6-117">Text value</span></span>

<span data-ttu-id="ff9b6-118">В следующей таблице приведены возможные значения для элемента **configurationName** .</span><span class="sxs-lookup"><span data-stu-id="ff9b6-118">The following table lists the possible values for the **ConfigurationName** element.</span></span> 
  
<span data-ttu-id="ff9b6-119">**Значения элементов ConfigurationName**</span><span class="sxs-lookup"><span data-stu-id="ff9b6-119">**ConfigurationName element values**</span></span>

|<span data-ttu-id="ff9b6-120">**Значение**</span><span class="sxs-lookup"><span data-stu-id="ff9b6-120">**Value**</span></span>|<span data-ttu-id="ff9b6-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ff9b6-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ff9b6-122">Подсказки</span><span class="sxs-lookup"><span data-stu-id="ff9b6-122">MailTips</span></span>  <br/> |<span data-ttu-id="ff9b6-123">Определяет конфигурацию службы почтовых подсказок.</span><span class="sxs-lookup"><span data-stu-id="ff9b6-123">Identifies the MailTips service configuration.</span></span>  <br/> |
|<span data-ttu-id="ff9b6-124">унифиедмессагингконфигуратион</span><span class="sxs-lookup"><span data-stu-id="ff9b6-124">UnifiedMessagingConfiguration</span></span>  <br/> |<span data-ttu-id="ff9b6-125">Определяет конфигурацию службы единой системы обмена сообщениями.</span><span class="sxs-lookup"><span data-stu-id="ff9b6-125">Identifies the Unified Messaging service configuration.</span></span>  <br/> |
|<span data-ttu-id="ff9b6-126">протектионрулес</span><span class="sxs-lookup"><span data-stu-id="ff9b6-126">ProtectionRules</span></span>  <br/> |<span data-ttu-id="ff9b6-127">Определяет конфигурацию службы правил защиты.</span><span class="sxs-lookup"><span data-stu-id="ff9b6-127">Identifies the Protection Rules service configuration.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ff9b6-128">Примечания</span><span class="sxs-lookup"><span data-stu-id="ff9b6-128">Remarks</span></span>

<span data-ttu-id="ff9b6-129">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="ff9b6-129">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ff9b6-130">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="ff9b6-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ff9b6-131">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="ff9b6-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ff9b6-132">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="ff9b6-132">Schema Name</span></span>  <br/> |<span data-ttu-id="ff9b6-133">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="ff9b6-133">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ff9b6-134">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="ff9b6-134">Validation File</span></span>  <br/> |<span data-ttu-id="ff9b6-135">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="ff9b6-135">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ff9b6-136">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="ff9b6-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="ff9b6-137">False</span><span class="sxs-lookup"><span data-stu-id="ff9b6-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ff9b6-138">См. также</span><span class="sxs-lookup"><span data-stu-id="ff9b6-138">See also</span></span>



- [<span data-ttu-id="ff9b6-139">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="ff9b6-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

