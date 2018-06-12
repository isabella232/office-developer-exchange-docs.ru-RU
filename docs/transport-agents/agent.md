---
title: агент
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
description: 'Последнее изменение: 17 сентября 2015'
ms.openlocfilehash: 3895095ed4e469cdb9fec489ba6b6e228779a9c8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761286"
---
# <a name="agent"></a><span data-ttu-id="7d402-103">агент</span><span class="sxs-lookup"><span data-stu-id="7d402-103">agent</span></span>
  
<span data-ttu-id="7d402-104">**Применимо к:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="7d402-104">**Applies to:** Exchange Server 2013</span></span>
  
<span data-ttu-id="7d402-105">Элемент **агента** содержит сведения о конфигурации об установленных агентов.</span><span class="sxs-lookup"><span data-stu-id="7d402-105">The **agent** element contains configuration information about an installed agent.</span></span> 
  
- [<span data-ttu-id="7d402-106">Конфигурация</span><span class="sxs-lookup"><span data-stu-id="7d402-106">configuration</span></span>](configuration.md) 
- [<span data-ttu-id="7d402-107">mexRuntime</span><span class="sxs-lookup"><span data-stu-id="7d402-107">mexRuntime</span></span>](mexruntime.md)
- [<span data-ttu-id="7d402-108">agentList</span><span class="sxs-lookup"><span data-stu-id="7d402-108">agentList</span></span>](agentlist.md)
- [<span data-ttu-id="7d402-109">агент</span><span class="sxs-lookup"><span data-stu-id="7d402-109">agent</span></span>](agent.md)
  
```XML
<agent
        name=""
        baseType=""
        classFactory=""
        assemblyPath=""
        enabled="" />
</agent>
```

<span data-ttu-id="7d402-110">**agentType (complexType)**</span><span class="sxs-lookup"><span data-stu-id="7d402-110">**agentType (complexType)**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="7d402-111">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="7d402-111">Attributes and elements</span></span>

<span data-ttu-id="7d402-112">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="7d402-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7d402-113">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="7d402-113">Attributes</span></span>

|<span data-ttu-id="7d402-114">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="7d402-114">**Attribute**</span></span>|<span data-ttu-id="7d402-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7d402-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7d402-116">**name**</span><span class="sxs-lookup"><span data-stu-id="7d402-116">**name**</span></span> <br/> |<span data-ttu-id="7d402-117">Имя, которое было указано при установке агента.</span><span class="sxs-lookup"><span data-stu-id="7d402-117">The name that was specified when the agent was installed.</span></span> <span data-ttu-id="7d402-118">Этот атрибут иметь значение пустая строка, которая содержит не более 64 символов.</span><span class="sxs-lookup"><span data-stu-id="7d402-118">This attribute requires a nonempty string value that contains a maximum of 64 characters.</span></span>  <br/> |
|<span data-ttu-id="7d402-119">**baseType**</span><span class="sxs-lookup"><span data-stu-id="7d402-119">**baseType**</span></span> <br/> |<span data-ttu-id="7d402-120">Полное имя, включая пространства имен, класса, от которого наследует агент.</span><span class="sxs-lookup"><span data-stu-id="7d402-120">The full name, including the namespace, of the class from which the agent derives.</span></span> <span data-ttu-id="7d402-121">Этот атрибут иметь значение пустая строка, которая содержит по крайней мере один знак.</span><span class="sxs-lookup"><span data-stu-id="7d402-121">This attribute requires a nonempty string value that contains at least one character.</span></span>  <br/> |
|<span data-ttu-id="7d402-122">**classFactory**</span><span class="sxs-lookup"><span data-stu-id="7d402-122">**classFactory**</span></span> <br/> |<span data-ttu-id="7d402-123">Полное имя, включая пространство имен, класс, реализующий фабрика агентов, который создает экземпляры агента.</span><span class="sxs-lookup"><span data-stu-id="7d402-123">The full name, including the namespace, of the class that implements the agent factory that creates instances of the agent.</span></span> <span data-ttu-id="7d402-124">Этот атрибут должен содержать полное имя класса, реализующего фабрика агентов, который создает экземпляры агента.</span><span class="sxs-lookup"><span data-stu-id="7d402-124">This attribute must contain the fully qualified name of the class that implements the agent factory that creates instances of the agent.</span></span> <span data-ttu-id="7d402-125">Этот класс должен наследовать от класса либо [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) , либо [RoutingAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx) .</span><span class="sxs-lookup"><span data-stu-id="7d402-125">This class must derive from either the [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) or [RoutingAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx) class.</span></span>  <br/> |
|<span data-ttu-id="7d402-126">**путь _ сборки**</span><span class="sxs-lookup"><span data-stu-id="7d402-126">**assemblyPath**</span></span> <br/> |<span data-ttu-id="7d402-127">Полный путь, включая имя файла сборки, которая содержит код для агента.</span><span class="sxs-lookup"><span data-stu-id="7d402-127">The fully qualified path, including the file name, of the assembly that contains the code for the agent.</span></span> <span data-ttu-id="7d402-128">Этот атрибут иметь значение пустая строка, которая содержит по крайней мере один знак.</span><span class="sxs-lookup"><span data-stu-id="7d402-128">This attribute requires a nonempty string value that contains at least one character.</span></span>  <br/> |
|<span data-ttu-id="7d402-129">**включено**</span><span class="sxs-lookup"><span data-stu-id="7d402-129">**enabled**</span></span> <br/> |<span data-ttu-id="7d402-130">Логическое значение, указывающее, включено ли агент.</span><span class="sxs-lookup"><span data-stu-id="7d402-130">A Boolean value that indicates whether the agent is enabled.</span></span> <span data-ttu-id="7d402-131">Значение равно **true** , если включена агент. в противном случае — значение **false**.</span><span class="sxs-lookup"><span data-stu-id="7d402-131">The value is **true** if the agent is enabled; otherwise, the value is **false**.</span></span> <span data-ttu-id="7d402-132">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="7d402-132">This attribute is required.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="7d402-133">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="7d402-133">Child elements</span></span>

