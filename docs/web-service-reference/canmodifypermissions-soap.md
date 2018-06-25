---
title: CanModifyPermissions (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 9693de1a-0c76-4898-8f4d-a8693fb005b3
description: Элемент CanModifyPermissions указывает, может ли пользователь изменить разрешения на доступ к документу, расположение для обмена.
ms.openlocfilehash: 16526cb79eeca591af6e009e67959a1c3b58a5d7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761666"
---
# <a name="canmodifypermissions-soap"></a><span data-ttu-id="20d4a-103">CanModifyPermissions (SOAP)</span><span class="sxs-lookup"><span data-stu-id="20d4a-103">CanModifyPermissions (SOAP)</span></span>

<span data-ttu-id="20d4a-104">Элемент **CanModifyPermissions** указывает, может ли пользователь изменить разрешения на доступ к документу, расположение для обмена.</span><span class="sxs-lookup"><span data-stu-id="20d4a-104">The **CanModifyPermissions** element indicates whether a user can modify access permissions to a document sharing location.</span></span> 
  
```XML
<CanModifyPermissions /> 
```

 <span data-ttu-id="20d4a-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="20d4a-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="20d4a-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="20d4a-106">Attributes and elements</span></span>

<span data-ttu-id="20d4a-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="20d4a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="20d4a-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="20d4a-108">Attributes</span></span>

<span data-ttu-id="20d4a-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="20d4a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="20d4a-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="20d4a-110">Child elements</span></span>

<span data-ttu-id="20d4a-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="20d4a-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="20d4a-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="20d4a-112">Parent elements</span></span>

|<span data-ttu-id="20d4a-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="20d4a-113">**Element**</span></span>|<span data-ttu-id="20d4a-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="20d4a-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="20d4a-115">DocumentSharingLocation (SOAP)</span><span class="sxs-lookup"><span data-stu-id="20d4a-115">DocumentSharingLocation (SOAP)</span></span>](documentsharinglocation-soap.md) <br/> |<span data-ttu-id="20d4a-116">Представляет сведения о расположении и метаданных для документа расположение для обмена.</span><span class="sxs-lookup"><span data-stu-id="20d4a-116">Represents location and metadata information for a document sharing location.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="20d4a-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="20d4a-117">Text value</span></span>

<span data-ttu-id="20d4a-118">Логическое значение элемента **CanModifyPermissions** указывает, будет ли пользователи смогут изменять разрешения на доступ к месту общего доступа.</span><span class="sxs-lookup"><span data-stu-id="20d4a-118">The Boolean value of the **CanModifyPermissions** element indicates whether users can modify access permissions to the sharing location.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="20d4a-119">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="20d4a-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="20d4a-120">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="20d4a-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="20d4a-121">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="20d4a-121">Schema Name</span></span>  <br/> |<span data-ttu-id="20d4a-122">Схема службы автообнаружения</span><span class="sxs-lookup"><span data-stu-id="20d4a-122">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="20d4a-123">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="20d4a-123">Validation File</span></span>  <br/> |<span data-ttu-id="20d4a-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="20d4a-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="20d4a-125">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="20d4a-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="20d4a-126">True</span><span class="sxs-lookup"><span data-stu-id="20d4a-126">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="20d4a-127">См. также</span><span class="sxs-lookup"><span data-stu-id="20d4a-127">See also</span></span>



[<span data-ttu-id="20d4a-128">Операция GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="20d4a-128">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)


[<span data-ttu-id="20d4a-129">Ссылки веб-службу автообнаружения для Exchange</span><span class="sxs-lookup"><span data-stu-id="20d4a-129">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
  
[<span data-ttu-id="20d4a-130">Элементы XML автоматического обнаружения SOAP для Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="20d4a-130">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)

