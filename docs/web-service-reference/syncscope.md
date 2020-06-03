---
title: синкскопе
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SyncScope
api_type:
- schema
ms.assetid: e0ca231f-0374-4844-8d4c-ada8da167920
description: Элемент Синкскопе указывает, будут ли в ответе синхронизации возвращаться только элементы, связанные с папкой, а также сведения о них.
ms.openlocfilehash: 5ede26204c823a452189222075c784f24e98d188
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463036"
---
# <a name="syncscope"></a><span data-ttu-id="ecadb-103">синкскопе</span><span class="sxs-lookup"><span data-stu-id="ecadb-103">SyncScope</span></span>

<span data-ttu-id="ecadb-104">Элемент **синкскопе** указывает, будут ли в ответе синхронизации возвращаться только элементы, связанные с папкой, а также сведения о них.</span><span class="sxs-lookup"><span data-stu-id="ecadb-104">The **SyncScope** element specifies whether just items or items and folder associated information are returned in a synchronization response.</span></span> 
  
```xml
<SyncScope>NormalItems or NormalAndAssociatedItems</SyncScope>
```

 <span data-ttu-id="ecadb-105">**синкфолдеритемсскопетипе**</span><span class="sxs-lookup"><span data-stu-id="ecadb-105">**SyncFolderItemsScopeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ecadb-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="ecadb-106">Attributes and elements</span></span>

<span data-ttu-id="ecadb-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="ecadb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ecadb-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="ecadb-108">Attributes</span></span>

<span data-ttu-id="ecadb-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="ecadb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ecadb-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="ecadb-110">Child elements</span></span>

<span data-ttu-id="ecadb-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="ecadb-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ecadb-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="ecadb-112">Parent elements</span></span>

|<span data-ttu-id="ecadb-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ecadb-113">**Element**</span></span>|<span data-ttu-id="ecadb-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ecadb-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ecadb-115">SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="ecadb-115">SyncFolderItems</span></span>](syncfolderitems.md) <br/> |<span data-ttu-id="ecadb-116">Элемент, определяющий запрос на синхронизацию элементов в папке хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="ecadb-116">The element that defines a request to synchronize items in an Exchange store folder.</span></span>  <br/> <span data-ttu-id="ecadb-117">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="ecadb-117">The following is the XPath expression to this element:</span></span>  <br/> <span data-ttu-id="ecadb-118">/синкфолдеритемс</span><span class="sxs-lookup"><span data-stu-id="ecadb-118">/SyncFolderItems</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ecadb-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="ecadb-119">Text value</span></span>

<span data-ttu-id="ecadb-120">В следующей таблице приведены возможные значения для элемента **синкскопе** .</span><span class="sxs-lookup"><span data-stu-id="ecadb-120">The following table lists the possible values for the **SyncScope** element.</span></span> 
  
<span data-ttu-id="ecadb-121">**Значения элементов Синкскопе**</span><span class="sxs-lookup"><span data-stu-id="ecadb-121">**SyncScope element values**</span></span>

|<span data-ttu-id="ecadb-122">**Значение**</span><span class="sxs-lookup"><span data-stu-id="ecadb-122">**Value**</span></span>|<span data-ttu-id="ecadb-123">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ecadb-123">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ecadb-124">нормалитемс</span><span class="sxs-lookup"><span data-stu-id="ecadb-124">NormalItems</span></span>  <br/> |<span data-ttu-id="ecadb-125">Указывает, что в отклике синхронизации возвращаются только элементы в папке.</span><span class="sxs-lookup"><span data-stu-id="ecadb-125">Specifies that only items in the folder are returned in a synchronization response.</span></span>  <br/> |
|<span data-ttu-id="ecadb-126">нормаландассоЦиатедитемс</span><span class="sxs-lookup"><span data-stu-id="ecadb-126">NormalAndAssociatedItems</span></span>  <br/> |<span data-ttu-id="ecadb-127">Указывает, что оба элемента в папке и связанных с ней сведениями возвращаются в ответе синхронизации.</span><span class="sxs-lookup"><span data-stu-id="ecadb-127">Specifies that both items in the folder and folder associated information are returned in a synchronization response.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ecadb-128">Примечания</span><span class="sxs-lookup"><span data-stu-id="ecadb-128">Remarks</span></span>

<span data-ttu-id="ecadb-129">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера, на котором работает сервер Microsoft Exchange с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="ecadb-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ecadb-130">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="ecadb-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ecadb-131">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="ecadb-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ecadb-132">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="ecadb-132">Schema Name</span></span>  <br/> |<span data-ttu-id="ecadb-133">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="ecadb-133">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ecadb-134">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="ecadb-134">Validation File</span></span>  <br/> |<span data-ttu-id="ecadb-135">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="ecadb-135">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ecadb-136">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="ecadb-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="ecadb-137">False</span><span class="sxs-lookup"><span data-stu-id="ecadb-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ecadb-138">См. также</span><span class="sxs-lookup"><span data-stu-id="ecadb-138">See also</span></span>



[<span data-ttu-id="ecadb-139">Операция SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="ecadb-139">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)


- [<span data-ttu-id="ecadb-140">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="ecadb-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

