---
title: Жетумпропертиесреспонсе (веб-служба единой системы обмена сообщениями)
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
description: Элемент Жетумпропертиесреспонсе определяет ответ на запрос для операции GetUMProperties (веб-служба единой системы обмена сообщениями).
ms.openlocfilehash: 3247489a305c694c10764d7a0c6f02b1fad51ebf
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459127"
---
# <a name="getumpropertiesresponse-um-web-service"></a><span data-ttu-id="27622-103">Жетумпропертиесреспонсе (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="27622-103">GetUMPropertiesResponse (UM web service)</span></span>

<span data-ttu-id="27622-104">Элемент **жетумпропертиесреспонсе** определяет ответ на запрос для [операции GetUMProperties (веб-служба единой системы обмена сообщениями)](getumproperties-operation-um-web-service.md) .</span><span class="sxs-lookup"><span data-stu-id="27622-104">The **GetUMPropertiesResponse** element defines a response to a [GetUMProperties operation (UM web service)](getumproperties-operation-um-web-service.md) request.</span></span> 
  
[<span data-ttu-id="27622-105">Жетумпропертиесреспонсе (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="27622-105">GetUMPropertiesResponse (UM web service)</span></span>](getumpropertiesresponse-um-web-service.md)
  
```xml
<GetUMPropertiesResponse>
  <OofStatus/>
  <MissedCallNotificationEnabled/>
  <PlayOnPhoneDialString/>
  <TelephoneAccessNumbers/>
  <TelephoneAccessFolderEmail/>
</GetUMPropertiesResponse>
```

 <span data-ttu-id="27622-106">**умпропертиес**</span><span class="sxs-lookup"><span data-stu-id="27622-106">**UMProperties**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="27622-107">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="27622-107">Attributes and elements</span></span>

<span data-ttu-id="27622-108">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="27622-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="27622-109">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="27622-109">Attributes</span></span>

<span data-ttu-id="27622-110">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="27622-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="27622-111">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="27622-111">Child elements</span></span>

|<span data-ttu-id="27622-112">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="27622-112">**Element**</span></span>|<span data-ttu-id="27622-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="27622-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="27622-114">MissedCallNotificationEnabled (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="27622-114">MissedCallNotificationEnabled (UM web service)</span></span>](missedcallnotificationenabled-um-web-service.md) <br/> |<span data-ttu-id="27622-115">Указывает, включены ли уведомления о пропущенных вызовах.</span><span class="sxs-lookup"><span data-stu-id="27622-115">Indicates whether missed call notifications are enabled.</span></span>  <br/> |
|[<span data-ttu-id="27622-116">Плайонфонедиалстринг (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="27622-116">PlayOnPhoneDialString (UM web service)</span></span>](playonphonedialstring-um-web-service.md) <br/> |<span data-ttu-id="27622-117">Содержит строку набора номера, используемую по умолчанию для [операции PlayOnPhone (веб-служба единой системы обмена сообщениями)](playonphone-operation-um-web-service.md) и [операцию PlayOnPhoneGreeting (веб-служба единой системы обмена сообщениями)](playonphonegreeting-operation-um-web-service.md).</span><span class="sxs-lookup"><span data-stu-id="27622-117">Contains the default dial string to use for the [PlayOnPhone operation (UM web service)](playonphone-operation-um-web-service.md) and [PlayOnPhoneGreeting operation (UM web service)](playonphonegreeting-operation-um-web-service.md).</span></span>  <br/> |
|[<span data-ttu-id="27622-118">Телефонеакцесснумберс (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="27622-118">TelephoneAccessNumbers (UM web service)</span></span>](telephoneaccessnumbers-um-web-service.md) <br/> |<span data-ttu-id="27622-119">Содержит список номеров телефонов, которые пользователь может использовать для доступа к единой системе обмена сообщениями по телефону.</span><span class="sxs-lookup"><span data-stu-id="27622-119">Contains the list of telephone numbers the user can use to access Unified Messaging via a telephone.</span></span>  <br/> |
|[<span data-ttu-id="27622-120">Телефонеакцессфолдеремаил (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="27622-120">TelephoneAccessFolderEmail (UM web service)</span></span>](telephoneaccessfolderemail-um-web-service.md) <br/> |<span data-ttu-id="27622-121">Содержит идентификатор для папки электронной почты, из которой единая система обмена сообщениями будет читать сообщения по телефону.</span><span class="sxs-lookup"><span data-stu-id="27622-121">Contains the identifier for the e-mail folder from which Unified Messaging will read messages over the telephone.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="27622-122">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="27622-122">Parent elements</span></span>

<span data-ttu-id="27622-123">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="27622-123">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="27622-124">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="27622-124">Text value</span></span>

<span data-ttu-id="27622-125">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="27622-125">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="27622-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="27622-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="27622-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="27622-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="27622-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="27622-128">Schema Name</span></span>  <br/> |<span data-ttu-id="27622-129">Сообщения</span><span class="sxs-lookup"><span data-stu-id="27622-129">Messages</span></span>  <br/> |
|<span data-ttu-id="27622-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="27622-130">Validation File</span></span>  <br/> |<span data-ttu-id="27622-131">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="27622-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="27622-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="27622-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="27622-133">False</span><span class="sxs-lookup"><span data-stu-id="27622-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="27622-134">См. также</span><span class="sxs-lookup"><span data-stu-id="27622-134">See also</span></span>



[<span data-ttu-id="27622-135">Операция GetUMProperties (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="27622-135">GetUMProperties operation (UM web service)</span></span>](getumproperties-operation-um-web-service.md)

