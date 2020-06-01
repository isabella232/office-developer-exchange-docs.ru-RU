---
title: агента
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- agent
api_type:
- schema
ms.assetid: 0bf744a5-9d79-4c82-8ea7-45fdb3f55300
description: 'Дата последнего изменения: 17 сентября 2015 г.'
ms.openlocfilehash: a810bb229015054e0f244773760235114655a982
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455683"
---
# <a name="agent"></a><span data-ttu-id="71d6d-103">агента</span><span class="sxs-lookup"><span data-stu-id="71d6d-103">agent</span></span>
  
<span data-ttu-id="71d6d-104">**Применимо к:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="71d6d-104">**Applies to:** Exchange Server 2013</span></span>
  
<span data-ttu-id="71d6d-105">Элемент **Agent** содержит сведения о конфигурации установленного агента.</span><span class="sxs-lookup"><span data-stu-id="71d6d-105">The **agent** element contains configuration information about an installed agent.</span></span> 
  
- [<span data-ttu-id="71d6d-106">configuration</span><span class="sxs-lookup"><span data-stu-id="71d6d-106">configuration</span></span>](configuration.md) 
- [<span data-ttu-id="71d6d-107">мексрунтиме</span><span class="sxs-lookup"><span data-stu-id="71d6d-107">mexRuntime</span></span>](mexruntime.md)
- [<span data-ttu-id="71d6d-108">ажентлист</span><span class="sxs-lookup"><span data-stu-id="71d6d-108">agentList</span></span>](agentlist.md)
- [<span data-ttu-id="71d6d-109">агента</span><span class="sxs-lookup"><span data-stu-id="71d6d-109">agent</span></span>](agent.md)
  
```XML
<agent
        name=""
        baseType=""
        classFactory=""
        assemblyPath=""
        enabled="" />
</agent>
```

<span data-ttu-id="71d6d-110">**Аженттипе (complexType)**</span><span class="sxs-lookup"><span data-stu-id="71d6d-110">**agentType (complexType)**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="71d6d-111">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="71d6d-111">Attributes and elements</span></span>

<span data-ttu-id="71d6d-112">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="71d6d-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="71d6d-113">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="71d6d-113">Attributes</span></span>

|<span data-ttu-id="71d6d-114">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="71d6d-114">**Attribute**</span></span>|<span data-ttu-id="71d6d-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="71d6d-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="71d6d-116">**name**</span><span class="sxs-lookup"><span data-stu-id="71d6d-116">**name**</span></span> <br/> |<span data-ttu-id="71d6d-117">Имя, указанное при установке агента.</span><span class="sxs-lookup"><span data-stu-id="71d6d-117">The name that was specified when the agent was installed.</span></span> <span data-ttu-id="71d6d-118">Для этого атрибута требуется непустое строковое значение, содержащее не более 64 символов.</span><span class="sxs-lookup"><span data-stu-id="71d6d-118">This attribute requires a nonempty string value that contains a maximum of 64 characters.</span></span>  <br/> |
|<span data-ttu-id="71d6d-119">**baseType**</span><span class="sxs-lookup"><span data-stu-id="71d6d-119">**baseType**</span></span> <br/> |<span data-ttu-id="71d6d-120">Полное имя класса, который является производным от агента, включая пространство имен.</span><span class="sxs-lookup"><span data-stu-id="71d6d-120">The full name, including the namespace, of the class from which the agent derives.</span></span> <span data-ttu-id="71d6d-121">Для этого атрибута требуется непустое строковое значение, содержащее по крайней мере один символ.</span><span class="sxs-lookup"><span data-stu-id="71d6d-121">This attribute requires a nonempty string value that contains at least one character.</span></span>  <br/> |
|<span data-ttu-id="71d6d-122">**классфактори**</span><span class="sxs-lookup"><span data-stu-id="71d6d-122">**classFactory**</span></span> <br/> |<span data-ttu-id="71d6d-123">Полное имя (включая пространство имен) класса, который реализует фабрику агентов, которая создает экземпляры агента.</span><span class="sxs-lookup"><span data-stu-id="71d6d-123">The full name, including the namespace, of the class that implements the agent factory that creates instances of the agent.</span></span> <span data-ttu-id="71d6d-124">Этот атрибут должен содержать полное имя класса, реализующего фабрику агентов, которая создает экземпляры агента.</span><span class="sxs-lookup"><span data-stu-id="71d6d-124">This attribute must contain the fully qualified name of the class that implements the agent factory that creates instances of the agent.</span></span> <span data-ttu-id="71d6d-125">Этот класс должен быть производным от класса [смтпрецеивеажентфактори](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) или [раутингажентфактори](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx) .</span><span class="sxs-lookup"><span data-stu-id="71d6d-125">This class must derive from either the [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) or [RoutingAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx) class.</span></span>  <br/> |
|<span data-ttu-id="71d6d-126">**Путь**</span><span class="sxs-lookup"><span data-stu-id="71d6d-126">**assemblyPath**</span></span> <br/> |<span data-ttu-id="71d6d-127">Полный путь, включая имя файла сборки, содержащей код для агента.</span><span class="sxs-lookup"><span data-stu-id="71d6d-127">The fully qualified path, including the file name, of the assembly that contains the code for the agent.</span></span> <span data-ttu-id="71d6d-128">Для этого атрибута требуется непустое строковое значение, содержащее по крайней мере один символ.</span><span class="sxs-lookup"><span data-stu-id="71d6d-128">This attribute requires a nonempty string value that contains at least one character.</span></span>  <br/> |
|<span data-ttu-id="71d6d-129">**enabled**</span><span class="sxs-lookup"><span data-stu-id="71d6d-129">**enabled**</span></span> <br/> |<span data-ttu-id="71d6d-130">Логическое значение, которое указывает, включен ли агент.</span><span class="sxs-lookup"><span data-stu-id="71d6d-130">A Boolean value that indicates whether the agent is enabled.</span></span> <span data-ttu-id="71d6d-131">Значение **true** , если агент включен; в противном случае — значение **false**.</span><span class="sxs-lookup"><span data-stu-id="71d6d-131">The value is **true** if the agent is enabled; otherwise, the value is **false**.</span></span> <span data-ttu-id="71d6d-132">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="71d6d-132">This attribute is required.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="71d6d-133">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="71d6d-133">Child elements</span></span>

