---
title: Серверверсионинфо (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 8662647b-e50a-4774-9ba3-a951ae6df781
description: Элемент Серверверсионинфо содержит версию сервера, который обработал запрос.
ms.openlocfilehash: b02071e4997aba91fb538d52df2612fe6fd32800
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835385"
---
# <a name="serverversioninfo-soap"></a><span data-ttu-id="54ce0-103">Серверверсионинфо (SOAP)</span><span class="sxs-lookup"><span data-stu-id="54ce0-103">ServerVersionInfo (SOAP)</span></span>

<span data-ttu-id="54ce0-104">Элемент **серверверсионинфо** содержит версию сервера, который обработал запрос.</span><span class="sxs-lookup"><span data-stu-id="54ce0-104">The **ServerVersionInfo** element contains the version of the server that processed the request.</span></span> 
  
```XML
<ServerVersionInfo>
   <MajorVersion/>
   <MinorVersion/>
   <MajorBuildNumber/>
   <MinorBuildNumber/>
   <Version/>
</ServerVersionInfo>
```

 <span data-ttu-id="54ce0-105">**серверверсионинфо**</span><span class="sxs-lookup"><span data-stu-id="54ce0-105">**ServerVersionInfo**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="54ce0-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="54ce0-106">Attributes and elements</span></span>

<span data-ttu-id="54ce0-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="54ce0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="54ce0-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="54ce0-108">Attributes</span></span>

<span data-ttu-id="54ce0-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="54ce0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="54ce0-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="54ce0-110">Child elements</span></span>

|<span data-ttu-id="54ce0-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="54ce0-111">**Element**</span></span>|<span data-ttu-id="54ce0-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="54ce0-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="54ce0-113">MajorVersion (SOAP)</span><span class="sxs-lookup"><span data-stu-id="54ce0-113">MajorVersion (SOAP)</span></span>](majorversion-soap.md) <br/> |<span data-ttu-id="54ce0-114">Основной номер версии сервера.</span><span class="sxs-lookup"><span data-stu-id="54ce0-114">The major version number for the server.</span></span>  <br/> |
|[<span data-ttu-id="54ce0-115">MinorVersion (SOAP)</span><span class="sxs-lookup"><span data-stu-id="54ce0-115">MinorVersion (SOAP)</span></span>](minorversion-soap.md) <br/> |<span data-ttu-id="54ce0-116">Дополнительный номер версии сервера.</span><span class="sxs-lookup"><span data-stu-id="54ce0-116">The minor version number for the server.</span></span>  <br/> |
|[<span data-ttu-id="54ce0-117">Мажорбуилднумбер (SOAP)</span><span class="sxs-lookup"><span data-stu-id="54ce0-117">MajorBuildNumber (SOAP)</span></span>](majorbuildnumber-soap.md) <br/> |<span data-ttu-id="54ce0-118">Основной номер сборки для сервера.</span><span class="sxs-lookup"><span data-stu-id="54ce0-118">The major build number for the server.</span></span>  <br/> |
|[<span data-ttu-id="54ce0-119">Минорбуилднумбер (SOAP)</span><span class="sxs-lookup"><span data-stu-id="54ce0-119">MinorBuildNumber (SOAP)</span></span>](minorbuildnumber-soap.md) <br/> |<span data-ttu-id="54ce0-120">Дополнительный номер сборки для сервера.</span><span class="sxs-lookup"><span data-stu-id="54ce0-120">The minor build number for the server.</span></span>  <br/> |
|[<span data-ttu-id="54ce0-121">Версия (SOAP)</span><span class="sxs-lookup"><span data-stu-id="54ce0-121">Version (SOAP)</span></span>](version-soap.md) <br/> |<span data-ttu-id="54ce0-122">Описание версии серверного продукта.</span><span class="sxs-lookup"><span data-stu-id="54ce0-122">A description of the server product version.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="54ce0-123">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="54ce0-123">Parent elements</span></span>

<span data-ttu-id="54ce0-124">Нет.</span><span class="sxs-lookup"><span data-stu-id="54ce0-124">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="54ce0-125">Примечания</span><span class="sxs-lookup"><span data-stu-id="54ce0-125">Remarks</span></span>

<span data-ttu-id="54ce0-126">Этот элемент возвращается в заголовке SOAP.</span><span class="sxs-lookup"><span data-stu-id="54ce0-126">This element is returned in the SOAP header.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="54ce0-127">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="54ce0-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="54ce0-128">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="54ce0-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="54ce0-129">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="54ce0-129">Schema Name</span></span>  <br/> |<span data-ttu-id="54ce0-130">Схема автообнаружения</span><span class="sxs-lookup"><span data-stu-id="54ce0-130">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="54ce0-131">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="54ce0-131">Validation File</span></span>  <br/> |<span data-ttu-id="54ce0-132">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="54ce0-132">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="54ce0-133">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="54ce0-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="54ce0-134">True</span><span class="sxs-lookup"><span data-stu-id="54ce0-134">True</span></span>  <br/> |
   

