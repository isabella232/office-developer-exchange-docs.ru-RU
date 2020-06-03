---
title: Получатели (Аррайофсмтпаддресстипе)
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
description: Элемент Recipients указывает массив получателей сообщения.
ms.openlocfilehash: 4c2478a81836c2e52baad9c928d112108679b837
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465508"
---
# <a name="recipients-arrayofsmtpaddresstype"></a><span data-ttu-id="cb1fa-103">Получатели (Аррайофсмтпаддресстипе)</span><span class="sxs-lookup"><span data-stu-id="cb1fa-103">Recipients (ArrayOfSmtpAddressType)</span></span>

<span data-ttu-id="cb1fa-104">Элемент **Recipients** указывает массив получателей сообщения.</span><span class="sxs-lookup"><span data-stu-id="cb1fa-104">The **Recipients** element specifies an array of recipients of a message.</span></span> 
  
```xml
<Recipients>   <SmtpAddress/></Recipients>
```

 <span data-ttu-id="cb1fa-105">**аррайофсмтпаддресстипе**</span><span class="sxs-lookup"><span data-stu-id="cb1fa-105">**ArrayOfSmtpAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cb1fa-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="cb1fa-106">Attributes and elements</span></span>

<span data-ttu-id="cb1fa-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="cb1fa-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cb1fa-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="cb1fa-108">Attributes</span></span>

<span data-ttu-id="cb1fa-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="cb1fa-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cb1fa-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="cb1fa-110">Child elements</span></span>

|<span data-ttu-id="cb1fa-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="cb1fa-111">**Element**</span></span>|<span data-ttu-id="cb1fa-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="cb1fa-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cb1fa-113">SmtpAddress</span><span class="sxs-lookup"><span data-stu-id="cb1fa-113">SmtpAddress</span></span>](smtpaddress.md) <br/> |<span data-ttu-id="cb1fa-114">Представляет адрес получателя протокола SMTP для запроса на общий доступ к календарю или контакту.</span><span class="sxs-lookup"><span data-stu-id="cb1fa-114">Represents the Simple Mail Transfer Protocol (SMTP) recipient address of a calendar or contact sharing request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="cb1fa-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="cb1fa-115">Parent elements</span></span>

|<span data-ttu-id="cb1fa-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="cb1fa-116">**Element**</span></span>|<span data-ttu-id="cb1fa-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="cb1fa-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cb1fa-118">GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="cb1fa-118">GetSharingMetadata</span></span>](getsharingmetadata.md) <br/> |<span data-ttu-id="cb1fa-119">Определяет запрос на получение непрозрачного маркера проверки подлинности, который определяет приглашение к совместному использованию.</span><span class="sxs-lookup"><span data-stu-id="cb1fa-119">Defines a request to get an opaque authentication token that identifies the sharing invitation.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="cb1fa-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="cb1fa-120">Remarks</span></span>

<span data-ttu-id="cb1fa-121">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, на котором размещены веб-службы Exchange компьютера, на котором установлен сервер Microsoft Exchange, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="cb1fa-121">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cb1fa-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="cb1fa-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cb1fa-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="cb1fa-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="cb1fa-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="cb1fa-124">Schema Name</span></span>  <br/> |<span data-ttu-id="cb1fa-125">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="cb1fa-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="cb1fa-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="cb1fa-126">Validation File</span></span>  <br/> |<span data-ttu-id="cb1fa-127">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="cb1fa-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="cb1fa-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="cb1fa-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="cb1fa-129">False</span><span class="sxs-lookup"><span data-stu-id="cb1fa-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cb1fa-130">См. также</span><span class="sxs-lookup"><span data-stu-id="cb1fa-130">See also</span></span>



[<span data-ttu-id="cb1fa-131">Операция GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="cb1fa-131">GetSharingMetadata operation</span></span>](getsharingmetadata-operation.md)


- [<span data-ttu-id="cb1fa-132">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="cb1fa-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

