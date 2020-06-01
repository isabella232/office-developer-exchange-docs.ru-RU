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
ms.openlocfilehash: 4184092cf98161e4c2f74446cef5439722ae71a1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457895"
---
# <a name="getpasswordexpirationdate-operation"></a><span data-ttu-id="611bf-103">Операция GetPasswordExpirationDate</span><span class="sxs-lookup"><span data-stu-id="611bf-103">GetPasswordExpirationDate operation</span></span>

<span data-ttu-id="611bf-104">Операция **GetPasswordExpirationDate** предоставляет срок действия пароля учетной записи электронной почты для текущего пользователя.</span><span class="sxs-lookup"><span data-stu-id="611bf-104">The **GetPasswordExpirationDate** operation provides the email account password expiration date for the current user.</span></span> 
  
<span data-ttu-id="611bf-105">Эта операция появилась в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="611bf-105">This operation was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="getpasswordexpirationdate-operation-soap-headers"></a><span data-ttu-id="611bf-106">Заголовки SOAP операции GetPasswordExpirationDate</span><span class="sxs-lookup"><span data-stu-id="611bf-106">GetPasswordExpirationDate operation SOAP headers</span></span>

<span data-ttu-id="611bf-107">Операция **GetPasswordExpirationDate** может использовать заголовки SOAP, указанные в приведенной ниже таблице.</span><span class="sxs-lookup"><span data-stu-id="611bf-107">The **GetPasswordExpirationDate** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="611bf-108">**Header**</span><span class="sxs-lookup"><span data-stu-id="611bf-108">**Header**</span></span>|<span data-ttu-id="611bf-109">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="611bf-109">**Element**</span></span>|<span data-ttu-id="611bf-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="611bf-110">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="611bf-111">**маилбокскултуре**</span><span class="sxs-lookup"><span data-stu-id="611bf-111">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="611bf-112">маилбокскултуре</span><span class="sxs-lookup"><span data-stu-id="611bf-112">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="611bf-113">Определяет язык и региональные параметры, определенные в документе RFC 3066 "Теги для идентификации языков", которые будут использоваться для доступа к почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="611bf-113">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="611bf-114">Это относится к запросу.</span><span class="sxs-lookup"><span data-stu-id="611bf-114">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="611bf-115">**рекуестверсион**</span><span class="sxs-lookup"><span data-stu-id="611bf-115">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="611bf-116">рекуестсерверверсион</span><span class="sxs-lookup"><span data-stu-id="611bf-116">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="611bf-117">Определяет схему запроса операции.</span><span class="sxs-lookup"><span data-stu-id="611bf-117">Identifies the schema for the operation request.</span></span> <span data-ttu-id="611bf-118">Это относится к запросу.</span><span class="sxs-lookup"><span data-stu-id="611bf-118">This is applicable to a request.</span></span> <span data-ttu-id="611bf-119">Это относится к запросу.</span><span class="sxs-lookup"><span data-stu-id="611bf-119">This is applicable to a request.</span></span>  <br/> |
   
## <a name="getpasswordexpirationdate-operation-request-example"></a><span data-ttu-id="611bf-120">Пример запроса операции GetPasswordExpirationDate</span><span class="sxs-lookup"><span data-stu-id="611bf-120">GetPasswordExpirationDate operation request example</span></span>

### <a name="description"></a><span data-ttu-id="611bf-121">Описание</span><span class="sxs-lookup"><span data-stu-id="611bf-121">Description</span></span>

<span data-ttu-id="611bf-122">В приведенном ниже примере запроса операции **GetPasswordExpirationDate** показано, как получить срок действия пароля для учетной записи электронной почты.</span><span class="sxs-lookup"><span data-stu-id="611bf-122">The following example of a **GetPasswordExpirationDate** operation request shows how to get the password expiration date for an email account.</span></span> 
  
### <a name="code"></a><span data-ttu-id="611bf-123">Код</span><span class="sxs-lookup"><span data-stu-id="611bf-123">Code</span></span>

```XML
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Header>
  </soap:Header>
  <soap:Body>
    <tns:GetPasswordExpirationDate>
      <tns:MailboxSmtpAddress>user1@DTZMZX-dom.extest.microsoft.com</tns:MailboxSmtpAddress>
    </tns:GetPasswordExpirationDate>
  </soap:Body>
</soap:Envelope>

```

### <a name="request-elements"></a><span data-ttu-id="611bf-124">Элементы Request</span><span class="sxs-lookup"><span data-stu-id="611bf-124">Request elements</span></span>

<span data-ttu-id="611bf-125">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="611bf-125">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="611bf-126">GetPasswordExpirationDate</span><span class="sxs-lookup"><span data-stu-id="611bf-126">GetPasswordExpirationDate</span></span>](getpasswordexpirationdate.md)
    
- [<span data-ttu-id="611bf-127">маилбокссмтпаддресс</span><span class="sxs-lookup"><span data-stu-id="611bf-127">MailboxSmtpAddress</span></span>](mailboxsmtpaddress.md)
    
## <a name="successful-getpasswordexpirationdate-operation-response"></a><span data-ttu-id="611bf-128">Успешный отклик операции GetPasswordExpirationDate</span><span class="sxs-lookup"><span data-stu-id="611bf-128">Successful GetPasswordExpirationDate operation response</span></span>

<span data-ttu-id="611bf-129">В отклике используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="611bf-129">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="611bf-130">жетпассвордекспиратиондатереспонсе</span><span class="sxs-lookup"><span data-stu-id="611bf-130">GetPasswordExpirationDateResponse</span></span>](getpasswordexpirationdateresponse.md)
    
- [<span data-ttu-id="611bf-131">пассвордекспиратиондате</span><span class="sxs-lookup"><span data-stu-id="611bf-131">PasswordExpirationDate</span></span>](passwordexpirationdate.md)
    

