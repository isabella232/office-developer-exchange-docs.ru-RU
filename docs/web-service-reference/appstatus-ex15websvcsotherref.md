---
title: аппстатус
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f3ab8bf1-abc5-45cf-a2e1-d7602f2c24ec
description: Значение элемента Аппстатус указывает состояние почтового приложения.
ms.openlocfilehash: d833947fd62d500418f257829d241a2e0b3bca9c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464779"
---
# <a name="appstatus"></a><span data-ttu-id="9e487-103">аппстатус</span><span class="sxs-lookup"><span data-stu-id="9e487-103">AppStatus</span></span>

<span data-ttu-id="9e487-104">Значение элемента **аппстатус** указывает состояние почтового приложения.</span><span class="sxs-lookup"><span data-stu-id="9e487-104">The **AppStatus** element value indicates the status of the mail app.</span></span> 
  
```XML
<AppStatus/>
```

 <span data-ttu-id="9e487-105">**строка**</span><span class="sxs-lookup"><span data-stu-id="9e487-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9e487-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="9e487-106">Attributes and elements</span></span>

<span data-ttu-id="9e487-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="9e487-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9e487-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="9e487-108">Attributes</span></span>

<span data-ttu-id="9e487-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="9e487-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9e487-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="9e487-110">Child elements</span></span>

<span data-ttu-id="9e487-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="9e487-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9e487-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="9e487-112">Parent elements</span></span>

[<span data-ttu-id="9e487-113">Метаданные</span><span class="sxs-lookup"><span data-stu-id="9e487-113">Metadata</span></span>](metadata-ex15websvcsotherref.md)
  
## <a name="text-value"></a><span data-ttu-id="9e487-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="9e487-114">Text value</span></span>

<span data-ttu-id="9e487-115">Текстовое значение элемента **аппстатус** указывает состояние почтового приложения.</span><span class="sxs-lookup"><span data-stu-id="9e487-115">The text value of the **AppStatus** element indicates the status of the mail app.</span></span> <span data-ttu-id="9e487-116">Если пользователь может устранить проблему, связанную с состоянием почтового приложения, элемент [актионурл](actionurl.md) предоставляет URL-адрес для выполнения исправления.</span><span class="sxs-lookup"><span data-stu-id="9e487-116">If the user can fix an issue related to the status of the mail app, the [ActionUrl](actionurl.md) element provides the URL to perform the fix.</span></span> 
  
<span data-ttu-id="9e487-117">**Таблица 1. Значения Аппстатус**</span><span class="sxs-lookup"><span data-stu-id="9e487-117">**Table 1. AppStatus values**</span></span>

