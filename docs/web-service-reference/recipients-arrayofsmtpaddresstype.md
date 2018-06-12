---
title: Получатели (ArrayOfSmtpAddressType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Recipients
api_type:
- schema
ms.assetid: cf68417d-85cf-49e0-857a-f987d3675344
description: Элемент получателей указывает массив получателей сообщения.
ms.openlocfilehash: 8490988043b1e06fd3a8f553fcefaeb2e90e9d31
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834988"
---
# <a name="recipients-arrayofsmtpaddresstype"></a><span data-ttu-id="8a8a7-103">Получатели (ArrayOfSmtpAddressType)</span><span class="sxs-lookup"><span data-stu-id="8a8a7-103">Recipients (ArrayOfSmtpAddressType)</span></span>

<span data-ttu-id="8a8a7-104">Элемент **получателей** указывает массив получателей сообщения.</span><span class="sxs-lookup"><span data-stu-id="8a8a7-104">The **Recipients** element specifies an array of recipients of a message.</span></span> 
  
```xml
<Recipients>   <SmtpAddress/></Recipients>
```

 <span data-ttu-id="8a8a7-105">**ArrayOfSmtpAddressType**</span><span class="sxs-lookup"><span data-stu-id="8a8a7-105">**ArrayOfSmtpAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8a8a7-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="8a8a7-106">Attributes and elements</span></span>

<span data-ttu-id="8a8a7-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="8a8a7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8a8a7-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="8a8a7-108">Attributes</span></span>

<span data-ttu-id="8a8a7-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="8a8a7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8a8a7-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="8a8a7-110">Child elements</span></span>

|<span data-ttu-id="8a8a7-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="8a8a7-111">**Element**</span></span>|<span data-ttu-id="8a8a7-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8a8a7-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8a8a7-113">SmtpAddress</span><span class="sxs-lookup"><span data-stu-id="8a8a7-113">SmtpAddress</span></span>](smtpaddress.md) <br/> |<span data-ttu-id="8a8a7-114">Представляет адрес получателя Simple Mail Transfer Protocol (SMTP) календаря или контакта, запрос на общий доступ.</span><span class="sxs-lookup"><span data-stu-id="8a8a7-114">Represents the Simple Mail Transfer Protocol (SMTP) recipient address of a calendar or contact sharing request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8a8a7-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="8a8a7-115">Parent elements</span></span>

|<span data-ttu-id="8a8a7-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="8a8a7-116">**Element**</span></span>|<span data-ttu-id="8a8a7-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8a8a7-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8a8a7-118">GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="8a8a7-118">GetSharingMetadata</span></span>](getsharingmetadata.md) <br/> |<span data-ttu-id="8a8a7-119">Определяет запрос на получение маркера непрозрачный проверки подлинности, идентифицирующее приглашение к совместному использованию.</span><span class="sxs-lookup"><span data-stu-id="8a8a7-119">Defines a request to get an opaque authentication token that identifies the sharing invitation.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="8a8a7-120">Замечания</span><span class="sxs-lookup"><span data-stu-id="8a8a7-120">Remarks</span></span>

<span data-ttu-id="8a8a7-121">Схема, описывающая этот элемент находится в IIS виртуального каталога веб-служб Exchange узлов компьютера, на котором выполняется Microsoft Exchange Server, на наличие установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="8a8a7-121">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8a8a7-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="8a8a7-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8a8a7-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="8a8a7-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="8a8a7-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="8a8a7-124">Schema Name</span></span>  <br/> |<span data-ttu-id="8a8a7-125">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="8a8a7-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="8a8a7-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="8a8a7-126">Validation File</span></span>  <br/> |<span data-ttu-id="8a8a7-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="8a8a7-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="8a8a7-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="8a8a7-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="8a8a7-129">False</span><span class="sxs-lookup"><span data-stu-id="8a8a7-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8a8a7-130">См. также</span><span class="sxs-lookup"><span data-stu-id="8a8a7-130">See also</span></span>



[<span data-ttu-id="8a8a7-131">Операция GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="8a8a7-131">GetSharingMetadata operation</span></span>](getsharingmetadata-operation.md)


- [<span data-ttu-id="8a8a7-132">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="8a8a7-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

