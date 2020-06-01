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
ms.openlocfilehash: d604604d582d28c07eaa75d3239082d1b6735e65
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456362"
---
# <a name="updateinboxrules"></a><span data-ttu-id="aceaa-103">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="aceaa-103">UpdateInboxRules</span></span>

<span data-ttu-id="aceaa-104">Информация, содержащаяся в этом документе, может относиться к функциям и продуктам предварительной версии и может претерпеть значительные изменения до окончательного коммерческого выпуска. Настоящий документ предоставляется "как есть" и служит только для информационных целей. Корпорация Майкрософт не предоставляет никаких гарантий, явных или подразумеваемых, в связи с этим документом Элемент **UpdateInboxRules** определяет запрос на обновление правил папки "Входящие" почтового ящика в хранилище сервера.</span><span class="sxs-lookup"><span data-stu-id="aceaa-104">The **UpdateInboxRules** element defines a request to update the Inbox rules in a mailbox in the server store.</span></span> 
  
```XML
<UpdateInboxRules>
   <MailboxSmtpAddress/>
   <RemoveOutlookRuleBlob/>
   <Operations/>
</UpdateInboxRules>
```

 <span data-ttu-id="aceaa-105">**упдатеинбоксрулесрекуесттипе**</span><span class="sxs-lookup"><span data-stu-id="aceaa-105">**UpdateInboxRulesRequestType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="aceaa-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="aceaa-106">Attributes and elements</span></span>

<span data-ttu-id="aceaa-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="aceaa-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="aceaa-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="aceaa-108">Attributes</span></span>

<span data-ttu-id="aceaa-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="aceaa-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="aceaa-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="aceaa-110">Child elements</span></span>

|<span data-ttu-id="aceaa-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="aceaa-111">**Element**</span></span>|<span data-ttu-id="aceaa-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="aceaa-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aceaa-113">маилбокссмтпаддресс</span><span class="sxs-lookup"><span data-stu-id="aceaa-113">MailboxSmtpAddress</span></span>](mailboxsmtpaddress.md) <br/> |<span data-ttu-id="aceaa-114">Представляет SMTP-адрес пользователя, чьи правила папки «Входящие», для создания, изменения или удаления.</span><span class="sxs-lookup"><span data-stu-id="aceaa-114">Represents the SMTP address of the user whose Inbox rules are to be created, modified, or deleted.</span></span>  <br/> |
|[<span data-ttu-id="aceaa-115">ремовеаутлукрулеблоб</span><span class="sxs-lookup"><span data-stu-id="aceaa-115">RemoveOutlookRuleBlob</span></span>](removeoutlookruleblob.md) <br/> |<span data-ttu-id="aceaa-116">Указывает, следует ли удалять больших двоичных объектов Microsoft Outlook правило.</span><span class="sxs-lookup"><span data-stu-id="aceaa-116">Indicates whether to remove the Microsoft Outlook rule blob.</span></span>  <br/> |
|[<span data-ttu-id="aceaa-117">Операции</span><span class="sxs-lookup"><span data-stu-id="aceaa-117">Operations</span></span>](operations.md) <br/> |<span data-ttu-id="aceaa-118">Содержит набор операций правила, которые могут выполняться в папке "Входящие".</span><span class="sxs-lookup"><span data-stu-id="aceaa-118">Contains an array of rule operations that can be performed on an Inbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="aceaa-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="aceaa-119">Parent elements</span></span>

<span data-ttu-id="aceaa-120">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="aceaa-120">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="aceaa-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="aceaa-121">Text value</span></span>

<span data-ttu-id="aceaa-122">Нет.</span><span class="sxs-lookup"><span data-stu-id="aceaa-122">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="aceaa-123">Примечания</span><span class="sxs-lookup"><span data-stu-id="aceaa-123">Remarks</span></span>

<span data-ttu-id="aceaa-124">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="aceaa-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="aceaa-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="aceaa-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="aceaa-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="aceaa-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="aceaa-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="aceaa-127">Schema Name</span></span>  <br/> |<span data-ttu-id="aceaa-128">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="aceaa-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="aceaa-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="aceaa-129">Validation File</span></span>  <br/> |<span data-ttu-id="aceaa-130">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="aceaa-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="aceaa-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="aceaa-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="aceaa-132">True</span><span class="sxs-lookup"><span data-stu-id="aceaa-132">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="aceaa-133">См. также</span><span class="sxs-lookup"><span data-stu-id="aceaa-133">See also</span></span>



[<span data-ttu-id="aceaa-134">Операция UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="aceaa-134">UpdateInboxRules operation</span></span>](updateinboxrules-operation.md)


- [<span data-ttu-id="aceaa-135">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="aceaa-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

