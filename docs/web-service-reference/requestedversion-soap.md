---
title: Рекуестедверсион (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 962036c9-9b13-4669-bed2-2502c0f5aabe
description: Элемент Рекуестедверсион Указывает минимальную версию службы, на которую клиент хочет обработать запрос.
ms.openlocfilehash: ded276b3eb2c70b6edd39ca12289098de2b3faea
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459169"
---
# <a name="requestedversion-soap"></a><span data-ttu-id="f3adf-103">Рекуестедверсион (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f3adf-103">RequestedVersion (SOAP)</span></span>

<span data-ttu-id="f3adf-104">Элемент **рекуестедверсион** Указывает минимальную версию службы, на которую клиент хочет обработать запрос.</span><span class="sxs-lookup"><span data-stu-id="f3adf-104">The **RequestedVersion** element specifies the minimum service version that the client wants the request to be processed on.</span></span> 
  
```XML
<RequestedVersion/>
```

 <span data-ttu-id="f3adf-105">**ексчанжеверсион**</span><span class="sxs-lookup"><span data-stu-id="f3adf-105">**ExchangeVersion**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f3adf-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f3adf-106">Attributes and elements</span></span>

<span data-ttu-id="f3adf-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="f3adf-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f3adf-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f3adf-108">Attributes</span></span>

<span data-ttu-id="f3adf-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f3adf-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f3adf-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f3adf-110">Child elements</span></span>

<span data-ttu-id="f3adf-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f3adf-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f3adf-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f3adf-112">Parent elements</span></span>

|<span data-ttu-id="f3adf-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f3adf-113">**Element**</span></span>|<span data-ttu-id="f3adf-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f3adf-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f3adf-115">Запрос (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f3adf-115">Request (SOAP)</span></span>](request-soap.md) <br/> |<span data-ttu-id="f3adf-116">Содержит запрошенные параметры конфигурации и конечных пользователей.</span><span class="sxs-lookup"><span data-stu-id="f3adf-116">Contains the requested configuration settings and the target users.</span></span>  <br/> |
|[<span data-ttu-id="f3adf-117">Request (Жетдомаинсеттингс) (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f3adf-117">Request (GetDomainSettings) (SOAP)</span></span>](request-getdomainsettingssoap.md) <br/> |<span data-ttu-id="f3adf-118">Представляет запрос на получение параметров домена.</span><span class="sxs-lookup"><span data-stu-id="f3adf-118">Represents a request to get domain settings.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f3adf-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="f3adf-119">Text value</span></span>

<span data-ttu-id="f3adf-120">Текстовое значение для элемента **рекуестедверсион** может быть Exchange2010, Exchange2010_SP1, Exchange2010_SP2 или Exchange2013.</span><span class="sxs-lookup"><span data-stu-id="f3adf-120">The text value for the **RequestedVersion** element can be Exchange2010, Exchange2010_SP1, Exchange2010_SP2, or Exchange2013.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f3adf-121">Примечания</span><span class="sxs-lookup"><span data-stu-id="f3adf-121">Remarks</span></span>

<span data-ttu-id="f3adf-122">Если этот элемент не указан, используется последняя версия службы.</span><span class="sxs-lookup"><span data-stu-id="f3adf-122">If this element is not present, the latest service version is used.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f3adf-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f3adf-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f3adf-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f3adf-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="f3adf-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f3adf-125">Schema Name</span></span>  <br/> |<span data-ttu-id="f3adf-126">Схема автообнаружения</span><span class="sxs-lookup"><span data-stu-id="f3adf-126">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="f3adf-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f3adf-127">Validation File</span></span>  <br/> |<span data-ttu-id="f3adf-128">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="f3adf-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f3adf-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f3adf-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="f3adf-130">False</span><span class="sxs-lookup"><span data-stu-id="f3adf-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f3adf-131">См. также</span><span class="sxs-lookup"><span data-stu-id="f3adf-131">See also</span></span>



[<span data-ttu-id="f3adf-132">Операция GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f3adf-132">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
  
[<span data-ttu-id="f3adf-133">Операция Жетдомаинсеттингс (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f3adf-133">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

