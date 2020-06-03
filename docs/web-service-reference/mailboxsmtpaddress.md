---
title: маилбокссмтпаддресс
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
description: Элемент Маилбокссмтпаддресс представляет SMTP-адрес пользователя, чьи правила папки "Входящие" извлекаются или обновляются; или Дата окончания срока действия пароля, который необходимо получить.
ms.openlocfilehash: 613e8098210257280bec47f2b22a2d29d04fa07c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530546"
---
# <a name="mailboxsmtpaddress"></a><span data-ttu-id="e5f8d-103">маилбокссмтпаддресс</span><span class="sxs-lookup"><span data-stu-id="e5f8d-103">MailboxSmtpAddress</span></span>

<span data-ttu-id="e5f8d-104">Элемент **маилбокссмтпаддресс** представляет SMTP-адрес пользователя, чьи правила папки "Входящие" извлекаются или обновляются; или Дата окончания срока действия пароля, который необходимо получить.</span><span class="sxs-lookup"><span data-stu-id="e5f8d-104">The **MailboxSmtpAddress** element represents the SMTP address of the user whose Inbox rules are to be retrieved or updated; or whose password expiration date is to be retrieved.</span></span> 
  
```XML
<MailboxSmtpAddress/>
```

<span data-ttu-id="e5f8d-105">**строка**</span><span class="sxs-lookup"><span data-stu-id="e5f8d-105">**string**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="e5f8d-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e5f8d-106">Attributes and elements</span></span>

<span data-ttu-id="e5f8d-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="e5f8d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e5f8d-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e5f8d-108">Attributes</span></span>

<span data-ttu-id="e5f8d-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e5f8d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e5f8d-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e5f8d-110">Child elements</span></span>

<span data-ttu-id="e5f8d-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e5f8d-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e5f8d-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e5f8d-112">Parent elements</span></span>

|<span data-ttu-id="e5f8d-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e5f8d-113">**Element**</span></span>|<span data-ttu-id="e5f8d-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e5f8d-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e5f8d-115">GetInboxRules</span><span class="sxs-lookup"><span data-stu-id="e5f8d-115">GetInboxRules</span></span>](getinboxrules.md) <br/> |<span data-ttu-id="e5f8d-116">Определяет запрос на получение правил для папки "Входящие" для почтового ящика в хранилище сервера.</span><span class="sxs-lookup"><span data-stu-id="e5f8d-116">Defines a request to get the Inbox rules on a mailbox in the server store.</span></span>  <br/> |
|[<span data-ttu-id="e5f8d-117">GetPasswordExpirationDate</span><span class="sxs-lookup"><span data-stu-id="e5f8d-117">GetPasswordExpirationDate</span></span>](getpasswordexpirationdate.md) <br/> |<span data-ttu-id="e5f8d-118">Определяет запрос на получение даты истечения срока действия пароля учетной записи электронной почты.</span><span class="sxs-lookup"><span data-stu-id="e5f8d-118">Defines a request to get the password expiration date of an email account.</span></span>  <br/> |
|[<span data-ttu-id="e5f8d-119">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="e5f8d-119">UpdateInboxRules</span></span>](updateinboxrules.md) <br/> |<span data-ttu-id="e5f8d-120">Определяет запрос на обновление правил папки "Входящие" в почтовом ящике в хранилище сервера.</span><span class="sxs-lookup"><span data-stu-id="e5f8d-120">Defines a request to update the Inbox rules in a mailbox in the server store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e5f8d-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="e5f8d-121">Text value</span></span>

<span data-ttu-id="e5f8d-122">Нет.</span><span class="sxs-lookup"><span data-stu-id="e5f8d-122">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e5f8d-123">Примечания</span><span class="sxs-lookup"><span data-stu-id="e5f8d-123">Remarks</span></span>

<span data-ttu-id="e5f8d-124">Элемент **маилбокссмтпаддресс** является необязательным элементом.</span><span class="sxs-lookup"><span data-stu-id="e5f8d-124">The **MailboxSmtpAddress** element is an optional element.</span></span> <span data-ttu-id="e5f8d-125">Если элемент **маилбокссмтпаддресс** опущен, используется адрес пользователя, выполнившего вход в систему.</span><span class="sxs-lookup"><span data-stu-id="e5f8d-125">If the **MailboxSmtpAddress** element is omitted, the address of the logged on user is used.</span></span> 
  
<span data-ttu-id="e5f8d-126">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="e5f8d-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e5f8d-127">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e5f8d-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e5f8d-128">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e5f8d-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e5f8d-129">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e5f8d-129">Schema Name</span></span>  <br/> |<span data-ttu-id="e5f8d-130">Схема Types</span><span class="sxs-lookup"><span data-stu-id="e5f8d-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="e5f8d-131">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e5f8d-131">Validation File</span></span>  <br/> |<span data-ttu-id="e5f8d-132">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="e5f8d-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e5f8d-133">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e5f8d-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="e5f8d-134">True</span><span class="sxs-lookup"><span data-stu-id="e5f8d-134">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e5f8d-135">См. также</span><span class="sxs-lookup"><span data-stu-id="e5f8d-135">See also</span></span>

- [<span data-ttu-id="e5f8d-136">Операция GetInboxRules</span><span class="sxs-lookup"><span data-stu-id="e5f8d-136">GetInboxRules operation</span></span>](getinboxrules-operation.md)
- [<span data-ttu-id="e5f8d-137">Операция GetPasswordExpirationDate</span><span class="sxs-lookup"><span data-stu-id="e5f8d-137">GetPasswordExpirationDate operation</span></span>](getpasswordexpirationdate-operation.md)
- [<span data-ttu-id="e5f8d-138">Операция UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="e5f8d-138">UpdateInboxRules operation</span></span>](updateinboxrules-operation.md)
- [<span data-ttu-id="e5f8d-139">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="e5f8d-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

