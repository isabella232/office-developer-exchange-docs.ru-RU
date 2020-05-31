---
title: SenderSmtpAddress
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SenderSmtpAddress
api_type:
- schema
ms.assetid: e39c7df7-4bfa-455f-b4bb-1f1d05398eec
description: Элемент SenderSmtpAddress представляет адрес электронной почты SMTP, соответствующий почтовому ящику, содержащему папку, которая будет использоваться совместно.
ms.openlocfilehash: 70905dd1ae2c3df18224aceeea246b542d1338e3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835334"
---
# <a name="sendersmtpaddress"></a><span data-ttu-id="540f2-103">SenderSmtpAddress</span><span class="sxs-lookup"><span data-stu-id="540f2-103">SenderSmtpAddress</span></span>

<span data-ttu-id="540f2-104">Элемент **SenderSmtpAddress** представляет адрес электронной почты SMTP, соответствующий почтовому ящику, содержащему папку, которая будет использоваться совместно.</span><span class="sxs-lookup"><span data-stu-id="540f2-104">The **SenderSmtpAddress** element represents the SMTP e-mail address corresponding to the mailbox that contains the folder that will be shared.</span></span> 
  
```xml
<SenderSmtpAddress/>
```

 <span data-ttu-id="540f2-105">**нонемптистрингтипе**</span><span class="sxs-lookup"><span data-stu-id="540f2-105">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="540f2-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="540f2-106">Attributes and elements</span></span>

<span data-ttu-id="540f2-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="540f2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="540f2-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="540f2-108">Attributes</span></span>

<span data-ttu-id="540f2-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="540f2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="540f2-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="540f2-110">Child elements</span></span>

<span data-ttu-id="540f2-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="540f2-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="540f2-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="540f2-112">Parent elements</span></span>

|<span data-ttu-id="540f2-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="540f2-113">**Element**</span></span>|<span data-ttu-id="540f2-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="540f2-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="540f2-115">GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="540f2-115">GetSharingMetadata</span></span>](getsharingmetadata.md) <br/> |<span data-ttu-id="540f2-116">Определяет запрос на получение непрозрачного маркера проверки подлинности, который определяет приглашение к совместному использованию.</span><span class="sxs-lookup"><span data-stu-id="540f2-116">Defines a request to get an opaque authentication token that identifies the sharing invitation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="540f2-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="540f2-117">Text value</span></span>

<span data-ttu-id="540f2-118">Необходимо указать текстовое значение, представляющее SMTP-адрес.</span><span class="sxs-lookup"><span data-stu-id="540f2-118">A text value that represents an SMTP address is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="540f2-119">Примечания</span><span class="sxs-lookup"><span data-stu-id="540f2-119">Remarks</span></span>

<span data-ttu-id="540f2-120">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, на котором размещены веб-службы Exchange компьютера, на котором установлен сервер Microsoft Exchange, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="540f2-120">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="540f2-121">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="540f2-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="540f2-122">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="540f2-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="540f2-123">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="540f2-123">Schema Name</span></span>  <br/> |<span data-ttu-id="540f2-124">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="540f2-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="540f2-125">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="540f2-125">Validation File</span></span>  <br/> |<span data-ttu-id="540f2-126">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="540f2-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="540f2-127">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="540f2-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="540f2-128">False</span><span class="sxs-lookup"><span data-stu-id="540f2-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="540f2-129">См. также</span><span class="sxs-lookup"><span data-stu-id="540f2-129">See also</span></span>



[<span data-ttu-id="540f2-130">Операция GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="540f2-130">GetSharingMetadata operation</span></span>](getsharingmetadata-operation.md)


- [<span data-ttu-id="540f2-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="540f2-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

