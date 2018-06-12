---
title: GetUMPropertiesResponse (веб-служба единой системы обмена СООБЩЕНИЯМИ)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- GetUMPropertiesResponse
api_type:
- schema
ms.assetid: fcd93ce5-7403-46a9-b46e-56d2ebdd2f79
description: Элемент GetUMPropertiesResponse определяет ответа на запрос GetUMProperties операции (веб-служба единой системы обмена СООБЩЕНИЯМИ).
ms.openlocfilehash: c0df872ad6b8e6541fa750ab87f4c1e5f0118b00
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833685"
---
# <a name="getumpropertiesresponse-um-web-service"></a><span data-ttu-id="d24c2-103">GetUMPropertiesResponse (веб-служба единой системы обмена СООБЩЕНИЯМИ)</span><span class="sxs-lookup"><span data-stu-id="d24c2-103">GetUMPropertiesResponse (UM web service)</span></span>

<span data-ttu-id="d24c2-104">Элемент **GetUMPropertiesResponse** определяет ответ на запрос [операции GetUMProperties (веб-служба единой системы обмена СООБЩЕНИЯМИ)](getumproperties-operation-um-web-service.md) .</span><span class="sxs-lookup"><span data-stu-id="d24c2-104">The **GetUMPropertiesResponse** element defines a response to a [GetUMProperties operation (UM web service)](getumproperties-operation-um-web-service.md) request.</span></span> 
  
[<span data-ttu-id="d24c2-105">GetUMPropertiesResponse (веб-служба единой системы обмена СООБЩЕНИЯМИ)</span><span class="sxs-lookup"><span data-stu-id="d24c2-105">GetUMPropertiesResponse (UM web service)</span></span>](getumpropertiesresponse-um-web-service.md)
  
```xml
<GetUMPropertiesResponse>
  <OofStatus/>
  <MissedCallNotificationEnabled/>
  <PlayOnPhoneDialString/>
  <TelephoneAccessNumbers/>
  <TelephoneAccessFolderEmail/>
</GetUMPropertiesResponse>
```

 <span data-ttu-id="d24c2-106">**UMProperties**</span><span class="sxs-lookup"><span data-stu-id="d24c2-106">**UMProperties**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d24c2-107">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d24c2-107">Attributes and elements</span></span>

<span data-ttu-id="d24c2-108">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="d24c2-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d24c2-109">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d24c2-109">Attributes</span></span>

<span data-ttu-id="d24c2-110">Нет.</span><span class="sxs-lookup"><span data-stu-id="d24c2-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d24c2-111">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d24c2-111">Child elements</span></span>

|<span data-ttu-id="d24c2-112">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d24c2-112">**Element**</span></span>|<span data-ttu-id="d24c2-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d24c2-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d24c2-114">MissedCallNotificationEnabled (веб-служба единой системы обмена СООБЩЕНИЯМИ)</span><span class="sxs-lookup"><span data-stu-id="d24c2-114">MissedCallNotificationEnabled (UM web service)</span></span>](missedcallnotificationenabled-um-web-service.md) <br/> |<span data-ttu-id="d24c2-115">Указывает, включены ли уведомления о пропущенных вызовах.</span><span class="sxs-lookup"><span data-stu-id="d24c2-115">Indicates whether missed call notifications are enabled.</span></span>  <br/> |
|[<span data-ttu-id="d24c2-116">PlayOnPhoneDialString (веб-служба единой системы обмена СООБЩЕНИЯМИ)</span><span class="sxs-lookup"><span data-stu-id="d24c2-116">PlayOnPhoneDialString (UM web service)</span></span>](playonphonedialstring-um-web-service.md) <br/> |<span data-ttu-id="d24c2-117">Содержит строку звонков по умолчанию для [операции PlayOnPhone (веб-служба единой системы обмена СООБЩЕНИЯМИ)](playonphone-operation-um-web-service.md) и [PlayOnPhoneGreeting операции (веб-служба единой системы обмена СООБЩЕНИЯМИ)](playonphonegreeting-operation-um-web-service.md).</span><span class="sxs-lookup"><span data-stu-id="d24c2-117">Contains the default dial string to use for the [PlayOnPhone operation (UM web service)](playonphone-operation-um-web-service.md) and [PlayOnPhoneGreeting operation (UM web service)](playonphonegreeting-operation-um-web-service.md).</span></span>  <br/> |
|[<span data-ttu-id="d24c2-118">TelephoneAccessNumbers (веб-служба единой системы обмена СООБЩЕНИЯМИ)</span><span class="sxs-lookup"><span data-stu-id="d24c2-118">TelephoneAccessNumbers (UM web service)</span></span>](telephoneaccessnumbers-um-web-service.md) <br/> |<span data-ttu-id="d24c2-119">Содержит список телефонных номеров, которые пользователь может использовать для доступа к единой системе обмена сообщениями по телефону.</span><span class="sxs-lookup"><span data-stu-id="d24c2-119">Contains the list of telephone numbers the user can use to access Unified Messaging via a telephone.</span></span>  <br/> |
|[<span data-ttu-id="d24c2-120">TelephoneAccessFolderEmail (веб-служба единой системы обмена СООБЩЕНИЯМИ)</span><span class="sxs-lookup"><span data-stu-id="d24c2-120">TelephoneAccessFolderEmail (UM web service)</span></span>](telephoneaccessfolderemail-um-web-service.md) <br/> |<span data-ttu-id="d24c2-121">Содержит идентификатор для папки электронной почты, из которого единой системы обмена сообщениями будет читать сообщения по телефону.</span><span class="sxs-lookup"><span data-stu-id="d24c2-121">Contains the identifier for the e-mail folder from which Unified Messaging will read messages over the telephone.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d24c2-122">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d24c2-122">Parent elements</span></span>

<span data-ttu-id="d24c2-123">Нет.</span><span class="sxs-lookup"><span data-stu-id="d24c2-123">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="d24c2-124">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="d24c2-124">Text value</span></span>

<span data-ttu-id="d24c2-125">Нет.</span><span class="sxs-lookup"><span data-stu-id="d24c2-125">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d24c2-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d24c2-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d24c2-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d24c2-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d24c2-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d24c2-128">Schema Name</span></span>  <br/> |<span data-ttu-id="d24c2-129">Сообщения</span><span class="sxs-lookup"><span data-stu-id="d24c2-129">Messages</span></span>  <br/> |
|<span data-ttu-id="d24c2-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d24c2-130">Validation File</span></span>  <br/> |<span data-ttu-id="d24c2-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d24c2-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d24c2-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d24c2-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="d24c2-133">False</span><span class="sxs-lookup"><span data-stu-id="d24c2-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d24c2-134">См. также</span><span class="sxs-lookup"><span data-stu-id="d24c2-134">See also</span></span>



[<span data-ttu-id="d24c2-135">Операция GetUMProperties (веб-служба единой системы обмена СООБЩЕНИЯМИ)</span><span class="sxs-lookup"><span data-stu-id="d24c2-135">GetUMProperties operation (UM web service)</span></span>](getumproperties-operation-um-web-service.md)