<span data-ttu-id="7d402-134">Нет.</span><span class="sxs-lookup"><span data-stu-id="7d402-134">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7d402-135">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="7d402-135">Parent elements</span></span>

|<span data-ttu-id="7d402-136">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7d402-136">**Element**</span></span>|<span data-ttu-id="7d402-137">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7d402-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7d402-138">agentList</span><span class="sxs-lookup"><span data-stu-id="7d402-138">agentList</span></span>](agentlist.md) <br/> |<span data-ttu-id="7d402-139">Содержит элемент **агентов** для каждого установленного агента.</span><span class="sxs-lookup"><span data-stu-id="7d402-139">Contains an **agent** element for each installed agent.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="7d402-140">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="7d402-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7d402-141">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="7d402-141">Namespace</span></span>  <br/> |<span data-ttu-id="7d402-142">Этот файл не определяет пространство имен.</span><span class="sxs-lookup"><span data-stu-id="7d402-142">This file does not define a namespace.</span></span>  <br/> |
|<span data-ttu-id="7d402-143">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="7d402-143">Schema Name</span></span>  <br/> |<span data-ttu-id="7d402-144">Компонент недоступен.</span><span class="sxs-lookup"><span data-stu-id="7d402-144">Not available.</span></span>  <br/> |
|<span data-ttu-id="7d402-145">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="7d402-145">Validation File</span></span>  <br/> |<span data-ttu-id="7d402-146">Компонент недоступен.</span><span class="sxs-lookup"><span data-stu-id="7d402-146">Not available.</span></span>  <br/> |
|<span data-ttu-id="7d402-147">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="7d402-147">Can be Empty</span></span>  <br/> |<span data-ttu-id="7d402-148">false</span><span class="sxs-lookup"><span data-stu-id="7d402-148">False.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7d402-149">См. также</span><span class="sxs-lookup"><span data-stu-id="7d402-149">See also</span></span>

- [<span data-ttu-id="7d402-150">Элементы файла конфигурации агентов для Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="7d402-150">Agents configuration file elements for Exchange 2013</span></span>](agents-configuration-file-elements-for-exchange-2013.md)

