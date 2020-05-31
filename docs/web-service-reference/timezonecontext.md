---
title: тимезонеконтекст
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TimeZoneContext
api_type:
- schema
ms.assetid: 573c462b-aa1d-4ba0-8852-e3f48b26873b
description: Элемент Тимезонеконтекст используется в заголовке протокола SOAP, чтобы указать определение часового пояса, которое будет использоваться по умолчанию при назначении часового пояса для свойств объекта DateTime, которые создаются, обновляются и извлекаются с помощью веб-служб Exchange (EWS).
ms.openlocfilehash: 38b7ab4c587adac45fc3bcf351f417ea72313a97
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840191"
---
# <a name="timezonecontext"></a><span data-ttu-id="96366-103">тимезонеконтекст</span><span class="sxs-lookup"><span data-stu-id="96366-103">TimeZoneContext</span></span>

<span data-ttu-id="96366-104">Элемент **тимезонеконтекст** используется в заголовке протокола SOAP, чтобы указать определение часового пояса, которое будет использоваться по умолчанию при назначении часового пояса для свойств объекта DateTime, которые создаются, обновляются и извлекаются с помощью веб-служб Exchange (EWS).</span><span class="sxs-lookup"><span data-stu-id="96366-104">The **TimeZoneContext** element is used in the Simple Object Access Protocol (SOAP) header to specify the time zone definition that is to be used as the default when assigning the time zone for the DateTime properties of objects that are created, updated, and retrieved by using Exchange Web Services (EWS).</span></span> 
  
```xml
<TimeZoneContext>
   <TimeZoneDefinition/>
</TimeZoneContext>
```

 <span data-ttu-id="96366-105">**тимезонеконтексттипе**</span><span class="sxs-lookup"><span data-stu-id="96366-105">**TimeZoneContextType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="96366-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="96366-106">Attributes and elements</span></span>

<span data-ttu-id="96366-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="96366-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="96366-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="96366-108">Attributes</span></span>

<span data-ttu-id="96366-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="96366-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="96366-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="96366-110">Child elements</span></span>

|<span data-ttu-id="96366-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="96366-111">**Element**</span></span>|<span data-ttu-id="96366-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="96366-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="96366-113">тимезонедефинитион</span><span class="sxs-lookup"><span data-stu-id="96366-113">TimeZoneDefinition</span></span>](timezonedefinition.md) <br/> |<span data-ttu-id="96366-114">Задает периоды и переходы, определяющие часовой пояс.</span><span class="sxs-lookup"><span data-stu-id="96366-114">Specifies the periods and transitions that define a time zone.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="96366-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="96366-115">Parent elements</span></span>

<span data-ttu-id="96366-116">Нет.</span><span class="sxs-lookup"><span data-stu-id="96366-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="96366-117">Примечания</span><span class="sxs-lookup"><span data-stu-id="96366-117">Remarks</span></span>

<span data-ttu-id="96366-118">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера, на котором работает сервер Microsoft Exchange с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="96366-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="96366-119">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="96366-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="96366-120">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="96366-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="96366-121">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="96366-121">Schema Name</span></span>  <br/> |<span data-ttu-id="96366-122">Схема Types</span><span class="sxs-lookup"><span data-stu-id="96366-122">Types schema</span></span>  <br/> |
|<span data-ttu-id="96366-123">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="96366-123">Validation File</span></span>  <br/> |<span data-ttu-id="96366-124">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="96366-124">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="96366-125">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="96366-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="96366-126">False</span><span class="sxs-lookup"><span data-stu-id="96366-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="96366-127">См. также</span><span class="sxs-lookup"><span data-stu-id="96366-127">See also</span></span>



- [<span data-ttu-id="96366-128">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="96366-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

