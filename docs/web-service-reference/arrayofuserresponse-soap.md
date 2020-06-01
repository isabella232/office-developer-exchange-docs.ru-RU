---
title: Аррайофусерреспонсе (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 3e5cf65c-8d0b-4fd9-8207-56c07f914acd
description: Элемент Аррайофусерреспонсе содержит массив элементов Усерреспонсе (SOAP).
ms.openlocfilehash: fb14b6cd714a0561e9c8e17bd1779d955ba16dfc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/01/2020
ms.locfileid: "44466012"
---
# <a name="arrayofuserresponse-soap"></a><span data-ttu-id="f25fb-103">Аррайофусерреспонсе (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f25fb-103">ArrayOfUserResponse (SOAP)</span></span>

<span data-ttu-id="f25fb-104">Элемент **аррайофусерреспонсе** содержит массив элементов [усерреспонсе (SOAP)](userresponse-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="f25fb-104">The **ArrayOfUserResponse** element contains an array of [UserResponse (SOAP)](userresponse-soap.md) elements.</span></span> 
  
```XML
<ArrayOfUserResponse>
   <UserResponse/>
</ArrayOfUserResponse>
```

 <span data-ttu-id="f25fb-105">**аррайофусерреспонсе**</span><span class="sxs-lookup"><span data-stu-id="f25fb-105">**ArrayOfUserResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f25fb-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f25fb-106">Attributes and elements</span></span>

<span data-ttu-id="f25fb-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="f25fb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f25fb-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f25fb-108">Attributes</span></span>

<span data-ttu-id="f25fb-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f25fb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f25fb-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f25fb-110">Child elements</span></span>

|<span data-ttu-id="f25fb-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f25fb-111">**Element**</span></span>|<span data-ttu-id="f25fb-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f25fb-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f25fb-113">Усерреспонсе (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f25fb-113">UserResponse (SOAP)</span></span>](userresponse-soap.md) <br/> |<span data-ttu-id="f25fb-114">Содержит запрошенные параметры для указанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="f25fb-114">Contains the requested settings for the specified user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f25fb-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f25fb-115">Parent elements</span></span>

<span data-ttu-id="f25fb-116">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f25fb-116">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="f25fb-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="f25fb-117">Text value</span></span>

<span data-ttu-id="f25fb-118">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f25fb-118">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f25fb-119">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f25fb-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f25fb-120">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f25fb-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="f25fb-121">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f25fb-121">Schema Name</span></span>  <br/> |<span data-ttu-id="f25fb-122">Схема автообнаружения</span><span class="sxs-lookup"><span data-stu-id="f25fb-122">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="f25fb-123">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f25fb-123">Validation File</span></span>  <br/> |<span data-ttu-id="f25fb-124">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="f25fb-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f25fb-125">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f25fb-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="f25fb-126">True</span><span class="sxs-lookup"><span data-stu-id="f25fb-126">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f25fb-127">См. также</span><span class="sxs-lookup"><span data-stu-id="f25fb-127">See also</span></span>

- [<span data-ttu-id="f25fb-128">Операция GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f25fb-128">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)

