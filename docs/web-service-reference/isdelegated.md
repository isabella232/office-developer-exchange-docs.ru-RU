---
title: Isdelegated для
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsDelegated
api_type:
- schema
ms.assetid: c12907db-be80-4924-9469-8e58612cf42c
description: Элемент с делегатом "делегируемый" указывает, было ли собрание обработано с помощью учетной записи с делегированным доступом.
ms.openlocfilehash: 2c62b59665431d5ea203e972a506aa90afc76601
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456446"
---
# <a name="isdelegated"></a><span data-ttu-id="92d43-103">Isdelegated для</span><span class="sxs-lookup"><span data-stu-id="92d43-103">IsDelegated</span></span>

<span data-ttu-id="92d43-104">Элемент с **делегатом "делегируемый** " указывает, было ли собрание обработано с помощью учетной записи с делегированным доступом.</span><span class="sxs-lookup"><span data-stu-id="92d43-104">The **IsDelegated** element indicates whether a meeting was handled by an account that has delegate access.</span></span> 
  
```xml
<IsDelegated/>
```

 <span data-ttu-id="92d43-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="92d43-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="92d43-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="92d43-106">Attributes and elements</span></span>

<span data-ttu-id="92d43-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="92d43-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="92d43-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="92d43-108">Attributes</span></span>

<span data-ttu-id="92d43-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="92d43-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="92d43-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="92d43-110">Child elements</span></span>

<span data-ttu-id="92d43-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="92d43-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="92d43-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="92d43-112">Parent elements</span></span>

|<span data-ttu-id="92d43-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="92d43-113">**Element**</span></span>|<span data-ttu-id="92d43-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="92d43-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="92d43-115">митингканцеллатион</span><span class="sxs-lookup"><span data-stu-id="92d43-115">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="92d43-116">Представляет отмену собрания в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="92d43-116">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="92d43-117">митингмессаже</span><span class="sxs-lookup"><span data-stu-id="92d43-117">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="92d43-118">Представляет собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="92d43-118">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="92d43-119">Свойство meetingrequest</span><span class="sxs-lookup"><span data-stu-id="92d43-119">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="92d43-120">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="92d43-120">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="92d43-121">митингреспонсе</span><span class="sxs-lookup"><span data-stu-id="92d43-121">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="92d43-122">Представляет ответ на приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="92d43-122">Represents a meeting response in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="92d43-123">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="92d43-123">Text value</span></span>

<span data-ttu-id="92d43-124">Текстовое значение **true** указывает на то, что собрание было обработано учетной записью, имеющей доступ представителя.</span><span class="sxs-lookup"><span data-stu-id="92d43-124">A text value of **true** indicates that the meeting was handled by an account that has delegate access.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="92d43-125">Примечания</span><span class="sxs-lookup"><span data-stu-id="92d43-125">Remarks</span></span>

<span data-ttu-id="92d43-126">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="92d43-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="92d43-127">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="92d43-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="92d43-128">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="92d43-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="92d43-129">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="92d43-129">Schema Name</span></span>  <br/> |<span data-ttu-id="92d43-130">Схема Types</span><span class="sxs-lookup"><span data-stu-id="92d43-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="92d43-131">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="92d43-131">Validation File</span></span>  <br/> |<span data-ttu-id="92d43-132">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="92d43-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="92d43-133">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="92d43-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="92d43-134">False</span><span class="sxs-lookup"><span data-stu-id="92d43-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="92d43-135">См. также</span><span class="sxs-lookup"><span data-stu-id="92d43-135">See also</span></span>



- [<span data-ttu-id="92d43-136">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="92d43-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

