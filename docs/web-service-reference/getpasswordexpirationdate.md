---
title: GetPasswordExpirationDate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f4f958ed-9cf4-4ebf-9b01-e2df9a7cbd63
description: Элемент GetPasswordExpirationDate определяет запрос на получение срок действия пароля для учетной записи электронной почты. Этот элемент является базовый элемент для операции GetPasswordExpirationDate операции.
ms.openlocfilehash: a9e0955566372f7b99c48c56e62ce2c5025f9f95
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762877"
---
# <a name="getpasswordexpirationdate"></a><span data-ttu-id="02fa6-104">GetPasswordExpirationDate</span><span class="sxs-lookup"><span data-stu-id="02fa6-104">GetPasswordExpirationDate</span></span>

<span data-ttu-id="02fa6-105">Элемент **GetPasswordExpirationDate** определяет запрос на получение срок действия пароля для учетной записи электронной почты.</span><span class="sxs-lookup"><span data-stu-id="02fa6-105">The **GetPasswordExpirationDate** element defines a request to get the password expiration date for an email account.</span></span> <span data-ttu-id="02fa6-106">Этот элемент является базовый элемент для операции [GetPasswordExpirationDate операции](getpasswordexpirationdate-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="02fa6-106">This element is the base element for the [GetPasswordExpirationDate operation](getpasswordexpirationdate-operation.md) operation.</span></span> 
  
```XML
<GetPasswordExpirationDate>
    <MailboxSmtpAddress/>
</GetPasswordExpirationDate>
```

 <span data-ttu-id="02fa6-107">**GetPasswordExpirationDateType**</span><span class="sxs-lookup"><span data-stu-id="02fa6-107">**GetPasswordExpirationDateType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="02fa6-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="02fa6-108">Attributes and elements</span></span>

<span data-ttu-id="02fa6-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="02fa6-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="02fa6-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="02fa6-110">Attributes</span></span>

<span data-ttu-id="02fa6-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="02fa6-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="02fa6-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="02fa6-112">Child elements</span></span>

|<span data-ttu-id="02fa6-113">**Имя элемента**</span><span class="sxs-lookup"><span data-stu-id="02fa6-113">**Element name**</span></span>|<span data-ttu-id="02fa6-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="02fa6-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="02fa6-115">MailboxSmtpAddress</span><span class="sxs-lookup"><span data-stu-id="02fa6-115">MailboxSmtpAddress</span></span>](mailboxsmtpaddress.md) <br/> |<span data-ttu-id="02fa6-116">Представляет собой адрес электронной почты учетной записи электронной почты, для которого срок действия пароля — это должно быть возвращено.</span><span class="sxs-lookup"><span data-stu-id="02fa6-116">Represents the email address of the email account for which the password expiration date is to be returned.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="02fa6-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="02fa6-117">Parent elements</span></span>

<span data-ttu-id="02fa6-118">Нет.</span><span class="sxs-lookup"><span data-stu-id="02fa6-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="02fa6-119">Замечания</span><span class="sxs-lookup"><span data-stu-id="02fa6-119">Remarks</span></span>

<span data-ttu-id="02fa6-120">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="02fa6-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="02fa6-121">Этот элемент появился в Exchange Server 2010 с пакетом обновления 2 (SP2).</span><span class="sxs-lookup"><span data-stu-id="02fa6-121">This element was introduced in Exchange Server 2010 Service Pack 2 (SP2).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="02fa6-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="02fa6-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="02fa6-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="02fa6-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="02fa6-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="02fa6-124">Schema Name</span></span>  <br/> |<span data-ttu-id="02fa6-125">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="02fa6-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="02fa6-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="02fa6-126">Validation File</span></span>  <br/> |<span data-ttu-id="02fa6-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="02fa6-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="02fa6-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="02fa6-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="02fa6-129">False</span><span class="sxs-lookup"><span data-stu-id="02fa6-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="02fa6-130">См. также</span><span class="sxs-lookup"><span data-stu-id="02fa6-130">See also</span></span>



[<span data-ttu-id="02fa6-131">Операция GetPasswordExpirationDate</span><span class="sxs-lookup"><span data-stu-id="02fa6-131">GetPasswordExpirationDate operation</span></span>](getpasswordexpirationdate-operation.md)


- [<span data-ttu-id="02fa6-132">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="02fa6-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

