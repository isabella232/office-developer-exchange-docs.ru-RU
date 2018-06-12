---
title: AppStatus
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f3ab8bf1-abc5-45cf-a2e1-d7602f2c24ec
description: Значение элемента AppStatus указывает состояние почтового приложения.
ms.openlocfilehash: cf213fc3d7be02c411e9c2e83a4ff153dbefe098
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761485"
---
# <a name="appstatus"></a><span data-ttu-id="3b793-103">AppStatus</span><span class="sxs-lookup"><span data-stu-id="3b793-103">AppStatus</span></span>

<span data-ttu-id="3b793-104">Значение элемента **AppStatus** указывает состояние почтового приложения.</span><span class="sxs-lookup"><span data-stu-id="3b793-104">The **AppStatus** element value indicates the status of the mail app.</span></span> 
  
```XML
<AppStatus/>
```

 <span data-ttu-id="3b793-105">**string**</span><span class="sxs-lookup"><span data-stu-id="3b793-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3b793-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="3b793-106">Attributes and elements</span></span>

<span data-ttu-id="3b793-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="3b793-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3b793-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="3b793-108">Attributes</span></span>

<span data-ttu-id="3b793-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="3b793-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3b793-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="3b793-110">Child elements</span></span>

<span data-ttu-id="3b793-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="3b793-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3b793-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="3b793-112">Parent elements</span></span>

[<span data-ttu-id="3b793-113">Метаданные</span><span class="sxs-lookup"><span data-stu-id="3b793-113">Metadata</span></span>](metadata-ex15websvcsotherref.md)
  
## <a name="text-value"></a><span data-ttu-id="3b793-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="3b793-114">Text value</span></span>

<span data-ttu-id="3b793-115">Текстовое значение элемента **AppStatus** указывает состояние почтового приложения.</span><span class="sxs-lookup"><span data-stu-id="3b793-115">The text value of the **AppStatus** element indicates the status of the mail app.</span></span> <span data-ttu-id="3b793-116">Если пользователь можно устранить проблему, приводящую к состояние почтового приложения, [ActionUrl](actionurl.md) элемент содержит URL-адрес для выполнения исправление.</span><span class="sxs-lookup"><span data-stu-id="3b793-116">If the user can fix an issue related to the status of the mail app, the [ActionUrl](actionurl.md) element provides the URL to perform the fix.</span></span> 
  
<span data-ttu-id="3b793-117">**В таблице 1. AppStatus значения**</span><span class="sxs-lookup"><span data-stu-id="3b793-117">**Table 1. AppStatus values**</span></span>

