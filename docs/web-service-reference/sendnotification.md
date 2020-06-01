---
title: сенднотификатион
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SendNotification
api_type:
- schema
ms.assetid: e45c4451-a286-4aec-a691-119ec41c58e0
description: Элемент Сенднотификатион содержит push-уведомления, отправленные компьютером, на котором работает Microsoft Exchange Server 2007, к клиентскому приложению.
ms.openlocfilehash: 49f2f6cb7f5c8e1171b54ff965ee1d22accc9bf2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462117"
---
# <a name="sendnotification"></a><span data-ttu-id="a1d63-103">сенднотификатион</span><span class="sxs-lookup"><span data-stu-id="a1d63-103">SendNotification</span></span>

<span data-ttu-id="a1d63-104">Элемент **сенднотификатион** содержит push-уведомления, отправленные компьютером, на котором работает Microsoft Exchange Server 2007, к клиентскому приложению.</span><span class="sxs-lookup"><span data-stu-id="a1d63-104">The **SendNotification** element contains the push notifications that are sent by the computer that is running Microsoft Exchange Server 2007 to the client application.</span></span> 
  
```xml
<SendNotification>
   <ResponseMessages/>
</SendNotification>
```

 <span data-ttu-id="a1d63-105">**сенднотификатионреспонсетипе**</span><span class="sxs-lookup"><span data-stu-id="a1d63-105">**SendNotificationResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a1d63-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="a1d63-106">Attributes and elements</span></span>

<span data-ttu-id="a1d63-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="a1d63-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a1d63-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="a1d63-108">Attributes</span></span>

<span data-ttu-id="a1d63-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="a1d63-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a1d63-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="a1d63-110">Child elements</span></span>

|<span data-ttu-id="a1d63-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a1d63-111">**Element**</span></span>|<span data-ttu-id="a1d63-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a1d63-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a1d63-113">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="a1d63-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="a1d63-114">Содержит push-уведомления, отправляемые сервером клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="a1d63-114">Contains the push notifications that are sent by the Client Access server.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a1d63-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="a1d63-115">Parent elements</span></span>

<span data-ttu-id="a1d63-116">Нет.</span><span class="sxs-lookup"><span data-stu-id="a1d63-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a1d63-117">Примечания</span><span class="sxs-lookup"><span data-stu-id="a1d63-117">Remarks</span></span>

<span data-ttu-id="a1d63-118">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="a1d63-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a1d63-119">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="a1d63-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a1d63-120">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="a1d63-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a1d63-121">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="a1d63-121">Schema Name</span></span>  <br/> |<span data-ttu-id="a1d63-122">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="a1d63-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a1d63-123">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="a1d63-123">Validation File</span></span>  <br/> |<span data-ttu-id="a1d63-124">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="a1d63-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a1d63-125">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="a1d63-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="a1d63-126">False</span><span class="sxs-lookup"><span data-stu-id="a1d63-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a1d63-127">См. также</span><span class="sxs-lookup"><span data-stu-id="a1d63-127">See also</span></span>



- [<span data-ttu-id="a1d63-128">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="a1d63-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="a1d63-129">Уведомления о событиях в EWS</span><span class="sxs-lookup"><span data-stu-id="a1d63-129">Event notifications in EWS</span></span>](https://msdn.microsoft.com/library/4fd4b351-d35c-4ccc-9ed9-878932ab9d50%28Office.15%29.aspx)
  
[<span data-ttu-id="a1d63-130">Пример приложения для push-уведомлений</span><span class="sxs-lookup"><span data-stu-id="a1d63-130">Push Notification Sample Application</span></span>](https://msdn.microsoft.com/library/db1f8523-fa44-483f-bdb6-ab5939b52eee%28Office.15%29.aspx)

