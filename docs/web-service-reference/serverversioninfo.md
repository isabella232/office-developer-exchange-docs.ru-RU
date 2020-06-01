---
title: серверверсионинфо
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ServerVersionInfo
api_type:
- schema
ms.assetid: c04a6872-ca27-432b-aac2-36b023d0afc6
description: Элемент Серверверсионинфо представляет номер версии Microsoft Exchange Server.
ms.openlocfilehash: 5bd1fbd8fdee584a9d272fa8ab82f2a31c1357fe
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466831"
---
# <a name="serverversioninfo"></a><span data-ttu-id="d86c1-103">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="d86c1-103">ServerVersionInfo</span></span>

<span data-ttu-id="d86c1-104">Элемент **серверверсионинфо** представляет номер версии Microsoft Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="d86c1-104">The **ServerVersionInfo** element represents the Microsoft Exchange Server version number.</span></span> 
  
```xml
<ServerVersionInfo MajorVersion="" MinorVersion="" MajorBuildNumber="" MinorBuildNumber="" Version="" />
```

## <a name="attributes-and-elements"></a><span data-ttu-id="d86c1-105">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d86c1-105">Attributes and elements</span></span>

<span data-ttu-id="d86c1-106">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="d86c1-106">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d86c1-107">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d86c1-107">Attributes</span></span>

|<span data-ttu-id="d86c1-108">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="d86c1-108">**Attribute**</span></span>|<span data-ttu-id="d86c1-109">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d86c1-109">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d86c1-110">MajorVersion</span><span class="sxs-lookup"><span data-stu-id="d86c1-110">MajorVersion</span></span>  <br/> |<span data-ttu-id="d86c1-111">Описывает основной номер версии.</span><span class="sxs-lookup"><span data-stu-id="d86c1-111">Describes the major version number.</span></span>  <br/> |
|<span data-ttu-id="d86c1-112">MinorVersion</span><span class="sxs-lookup"><span data-stu-id="d86c1-112">MinorVersion</span></span>  <br/> |<span data-ttu-id="d86c1-113">Описывает дополнительный номер версии.</span><span class="sxs-lookup"><span data-stu-id="d86c1-113">Describes the minor version number.</span></span>  <br/> |
|<span data-ttu-id="d86c1-114">мажорбуилднумбер</span><span class="sxs-lookup"><span data-stu-id="d86c1-114">MajorBuildNumber</span></span>  <br/> |<span data-ttu-id="d86c1-115">Описывает основной номер сборки.</span><span class="sxs-lookup"><span data-stu-id="d86c1-115">Describes the major build number.</span></span>  <br/> |
|<span data-ttu-id="d86c1-116">минорбуилднумбер</span><span class="sxs-lookup"><span data-stu-id="d86c1-116">MinorBuildNumber</span></span>  <br/> |<span data-ttu-id="d86c1-117">Описывает дополнительный номер сборки.</span><span class="sxs-lookup"><span data-stu-id="d86c1-117">Describes the minor build number.</span></span>  <br/> |
|<span data-ttu-id="d86c1-118">Версия</span><span class="sxs-lookup"><span data-stu-id="d86c1-118">Version</span></span>  <br/> |<span data-ttu-id="d86c1-119">Описывает версию схемы веб-служб Exchange (EWS).</span><span class="sxs-lookup"><span data-stu-id="d86c1-119">Describes the Exchange Web Services (EWS) schema version.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="d86c1-120">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d86c1-120">Child elements</span></span>

<span data-ttu-id="d86c1-121">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="d86c1-121">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d86c1-122">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d86c1-122">Parent elements</span></span>

<span data-ttu-id="d86c1-123">Нет.</span><span class="sxs-lookup"><span data-stu-id="d86c1-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d86c1-124">Примечания</span><span class="sxs-lookup"><span data-stu-id="d86c1-124">Remarks</span></span>

<span data-ttu-id="d86c1-125">Этот элемент возвращается в заголовке SOAP ответного сообщения веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="d86c1-125">This element is returned in the SOAP header of an Exchange Web Services response message.</span></span>
  
<span data-ttu-id="d86c1-126">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера, на котором работает сервер Microsoft Exchange с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="d86c1-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="d86c1-127">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d86c1-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d86c1-128">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d86c1-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d86c1-129">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d86c1-129">Schema Name</span></span>  <br/> |<span data-ttu-id="d86c1-130">Схема Types</span><span class="sxs-lookup"><span data-stu-id="d86c1-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="d86c1-131">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d86c1-131">Validation File</span></span>  <br/> |<span data-ttu-id="d86c1-132">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="d86c1-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d86c1-133">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d86c1-133">Can Be Empty</span></span>  <br/> |<span data-ttu-id="d86c1-134">False</span><span class="sxs-lookup"><span data-stu-id="d86c1-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d86c1-135">См. также</span><span class="sxs-lookup"><span data-stu-id="d86c1-135">See also</span></span>



- [<span data-ttu-id="d86c1-136">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="d86c1-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

