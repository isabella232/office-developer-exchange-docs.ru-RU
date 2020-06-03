---
title: инсталлаппреспонсе
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c5e0582d-c1e1-453b-93ed-c31165c82697
description: Элемент Инсталлаппреспонсе указывает ответ на запрос InstallApp.
ms.openlocfilehash: 0f7690e2df7e71c4e478dec191671af24f96294b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465669"
---
# <a name="installappresponse"></a><span data-ttu-id="fa093-103">инсталлаппреспонсе</span><span class="sxs-lookup"><span data-stu-id="fa093-103">InstallAppResponse</span></span>

<span data-ttu-id="fa093-104">Элемент **инсталлаппреспонсе** указывает ответ на запрос **InstallAPP** .</span><span class="sxs-lookup"><span data-stu-id="fa093-104">The **InstallAppResponse** element specifies the response to an **InstallApp** request.</span></span> 
  
```xml
<InstallAppResponse ResponseClass="">
    <MessageText></MessageText>
    <ResponseCode></ResponseCode>
    <DescriptiveLinkKey></DescriptiveLinkKey>
    <MessageXml></MessageXml>
</InstallAppResponse>
```

 <span data-ttu-id="fa093-105">**инсталлаппреспонсетипе**</span><span class="sxs-lookup"><span data-stu-id="fa093-105">**InstallAppResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fa093-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="fa093-106">Attributes and elements</span></span>

<span data-ttu-id="fa093-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="fa093-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fa093-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="fa093-108">Attributes</span></span>

|<span data-ttu-id="fa093-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="fa093-109">**Attribute**</span></span>|<span data-ttu-id="fa093-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="fa093-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="fa093-111">респонсекласс</span><span class="sxs-lookup"><span data-stu-id="fa093-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="fa093-112">Указывает класс ответа.</span><span class="sxs-lookup"><span data-stu-id="fa093-112">Indicates the class of the response.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="fa093-113">респонсекласс</span><span class="sxs-lookup"><span data-stu-id="fa093-113">ResponseClass</span></span>

|<span data-ttu-id="fa093-114">**Значение**</span><span class="sxs-lookup"><span data-stu-id="fa093-114">**Value**</span></span>|<span data-ttu-id="fa093-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="fa093-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="fa093-116">Успешно</span><span class="sxs-lookup"><span data-stu-id="fa093-116">Success</span></span>  <br/> |<span data-ttu-id="fa093-117">Указывает на успешное выполнение.</span><span class="sxs-lookup"><span data-stu-id="fa093-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="fa093-118">Предупреждение</span><span class="sxs-lookup"><span data-stu-id="fa093-118">Warning</span></span>  <br/> |<span data-ttu-id="fa093-119">Указывает на предупреждение.</span><span class="sxs-lookup"><span data-stu-id="fa093-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="fa093-120">Ошибка</span><span class="sxs-lookup"><span data-stu-id="fa093-120">Error</span></span>  <br/> |<span data-ttu-id="fa093-121">Указывает на ошибку.</span><span class="sxs-lookup"><span data-stu-id="fa093-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="fa093-122">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="fa093-122">Child elements</span></span>

|<span data-ttu-id="fa093-123">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="fa093-123">**Element**</span></span>|<span data-ttu-id="fa093-124">**Описание**</span><span class="sxs-lookup"><span data-stu-id="fa093-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fa093-125">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="fa093-125">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="fa093-126">В настоящее время не используется и зарезервировано для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="fa093-126">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="fa093-127">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="fa093-127">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="fa093-128">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="fa093-128">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="fa093-129">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="fa093-129">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="fa093-130">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="fa093-130">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="fa093-131">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="fa093-131">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="fa093-132">Предоставляет сведения о состоянии запроса.</span><span class="sxs-lookup"><span data-stu-id="fa093-132">Provides status information about the request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="fa093-133">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="fa093-133">Parent elements</span></span>

|<span data-ttu-id="fa093-134">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="fa093-134">**Element**</span></span>|<span data-ttu-id="fa093-135">**Описание**</span><span class="sxs-lookup"><span data-stu-id="fa093-135">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fa093-136">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="fa093-136">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="fa093-137">Содержит ответные сообщения для запроса веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="fa093-137">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="fa093-138">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="fa093-138">Text value</span></span>

<span data-ttu-id="fa093-139">Нет.</span><span class="sxs-lookup"><span data-stu-id="fa093-139">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="fa093-140">Примечания</span><span class="sxs-lookup"><span data-stu-id="fa093-140">Remarks</span></span>

<span data-ttu-id="fa093-141">Элемент **жетаппманифестсреспонсемессаже** применяется для клиентов, которые ориентированы на Exchange Online и версии Microsoft Exchange Server, начиная с Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="fa093-141">The **GetAppManifestsResponseMessage** element is applicable for clients that target Exchange Online and versions of Microsoft Exchange Server starting with Exchange 2013.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="fa093-142">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="fa093-142">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fa093-143">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="fa093-143">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="fa093-144">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="fa093-144">Schema Name</span></span>  <br/> |<span data-ttu-id="fa093-145">Схема сообщения</span><span class="sxs-lookup"><span data-stu-id="fa093-145">Message schema</span></span>  <br/> |
|<span data-ttu-id="fa093-146">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="fa093-146">Validation File</span></span>  <br/> |<span data-ttu-id="fa093-147">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="fa093-147">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="fa093-148">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="fa093-148">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="fa093-149">См. также</span><span class="sxs-lookup"><span data-stu-id="fa093-149">See also</span></span>



- [<span data-ttu-id="fa093-150">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="fa093-150">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