|<span data-ttu-id="9e487-118">**Значение**</span><span class="sxs-lookup"><span data-stu-id="9e487-118">**Value**</span></span>|<span data-ttu-id="9e487-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9e487-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9e487-120">NULL или 0</span><span class="sxs-lookup"><span data-stu-id="9e487-120">Null or 0</span></span>  <br/> |<span data-ttu-id="9e487-121">Почтовое приложение имеет состояние работоспособности.</span><span class="sxs-lookup"><span data-stu-id="9e487-121">The mail app has a healthy status.</span></span>  <br/> |
|<span data-ttu-id="9e487-122">1.0</span><span class="sxs-lookup"><span data-stu-id="9e487-122">1.0</span></span>  <br/> |<span data-ttu-id="9e487-123">Почтовое приложение не удалось обновить автоматически.</span><span class="sxs-lookup"><span data-stu-id="9e487-123">The mail app could not be automatically updated.</span></span> <span data-ttu-id="9e487-124">Почтовое приложение необходимо повторно установить из магазина Office.</span><span class="sxs-lookup"><span data-stu-id="9e487-124">The mail app needs to be re-installed from the Office Store.</span></span>  <br/> |
|<span data-ttu-id="9e487-125">1.1</span><span class="sxs-lookup"><span data-stu-id="9e487-125">1.1</span></span>  <br/> |<span data-ttu-id="9e487-126">Почтовое приложение не удалось обновить автоматически.</span><span class="sxs-lookup"><span data-stu-id="9e487-126">The mail app could not be automatically updated.</span></span> <span data-ttu-id="9e487-127">Почтовому приложению требуются расширенные разрешения, и для этого требуется проверка и подтверждение установки.</span><span class="sxs-lookup"><span data-stu-id="9e487-127">The mail app requires increased permissions, and this requires your review and confirmation to install.</span></span>  <br/> |
|<span data-ttu-id="9e487-128">1.2</span><span class="sxs-lookup"><span data-stu-id="9e487-128">1.2</span></span>  <br/> |<span data-ttu-id="9e487-129">Не удалось автоматически обновить почтовое приложение.</span><span class="sxs-lookup"><span data-stu-id="9e487-129">The mail app couldn't be updated automatically.</span></span> <span data-ttu-id="9e487-130">Текущая лицензия просрочена или недействительна.</span><span class="sxs-lookup"><span data-stu-id="9e487-130">The current license has expired or is invalid.</span></span> <span data-ttu-id="9e487-131">Обновите почтовое приложение из магазина Office.</span><span class="sxs-lookup"><span data-stu-id="9e487-131">Please update the mail app from the Office Store.</span></span>  <br/> |
|<span data-ttu-id="9e487-132">2.0</span><span class="sxs-lookup"><span data-stu-id="9e487-132">2.0</span></span>  <br/> |<span data-ttu-id="9e487-133">Не удалось автоматически обновить лицензию почтового приложения.</span><span class="sxs-lookup"><span data-stu-id="9e487-133">The mail app license could not be automatically updated.</span></span> <span data-ttu-id="9e487-134">Лицензия для почтового приложения должна быть восстановлена из магазина Office.</span><span class="sxs-lookup"><span data-stu-id="9e487-134">The license for the mail app needs to be recovered from the Office Store.</span></span>  <br/> |
|<span data-ttu-id="9e487-135">2.1</span><span class="sxs-lookup"><span data-stu-id="9e487-135">2.1</span></span>  <br/> |<span data-ttu-id="9e487-136">Не удалось автоматически обновить лицензию почтового приложения.</span><span class="sxs-lookup"><span data-stu-id="9e487-136">The mail app license could not be automatically updated.</span></span> <span data-ttu-id="9e487-137">Срок действия текущей лицензии истек.</span><span class="sxs-lookup"><span data-stu-id="9e487-137">The current license has expired.</span></span> <span data-ttu-id="9e487-138">Новая лицензия для этого приложения должна быть установлена из магазина Office.</span><span class="sxs-lookup"><span data-stu-id="9e487-138">A new license for this app needs to be installed from the Office Store.</span></span>  <br/> |
|<span data-ttu-id="9e487-139">3,0</span><span class="sxs-lookup"><span data-stu-id="9e487-139">3.0</span></span>  <br/> |<span data-ttu-id="9e487-140">Состояние магазина Office для почтового приложения изменилось.</span><span class="sxs-lookup"><span data-stu-id="9e487-140">The Office Store status for the mail app has changed.</span></span> <span data-ttu-id="9e487-141">Это может означать, что в почтовом приложении возникла проблема.</span><span class="sxs-lookup"><span data-stu-id="9e487-141">This may indicate that there is a problem with the mail app.</span></span> <span data-ttu-id="9e487-142">Чтобы получить дополнительные сведения, перейдите на страницу почтового приложения в магазине Office.</span><span class="sxs-lookup"><span data-stu-id="9e487-142">Go to the mail app page in the Office Store for more information.</span></span>  <br/> |
|<span data-ttu-id="9e487-143">3.1</span><span class="sxs-lookup"><span data-stu-id="9e487-143">3.1</span></span>  <br/> |<span data-ttu-id="9e487-144">Почтовое приложение удалено из магазина Office.</span><span class="sxs-lookup"><span data-stu-id="9e487-144">The mail app has been removed from the Office Store.</span></span>  <br/> |
|<span data-ttu-id="9e487-145">3.2</span><span class="sxs-lookup"><span data-stu-id="9e487-145">3.2</span></span>  <br/> |<span data-ttu-id="9e487-146">В почтовом приложении обнаружена проблема, которая временно снята из магазина Office.</span><span class="sxs-lookup"><span data-stu-id="9e487-146">A problem has been discovered with the mail app and it has temporarily been withdrawn from the Office Store.</span></span>  <br/> |
|<span data-ttu-id="9e487-147">3.3</span><span class="sxs-lookup"><span data-stu-id="9e487-147">3.3</span></span>  <br/> |<span data-ttu-id="9e487-148">Почтовое приложение будет удалено из магазина Office в течение 30 дней.</span><span class="sxs-lookup"><span data-stu-id="9e487-148">The mail app will be removed from the Office Store within 30 days.</span></span>  <br/> |
|<span data-ttu-id="9e487-149">4,0</span><span class="sxs-lookup"><span data-stu-id="9e487-149">4.0</span></span>  <br/> |<span data-ttu-id="9e487-150">Почтовый клиент автоматически отключил почтовое приложение.</span><span class="sxs-lookup"><span data-stu-id="9e487-150">The mail app has been automatically disabled by your mail client.</span></span>  <br/> |
|<span data-ttu-id="9e487-151">4.1</span><span class="sxs-lookup"><span data-stu-id="9e487-151">4.1</span></span>  <br/> |<span data-ttu-id="9e487-152">Почтовые приложения отключены в Outlook по соображениям производительности.</span><span class="sxs-lookup"><span data-stu-id="9e487-152">The mail app has been disabled by Outlook for performance reasons.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9e487-153">Примечания</span><span class="sxs-lookup"><span data-stu-id="9e487-153">Remarks</span></span>

<span data-ttu-id="9e487-154">Этот элемент появился в Exchange Server 2013 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="9e487-154">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="9e487-155">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="9e487-155">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9e487-156">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="9e487-156">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9e487-157">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="9e487-157">Namespace</span></span>  <br/> | https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9e487-158">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="9e487-158">Schema Name</span></span>  <br/> |<span data-ttu-id="9e487-159">Схема Types</span><span class="sxs-lookup"><span data-stu-id="9e487-159">Types schema</span></span>  <br/> |
|<span data-ttu-id="9e487-160">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="9e487-160">Validation File</span></span>  <br/> |<span data-ttu-id="9e487-161">Неприменимо</span><span class="sxs-lookup"><span data-stu-id="9e487-161">Not applicable</span></span>  <br/> |
|<span data-ttu-id="9e487-162">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="9e487-162">Can be Empty</span></span>  <br/> |<span data-ttu-id="9e487-163">False</span><span class="sxs-lookup"><span data-stu-id="9e487-163">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9e487-164">См. также</span><span class="sxs-lookup"><span data-stu-id="9e487-164">See also</span></span>

- [<span data-ttu-id="9e487-165">Метаданные</span><span class="sxs-lookup"><span data-stu-id="9e487-165">Metadata</span></span>](metadata-ex15websvcsotherref.md)
- [<span data-ttu-id="9e487-166">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="9e487-166">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