<span data-ttu-id="71d6d-134">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="71d6d-134">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="71d6d-135">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="71d6d-135">Parent elements</span></span>

|<span data-ttu-id="71d6d-136">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="71d6d-136">**Element**</span></span>|<span data-ttu-id="71d6d-137">**Описание**</span><span class="sxs-lookup"><span data-stu-id="71d6d-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="71d6d-138">ажентлист</span><span class="sxs-lookup"><span data-stu-id="71d6d-138">agentList</span></span>](agentlist.md) <br/> |<span data-ttu-id="71d6d-139">Содержит элемент **Agent** для каждого установленного агента.</span><span class="sxs-lookup"><span data-stu-id="71d6d-139">Contains an **agent** element for each installed agent.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="71d6d-140">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="71d6d-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="71d6d-141">Namespace</span><span class="sxs-lookup"><span data-stu-id="71d6d-141">Namespace</span></span>  <br/> |<span data-ttu-id="71d6d-142">В этом файле не определено пространство имен.</span><span class="sxs-lookup"><span data-stu-id="71d6d-142">This file does not define a namespace.</span></span>  <br/> |
|<span data-ttu-id="71d6d-143">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="71d6d-143">Schema Name</span></span>  <br/> |<span data-ttu-id="71d6d-144">Недоступно.</span><span class="sxs-lookup"><span data-stu-id="71d6d-144">Not available.</span></span>  <br/> |
|<span data-ttu-id="71d6d-145">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="71d6d-145">Validation File</span></span>  <br/> |<span data-ttu-id="71d6d-146">Недоступно.</span><span class="sxs-lookup"><span data-stu-id="71d6d-146">Not available.</span></span>  <br/> |
|<span data-ttu-id="71d6d-147">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="71d6d-147">Can be Empty</span></span>  <br/> |<span data-ttu-id="71d6d-148">Неверно.</span><span class="sxs-lookup"><span data-stu-id="71d6d-148">False.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="71d6d-149">См. также</span><span class="sxs-lookup"><span data-stu-id="71d6d-149">See also</span></span>

- [<span data-ttu-id="71d6d-150">Элементы файла конфигурации агентов для Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="71d6d-150">Agents configuration file elements for Exchange 2013</span></span>](agents-configuration-file-elements-for-exchange-2013.md)

