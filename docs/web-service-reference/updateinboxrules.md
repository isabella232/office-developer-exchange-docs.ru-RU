---
title: UpdateInboxRules
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateInboxRules
api_type:
- schema
ms.assetid: d220064f-ff4d-4537-8077-adf94f2cbdbd
description: Элемент UpdateInboxRules определяет запрос на обновление правил папкиВходящиепочтового ящика в хранилище сервера.
ms.openlocfilehash: 73af3efcbf4320604576b724acf18530b8b86b26
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840342"
---
# <a name="updateinboxrules"></a><span data-ttu-id="c7d6d-103">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="c7d6d-103">UpdateInboxRules</span></span>

<span data-ttu-id="c7d6d-104">Информация, содержащаяся в этом документе, может относиться к функциям и продуктам предварительной версии и может претерпеть значительные изменения до окончательного коммерческого выпуска. Настоящий документ предоставляется "как есть" и служит только для информационных целей. Корпорация Майкрософт не предоставляет никаких гарантий, явных или подразумеваемых, в связи с этим документом Элемент **UpdateInboxRules** определяет запрос на обновление правил папки "Входящие" почтового ящика в хранилище сервера.</span><span class="sxs-lookup"><span data-stu-id="c7d6d-104">The **UpdateInboxRules** element defines a request to update the Inbox rules in a mailbox in the server store.</span></span> 
  
```XML
<UpdateInboxRules>
   <MailboxSmtpAddress/>
   <RemoveOutlookRuleBlob/>
   <Operations/>
</UpdateInboxRules>
```

 <span data-ttu-id="c7d6d-105">**UpdateInboxRulesRequestType**</span><span class="sxs-lookup"><span data-stu-id="c7d6d-105">**UpdateInboxRulesRequestType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c7d6d-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="c7d6d-106">Attributes and elements</span></span>

<span data-ttu-id="c7d6d-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="c7d6d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c7d6d-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="c7d6d-108">Attributes</span></span>

<span data-ttu-id="c7d6d-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="c7d6d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c7d6d-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="c7d6d-110">Child elements</span></span>

|<span data-ttu-id="c7d6d-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c7d6d-111">**Element**</span></span>|<span data-ttu-id="c7d6d-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c7d6d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c7d6d-113">MailboxSmtpAddress</span><span class="sxs-lookup"><span data-stu-id="c7d6d-113">MailboxSmtpAddress</span></span>](mailboxsmtpaddress.md) <br/> |<span data-ttu-id="c7d6d-114">Представляет SMTP-адрес пользователя, чьи правила папки «Входящие», для создания, изменения или удаления.</span><span class="sxs-lookup"><span data-stu-id="c7d6d-114">Represents the SMTP address of the user whose Inbox rules are to be created, modified, or deleted.</span></span>  <br/> |
|[<span data-ttu-id="c7d6d-115">RemoveOutlookRuleBlob</span><span class="sxs-lookup"><span data-stu-id="c7d6d-115">RemoveOutlookRuleBlob</span></span>](removeoutlookruleblob.md) <br/> |<span data-ttu-id="c7d6d-116">Указывает, следует ли удалять больших двоичных объектов Microsoft Outlook правило.</span><span class="sxs-lookup"><span data-stu-id="c7d6d-116">Indicates whether to remove the Microsoft Outlook rule blob.</span></span>  <br/> |
|[<span data-ttu-id="c7d6d-117">Операции</span><span class="sxs-lookup"><span data-stu-id="c7d6d-117">Operations</span></span>](operations.md) <br/> |<span data-ttu-id="c7d6d-118">Содержит набор операций правила, которые могут выполняться в папке "Входящие".</span><span class="sxs-lookup"><span data-stu-id="c7d6d-118">Contains an array of rule operations that can be performed on an Inbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c7d6d-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="c7d6d-119">Parent elements</span></span>

<span data-ttu-id="c7d6d-120">Нет.</span><span class="sxs-lookup"><span data-stu-id="c7d6d-120">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="c7d6d-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="c7d6d-121">Text value</span></span>

<span data-ttu-id="c7d6d-122">Нет.</span><span class="sxs-lookup"><span data-stu-id="c7d6d-122">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c7d6d-123">Замечания</span><span class="sxs-lookup"><span data-stu-id="c7d6d-123">Remarks</span></span>

<span data-ttu-id="c7d6d-124">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="c7d6d-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c7d6d-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="c7d6d-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c7d6d-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="c7d6d-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c7d6d-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="c7d6d-127">Schema Name</span></span>  <br/> |<span data-ttu-id="c7d6d-128">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="c7d6d-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="c7d6d-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="c7d6d-129">Validation File</span></span>  <br/> |<span data-ttu-id="c7d6d-130">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="c7d6d-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c7d6d-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="c7d6d-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="c7d6d-132">True</span><span class="sxs-lookup"><span data-stu-id="c7d6d-132">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c7d6d-133">См. также</span><span class="sxs-lookup"><span data-stu-id="c7d6d-133">See also</span></span>



[<span data-ttu-id="c7d6d-134">Операция UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="c7d6d-134">UpdateInboxRules operation</span></span>](updateinboxrules-operation.md)


- [<span data-ttu-id="c7d6d-135">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="c7d6d-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