|<span data-ttu-id="3b793-118">**Значение**</span><span class="sxs-lookup"><span data-stu-id="3b793-118">**Value**</span></span>|<span data-ttu-id="3b793-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3b793-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="3b793-120">NULL или 0</span><span class="sxs-lookup"><span data-stu-id="3b793-120">Null or 0</span></span>  <br/> |<span data-ttu-id="3b793-121">Почтовое приложение находится в работоспособном состоянии.</span><span class="sxs-lookup"><span data-stu-id="3b793-121">The mail app has a healthy status.</span></span>  <br/> |
|<span data-ttu-id="3b793-122">1.0</span><span class="sxs-lookup"><span data-stu-id="3b793-122">1.0</span></span>  <br/> |<span data-ttu-id="3b793-123">Почтовое приложение может не обновляются автоматически.</span><span class="sxs-lookup"><span data-stu-id="3b793-123">The mail app could not be automatically updated.</span></span> <span data-ttu-id="3b793-124">Почтовое приложение должно быть вновь установлен из магазина Office.</span><span class="sxs-lookup"><span data-stu-id="3b793-124">The mail app needs to be re-installed from the Office Store.</span></span>  <br/> |
|<span data-ttu-id="3b793-125">1.1</span><span class="sxs-lookup"><span data-stu-id="3b793-125">1.1</span></span>  <br/> |<span data-ttu-id="3b793-126">Почтовое приложение может не обновляются автоматически.</span><span class="sxs-lookup"><span data-stu-id="3b793-126">The mail app could not be automatically updated.</span></span> <span data-ttu-id="3b793-127">Почтовое приложение требует повышения разрешений и для этого необходимо знакомство и подтверждения для установки.</span><span class="sxs-lookup"><span data-stu-id="3b793-127">The mail app requires increased permissions, and this requires your review and confirmation to install.</span></span>  <br/> |
|<span data-ttu-id="3b793-128">1.2</span><span class="sxs-lookup"><span data-stu-id="3b793-128">1.2</span></span>  <br/> |<span data-ttu-id="3b793-129">Почтовое приложение не удалось обновить автоматически.</span><span class="sxs-lookup"><span data-stu-id="3b793-129">The mail app couldn't be updated automatically.</span></span> <span data-ttu-id="3b793-130">Текущей лицензии истек или является недопустимым.</span><span class="sxs-lookup"><span data-stu-id="3b793-130">The current license has expired or is invalid.</span></span> <span data-ttu-id="3b793-131">Обновите почтового приложения из магазина Office.</span><span class="sxs-lookup"><span data-stu-id="3b793-131">Please update the mail app from the Office Store.</span></span>  <br/> |
|<span data-ttu-id="3b793-132">2.0</span><span class="sxs-lookup"><span data-stu-id="3b793-132">2.0</span></span>  <br/> |<span data-ttu-id="3b793-133">Лицензия для почтового приложения не может быть обновлен автоматически.</span><span class="sxs-lookup"><span data-stu-id="3b793-133">The mail app license could not be automatically updated.</span></span> <span data-ttu-id="3b793-134">Лицензии для почтового приложения, необходимо восстановить из магазина Office.</span><span class="sxs-lookup"><span data-stu-id="3b793-134">The license for the mail app needs to be recovered from the Office Store.</span></span>  <br/> |
|<span data-ttu-id="3b793-135">2.1</span><span class="sxs-lookup"><span data-stu-id="3b793-135">2.1</span></span>  <br/> |<span data-ttu-id="3b793-136">Лицензия для почтового приложения не может быть обновлен автоматически.</span><span class="sxs-lookup"><span data-stu-id="3b793-136">The mail app license could not be automatically updated.</span></span> <span data-ttu-id="3b793-137">Истек срок действия текущей лицензии.</span><span class="sxs-lookup"><span data-stu-id="3b793-137">The current license has expired.</span></span> <span data-ttu-id="3b793-138">Новую лицензию для этого приложения должен быть установлен из магазина Office.</span><span class="sxs-lookup"><span data-stu-id="3b793-138">A new license for this app needs to be installed from the Office Store.</span></span>  <br/> |
|<span data-ttu-id="3b793-139">3.0</span><span class="sxs-lookup"><span data-stu-id="3b793-139">3.0</span></span>  <br/> |<span data-ttu-id="3b793-140">Состояние магазина Office для почтового приложения, была изменена.</span><span class="sxs-lookup"><span data-stu-id="3b793-140">The Office Store status for the mail app has changed.</span></span> <span data-ttu-id="3b793-141">Это предупреждение может указывать, что существует проблема с почтового приложения.</span><span class="sxs-lookup"><span data-stu-id="3b793-141">This may indicate that there is a problem with the mail app.</span></span> <span data-ttu-id="3b793-142">Перейдите на страницу почтового приложения в магазине Office для получения дополнительных сведений.</span><span class="sxs-lookup"><span data-stu-id="3b793-142">Go to the mail app page in the Office Store for more information.</span></span>  <br/> |
|<span data-ttu-id="3b793-143">3.1</span><span class="sxs-lookup"><span data-stu-id="3b793-143">3.1</span></span>  <br/> |<span data-ttu-id="3b793-144">Почтовое приложение был удален из магазина Office.</span><span class="sxs-lookup"><span data-stu-id="3b793-144">The mail app has been removed from the Office Store.</span></span>  <br/> |
|<span data-ttu-id="3b793-145">3.2</span><span class="sxs-lookup"><span data-stu-id="3b793-145">3.2</span></span>  <br/> |<span data-ttu-id="3b793-146">Был обнаружен проблема с почтового приложения и временно были сняты из магазина Office.</span><span class="sxs-lookup"><span data-stu-id="3b793-146">A problem has been discovered with the mail app and it has temporarily been withdrawn from the Office Store.</span></span>  <br/> |
|<span data-ttu-id="3b793-147">3.3</span><span class="sxs-lookup"><span data-stu-id="3b793-147">3.3</span></span>  <br/> |<span data-ttu-id="3b793-148">Почтовое приложение будет удален из магазина Office в течение 30 дней.</span><span class="sxs-lookup"><span data-stu-id="3b793-148">The mail app will be removed from the Office Store within 30 days.</span></span>  <br/> |
|<span data-ttu-id="3b793-149">4.0</span><span class="sxs-lookup"><span data-stu-id="3b793-149">4.0</span></span>  <br/> |<span data-ttu-id="3b793-150">Почтовое приложение автоматически запретил почтового клиента.</span><span class="sxs-lookup"><span data-stu-id="3b793-150">The mail app has been automatically disabled by your mail client.</span></span>  <br/> |
|<span data-ttu-id="3b793-151">4.1</span><span class="sxs-lookup"><span data-stu-id="3b793-151">4.1</span></span>  <br/> |<span data-ttu-id="3b793-152">Почтовое приложение запретил Outlook для повышения производительности.</span><span class="sxs-lookup"><span data-stu-id="3b793-152">The mail app has been disabled by Outlook for performance reasons.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="3b793-153">Замечания</span><span class="sxs-lookup"><span data-stu-id="3b793-153">Remarks</span></span>

<span data-ttu-id="3b793-154">Этот элемент появился в Exchange Server 2013 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="3b793-154">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="3b793-155">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="3b793-155">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3b793-156">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="3b793-156">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3b793-157">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="3b793-157">Namespace</span></span>  <br/> | http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3b793-158">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="3b793-158">Schema Name</span></span>  <br/> |<span data-ttu-id="3b793-159">Схема Types</span><span class="sxs-lookup"><span data-stu-id="3b793-159">Types schema</span></span>  <br/> |
|<span data-ttu-id="3b793-160">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="3b793-160">Validation File</span></span>  <br/> |<span data-ttu-id="3b793-161">Не применимо</span><span class="sxs-lookup"><span data-stu-id="3b793-161">Not applicable</span></span>  <br/> |
|<span data-ttu-id="3b793-162">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="3b793-162">Can be Empty</span></span>  <br/> |<span data-ttu-id="3b793-163">False</span><span class="sxs-lookup"><span data-stu-id="3b793-163">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3b793-164">См. также</span><span class="sxs-lookup"><span data-stu-id="3b793-164">See also</span></span>

- [<span data-ttu-id="3b793-165">Метаданные</span><span class="sxs-lookup"><span data-stu-id="3b793-165">Metadata</span></span>](metadata-ex15websvcsotherref.md)
- [<span data-ttu-id="3b793-166">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="3b793-166">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

