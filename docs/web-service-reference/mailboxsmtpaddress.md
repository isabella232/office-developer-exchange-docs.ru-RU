---
title: MailboxSmtpAddress
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MailboxSmtpAddress
api_type:
- schema
ms.assetid: de7c9035-ebbc-4473-ac14-3b22ce62768c
description: Элемент MailboxSmtpAddress представляет SMTP-адрес пользователя, которого правила папки «Входящие», чтобы извлечь или обновить; или, Дата истечения срока действия пароля нужно вернуть.
ms.openlocfilehash: 60b2c018f2a05e9630e92e28de1054a421b41e52
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834303"
---
# <a name="mailboxsmtpaddress"></a><span data-ttu-id="5fe40-103">MailboxSmtpAddress</span><span class="sxs-lookup"><span data-stu-id="5fe40-103">MailboxSmtpAddress</span></span>

<span data-ttu-id="5fe40-104">Элемент **MailboxSmtpAddress** представляет SMTP-адрес пользователя, которого правила папки «Входящие», чтобы извлечь или обновить; или, Дата истечения срока действия пароля нужно вернуть.</span><span class="sxs-lookup"><span data-stu-id="5fe40-104">The **MailboxSmtpAddress** element represents the SMTP address of the user whose Inbox rules are to be retrieved or updated; or whose password expiration date is to be retrieved.</span></span> 
  
```XML
<MailboxSmtpAddress/>
```

<span data-ttu-id="5fe40-105">**string**</span><span class="sxs-lookup"><span data-stu-id="5fe40-105">**string**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="5fe40-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="5fe40-106">Attributes and elements</span></span>

<span data-ttu-id="5fe40-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="5fe40-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5fe40-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="5fe40-108">Attributes</span></span>

<span data-ttu-id="5fe40-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="5fe40-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5fe40-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="5fe40-110">Child elements</span></span>

<span data-ttu-id="5fe40-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="5fe40-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5fe40-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="5fe40-112">Parent elements</span></span>

|<span data-ttu-id="5fe40-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="5fe40-113">**Element**</span></span>|<span data-ttu-id="5fe40-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="5fe40-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5fe40-115">GetInboxRules</span><span class="sxs-lookup"><span data-stu-id="5fe40-115">GetInboxRules</span></span>](getinboxrules.md) <br/> |<span data-ttu-id="5fe40-116">Определяет запрос на получение правил папки "Входящие" почтового ящика в хранилище сервера.</span><span class="sxs-lookup"><span data-stu-id="5fe40-116">Defines a request to get the Inbox rules on a mailbox in the server store.</span></span>  <br/> |
|[<span data-ttu-id="5fe40-117">GetPasswordExpirationDate</span><span class="sxs-lookup"><span data-stu-id="5fe40-117">GetPasswordExpirationDate</span></span>](getpasswordexpirationdate.md) <br/> |<span data-ttu-id="5fe40-118">Определяет запрос на получение срок действия пароля учетной записи электронной почты.</span><span class="sxs-lookup"><span data-stu-id="5fe40-118">Defines a request to get the password expiration date of an email account.</span></span>  <br/> |
|[<span data-ttu-id="5fe40-119">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="5fe40-119">UpdateInboxRules</span></span>](updateinboxrules.md) <br/> |<span data-ttu-id="5fe40-120">Определяет запрос на обновление правил папки "Входящие" почтового ящика в хранилище сервера.</span><span class="sxs-lookup"><span data-stu-id="5fe40-120">Defines a request to update the Inbox rules in a mailbox in the server store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5fe40-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="5fe40-121">Text value</span></span>

<span data-ttu-id="5fe40-122">Нет.</span><span class="sxs-lookup"><span data-stu-id="5fe40-122">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5fe40-123">Замечания</span><span class="sxs-lookup"><span data-stu-id="5fe40-123">Remarks</span></span>

<span data-ttu-id="5fe40-124">Элемент **MailboxSmtpAddress** — это необязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="5fe40-124">The **MailboxSmtpAddress** element is an optional element.</span></span> <span data-ttu-id="5fe40-125">Если элемент **MailboxSmtpAddress** опущен, используется адрес пользователя, выполнившего вход.</span><span class="sxs-lookup"><span data-stu-id="5fe40-125">If the **MailboxSmtpAddress** element is omitted, the address of the logged on user is used.</span></span> 
  
<span data-ttu-id="5fe40-126">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="5fe40-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5fe40-127">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="5fe40-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5fe40-128">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="5fe40-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5fe40-129">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="5fe40-129">Schema Name</span></span>  <br/> |<span data-ttu-id="5fe40-130">Схема Types</span><span class="sxs-lookup"><span data-stu-id="5fe40-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="5fe40-131">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="5fe40-131">Validation File</span></span>  <br/> |<span data-ttu-id="5fe40-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="5fe40-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5fe40-133">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="5fe40-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="5fe40-134">True</span><span class="sxs-lookup"><span data-stu-id="5fe40-134">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5fe40-135">См. также</span><span class="sxs-lookup"><span data-stu-id="5fe40-135">See also</span></span>

- [<span data-ttu-id="5fe40-136">Операция GetInboxRules</span><span class="sxs-lookup"><span data-stu-id="5fe40-136">GetInboxRules operation</span></span>](getinboxrules-operation.md)
- [<span data-ttu-id="5fe40-137">Операция GetPasswordExpirationDate</span><span class="sxs-lookup"><span data-stu-id="5fe40-137">GetPasswordExpirationDate operation</span></span>](getpasswordexpirationdate-operation.md)
- [<span data-ttu-id="5fe40-138">Операция UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="5fe40-138">UpdateInboxRules operation</span></span>](updateinboxrules-operation.md)
- [<span data-ttu-id="5fe40-139">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="5fe40-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

