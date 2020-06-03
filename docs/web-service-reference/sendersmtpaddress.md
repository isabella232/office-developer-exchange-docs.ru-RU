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
ms.openlocfilehash: 73047dcecfbccb55d74e373891c3154bc7baeeba
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464898"
---
# <a name="sendersmtpaddress"></a><span data-ttu-id="bc0a0-103">SenderSmtpAddress</span><span class="sxs-lookup"><span data-stu-id="bc0a0-103">SenderSmtpAddress</span></span>

<span data-ttu-id="bc0a0-104">Элемент **SenderSmtpAddress** представляет адрес электронной почты SMTP, соответствующий почтовому ящику, содержащему папку, которая будет использоваться совместно.</span><span class="sxs-lookup"><span data-stu-id="bc0a0-104">The **SenderSmtpAddress** element represents the SMTP e-mail address corresponding to the mailbox that contains the folder that will be shared.</span></span> 
  
```xml
<SenderSmtpAddress/>
```

 <span data-ttu-id="bc0a0-105">**нонемптистрингтипе**</span><span class="sxs-lookup"><span data-stu-id="bc0a0-105">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bc0a0-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="bc0a0-106">Attributes and elements</span></span>

<span data-ttu-id="bc0a0-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="bc0a0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bc0a0-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="bc0a0-108">Attributes</span></span>

<span data-ttu-id="bc0a0-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="bc0a0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bc0a0-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="bc0a0-110">Child elements</span></span>

<span data-ttu-id="bc0a0-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="bc0a0-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="bc0a0-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="bc0a0-112">Parent elements</span></span>

|<span data-ttu-id="bc0a0-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="bc0a0-113">**Element**</span></span>|<span data-ttu-id="bc0a0-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bc0a0-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bc0a0-115">GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="bc0a0-115">GetSharingMetadata</span></span>](getsharingmetadata.md) <br/> |<span data-ttu-id="bc0a0-116">Определяет запрос на получение непрозрачного маркера проверки подлинности, который определяет приглашение к совместному использованию.</span><span class="sxs-lookup"><span data-stu-id="bc0a0-116">Defines a request to get an opaque authentication token that identifies the sharing invitation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="bc0a0-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="bc0a0-117">Text value</span></span>

<span data-ttu-id="bc0a0-118">Необходимо указать текстовое значение, представляющее SMTP-адрес.</span><span class="sxs-lookup"><span data-stu-id="bc0a0-118">A text value that represents an SMTP address is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="bc0a0-119">Примечания</span><span class="sxs-lookup"><span data-stu-id="bc0a0-119">Remarks</span></span>

<span data-ttu-id="bc0a0-120">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, на котором размещены веб-службы Exchange компьютера, на котором установлен сервер Microsoft Exchange, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="bc0a0-120">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bc0a0-121">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="bc0a0-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bc0a0-122">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="bc0a0-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="bc0a0-123">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="bc0a0-123">Schema Name</span></span>  <br/> |<span data-ttu-id="bc0a0-124">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="bc0a0-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="bc0a0-125">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="bc0a0-125">Validation File</span></span>  <br/> |<span data-ttu-id="bc0a0-126">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="bc0a0-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="bc0a0-127">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="bc0a0-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="bc0a0-128">False</span><span class="sxs-lookup"><span data-stu-id="bc0a0-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bc0a0-129">См. также</span><span class="sxs-lookup"><span data-stu-id="bc0a0-129">See also</span></span>



[<span data-ttu-id="bc0a0-130">Операция GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="bc0a0-130">GetSharingMetadata operation</span></span>](getsharingmetadata-operation.md)


- [<span data-ttu-id="bc0a0-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="bc0a0-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

