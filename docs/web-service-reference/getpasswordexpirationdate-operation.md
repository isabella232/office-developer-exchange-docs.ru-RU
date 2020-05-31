---
title: Операция GetPasswordExpirationDate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: b0297458-58fb-4e5d-bb47-0cd17155e106
description: Операция GetPasswordExpirationDate предоставляет срок действия пароля учетной записи электронной почты для текущего пользователя.
ms.openlocfilehash: c57942c88b09a910e2d529a12ea279bb2da5d693
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762874"
---
# <a name="getpasswordexpirationdate-operation"></a><span data-ttu-id="e4779-103">Операция GetPasswordExpirationDate</span><span class="sxs-lookup"><span data-stu-id="e4779-103">GetPasswordExpirationDate operation</span></span>

<span data-ttu-id="e4779-104">Операция **GetPasswordExpirationDate** предоставляет срок действия пароля учетной записи электронной почты для текущего пользователя.</span><span class="sxs-lookup"><span data-stu-id="e4779-104">The **GetPasswordExpirationDate** operation provides the email account password expiration date for the current user.</span></span> 
  
<span data-ttu-id="e4779-105">Эта операция появилась в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="e4779-105">This operation was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="getpasswordexpirationdate-operation-soap-headers"></a><span data-ttu-id="e4779-106">Заголовки SOAP операции GetPasswordExpirationDate</span><span class="sxs-lookup"><span data-stu-id="e4779-106">GetPasswordExpirationDate operation SOAP headers</span></span>

<span data-ttu-id="e4779-107">Операция **GetPasswordExpirationDate** может использовать заголовки SOAP, указанные в приведенной ниже таблице.</span><span class="sxs-lookup"><span data-stu-id="e4779-107">The **GetPasswordExpirationDate** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="e4779-108">**Header**</span><span class="sxs-lookup"><span data-stu-id="e4779-108">**Header**</span></span>|<span data-ttu-id="e4779-109">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e4779-109">**Element**</span></span>|<span data-ttu-id="e4779-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e4779-110">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="e4779-111">**маилбокскултуре**</span><span class="sxs-lookup"><span data-stu-id="e4779-111">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="e4779-112">маилбокскултуре</span><span class="sxs-lookup"><span data-stu-id="e4779-112">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="e4779-113">Определяет язык и региональные параметры, определенные в документе RFC 3066 "Теги для идентификации языков", которые будут использоваться для доступа к почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="e4779-113">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="e4779-114">Это относится к запросу.</span><span class="sxs-lookup"><span data-stu-id="e4779-114">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="e4779-115">**рекуестверсион**</span><span class="sxs-lookup"><span data-stu-id="e4779-115">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="e4779-116">рекуестсерверверсион</span><span class="sxs-lookup"><span data-stu-id="e4779-116">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="e4779-117">Определяет схему запроса операции.</span><span class="sxs-lookup"><span data-stu-id="e4779-117">Identifies the schema for the operation request.</span></span> <span data-ttu-id="e4779-118">Это относится к запросу.</span><span class="sxs-lookup"><span data-stu-id="e4779-118">This is applicable to a request.</span></span> <span data-ttu-id="e4779-119">Это относится к запросу.</span><span class="sxs-lookup"><span data-stu-id="e4779-119">This is applicable to a request.</span></span>  <br/> |
   
## <a name="getpasswordexpirationdate-operation-request-example"></a><span data-ttu-id="e4779-120">Пример запроса операции GetPasswordExpirationDate</span><span class="sxs-lookup"><span data-stu-id="e4779-120">GetPasswordExpirationDate operation request example</span></span>

### <a name="description"></a><span data-ttu-id="e4779-121">Описание</span><span class="sxs-lookup"><span data-stu-id="e4779-121">Description</span></span>

<span data-ttu-id="e4779-122">В приведенном ниже примере запроса операции **GetPasswordExpirationDate** показано, как получить срок действия пароля для учетной записи электронной почты.</span><span class="sxs-lookup"><span data-stu-id="e4779-122">The following example of a **GetPasswordExpirationDate** operation request shows how to get the password expiration date for an email account.</span></span> 
  
### <a name="code"></a><span data-ttu-id="e4779-123">Код</span><span class="sxs-lookup"><span data-stu-id="e4779-123">Code</span></span>

```XML
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Header>
  </soap:Header>
  <soap:Body>
    <tns:GetPasswordExpirationDate>
      <tns:MailboxSmtpAddress>user1@DTZMZX-dom.extest.microsoft.com</tns:MailboxSmtpAddress>
    </tns:GetPasswordExpirationDate>
  </soap:Body>
</soap:Envelope>

```

### <a name="request-elements"></a><span data-ttu-id="e4779-124">Элементы Request</span><span class="sxs-lookup"><span data-stu-id="e4779-124">Request elements</span></span>

<span data-ttu-id="e4779-125">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="e4779-125">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="e4779-126">GetPasswordExpirationDate</span><span class="sxs-lookup"><span data-stu-id="e4779-126">GetPasswordExpirationDate</span></span>](getpasswordexpirationdate.md)
    
- [<span data-ttu-id="e4779-127">маилбокссмтпаддресс</span><span class="sxs-lookup"><span data-stu-id="e4779-127">MailboxSmtpAddress</span></span>](mailboxsmtpaddress.md)
    
## <a name="successful-getpasswordexpirationdate-operation-response"></a><span data-ttu-id="e4779-128">Успешный отклик операции GetPasswordExpirationDate</span><span class="sxs-lookup"><span data-stu-id="e4779-128">Successful GetPasswordExpirationDate operation response</span></span>

<span data-ttu-id="e4779-129">В отклике используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="e4779-129">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="e4779-130">жетпассвордекспиратиондатереспонсе</span><span class="sxs-lookup"><span data-stu-id="e4779-130">GetPasswordExpirationDateResponse</span></span>](getpasswordexpirationdateresponse.md)
    
- [<span data-ttu-id="e4779-131">пассвордекспиратиондате</span><span class="sxs-lookup"><span data-stu-id="e4779-131">PasswordExpirationDate</span></span>](passwordexpirationdate.md)
    

