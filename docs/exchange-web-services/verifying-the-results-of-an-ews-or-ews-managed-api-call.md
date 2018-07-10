---
title: Проверка результатов вызова веб-служб Exchange или управляемый API EWS
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: 78a1741c-1bbe-4cb4-9331-9d6d3171fc11
description: Узнайте, как проверка результатов вызовов веб-служб Exchange или управляемый API веб-служб Exchange.
ms.openlocfilehash: 077dd923710a1a7f5cad4c822cbbd58ab3603661
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761251"
---
# <a name="verifying-the-results-of-an-ews-or-ews-managed-api-call"></a><span data-ttu-id="4ffbf-103">Проверка результатов вызова веб-служб Exchange или управляемый API EWS</span><span class="sxs-lookup"><span data-stu-id="4ffbf-103">Verifying the results of an EWS or EWS Managed API call</span></span>

<span data-ttu-id="4ffbf-104">Узнайте, как проверка результатов вызовов веб-служб Exchange или управляемый API веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="4ffbf-104">Learn how to verify the results of your EWS or EWS Managed API calls.</span></span>
  
<span data-ttu-id="4ffbf-105">При действия не работает корректно, будет полезным взглянуть, что происходит изучив запросов SOAP, которые приложение передает по сети и ответы, сервер отправляет обратно.</span><span class="sxs-lookup"><span data-stu-id="4ffbf-105">When things aren't working correctly, it helps to see what's going on by examining the SOAP requests that your application is sending over the network and the responses that the server is sending back.</span></span> <span data-ttu-id="4ffbf-106">[Средства и ресурсы, необходимые для устранения неполадок приложений веб-служб Exchange](tools-and-resources-for-troubleshooting-ews-applications-for-exchange.md) статье содержатся ссылки на средства для регистрации и просмотра этих запросов SOAP.</span><span class="sxs-lookup"><span data-stu-id="4ffbf-106">The [tools and resources for troubleshooting EWS applications](tools-and-resources-for-troubleshooting-ews-applications-for-exchange.md) article includes links to tools to help capture and view those SOAP requests.</span></span> <span data-ttu-id="4ffbf-107">После создания запросов и ответов, как проверяется правильно обработать запрос отправки на сервере?</span><span class="sxs-lookup"><span data-stu-id="4ffbf-107">After you've got the requests and the responses, how do you verify that the request you sent to the server was processed correctly?</span></span> <span data-ttu-id="4ffbf-108">Познакомьтесь.</span><span class="sxs-lookup"><span data-stu-id="4ffbf-108">Read on to find out.</span></span> 
  
<span data-ttu-id="4ffbf-109">При отправке запросов веб-служб Exchange, которому необходимо запустить программу вашей проверки, установив атрибут **ResponseClass** для каждого сообщения ответа в ответе.</span><span class="sxs-lookup"><span data-stu-id="4ffbf-109">If you're sending EWS requests, you're going to start your verification by checking the **ResponseClass** attribute for each response message in the response.</span></span> <span data-ttu-id="4ffbf-110">Который будет указано, будет ли операция успешно завершена для каждого элемента.</span><span class="sxs-lookup"><span data-stu-id="4ffbf-110">That will tell you whether the operation completed successfully on each item.</span></span> 
  
<span data-ttu-id="4ffbf-111">В зависимости от объекта, что метод вызова, если вы используете управляемый API EWS для отправки запросов, можно выполнить некоторые проверки, с помощью объектов ответа.</span><span class="sxs-lookup"><span data-stu-id="4ffbf-111">Depending on the object that your method is calling, if you're using the EWS Managed API to send requests, you can do some verification using the response objects.</span></span> <span data-ttu-id="4ffbf-112">Однако поскольку ответ SOAP содержит подмножеством возможностей, включенных в объекты ответа управляемый API веб-служб Exchange, можно рассмотреть в ответе SOAP.</span><span class="sxs-lookup"><span data-stu-id="4ffbf-112">But because the SOAP response contains a superset of what's included in the EWS Managed API response objects, you might want to look at the SOAP response as well.</span></span> <span data-ttu-id="4ffbf-113">Так как ответ SOAP часто может содержать больше сведений, чем объекты ответа управляемый API веб-служб Exchange, начните проверить с ответа SOAP.</span><span class="sxs-lookup"><span data-stu-id="4ffbf-113">Because the SOAP response can often contain more information than the EWS Managed API response objects, start your verification with the SOAP response.</span></span>
  
## <a name="verifying-the-results-of-a-soap-response"></a><span data-ttu-id="4ffbf-114">Проверка результатов ответа SOAP</span><span class="sxs-lookup"><span data-stu-id="4ffbf-114">Verifying the results of a SOAP response</span></span>
<span data-ttu-id="4ffbf-115"><a name="bk_verifysoap"> </a></span><span class="sxs-lookup"><span data-stu-id="4ffbf-115"></span></span>

<span data-ttu-id="4ffbf-116">При получении ответа SOAP в первую очередь необходимо рассмотреть является атрибутом **ResponseClass** .</span><span class="sxs-lookup"><span data-stu-id="4ffbf-116">When you receive a SOAP response, the first thing to look at is the **ResponseClass** attribute.</span></span> <span data-ttu-id="4ffbf-117">Этот атрибут включается в каждый экземпляр **ResponseMessageType** в элементе [ResponseMessages](http://msdn.microsoft.com/library/2071bed8-ea66-4627-aa4f-a1d9a025cf3d%28Office.15%29.aspx) , как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="4ffbf-117">This attribute is included in each **ResponseMessageType** instance in the [ResponseMessages](http://msdn.microsoft.com/library/2071bed8-ea66-4627-aa4f-a1d9a025cf3d%28Office.15%29.aspx) element, as shown in the following example.</span></span> 
  
```XML
<s:Body>
      <m:GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
        <m:ResponseMessages>
          <m:GetItemResponseMessage ResponseClass="Success">
          …
```

<span data-ttu-id="4ffbf-118">Ответ SOAP может содержать несколько сообщений ответа в один ответ SOAP, важно проверить каждого сообщения ответа по отдельности.</span><span class="sxs-lookup"><span data-stu-id="4ffbf-118">Because a SOAP response might contain multiple response messages in a single SOAP response, it's important to check each response message individually.</span></span>
  
<span data-ttu-id="4ffbf-119">Если вы работаете с операции, которая включает в себя **ResponseClass** как часть ответа операции следующим образом, может возникнуть желание только проверка **ResponseClass** операции.</span><span class="sxs-lookup"><span data-stu-id="4ffbf-119">If you're working with an operation that includes a **ResponseClass** as part of the operation response, like the following, you might be tempted to only check the **ResponseClass** of the operation.</span></span> 
  
```XML
<soap:Body>
  <m:AddDelegateResponse xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                         ResponseClass="Success"
                         xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
  …

```

<span data-ttu-id="4ffbf-120">Тем не менее состояние операции только отражает фигуры верхнего уровня ответа и не зависит от состояния всех ответов отдельных сообщений.</span><span class="sxs-lookup"><span data-stu-id="4ffbf-120">However, the operation status only reflects the shape of the top-level response and does not reflect the status of all the individual message responses.</span></span> <span data-ttu-id="4ffbf-121">В следующем примере [AddDelegateResponse](http://msdn.microsoft.com/library/d7e6bebb-5dbf-43c1-aacf-4b3ca6a7c429%28Office.15%29.aspx) операция имеет **ResponseClass** **Успех**, но базовый элемент [DelegateUserResponseMessageType](http://msdn.microsoft.com/library/3dc9552c-1e2d-40ac-a137-827883c2bb88%28Office.15%29.aspx) имеет значение **ResponseClass** **об ошибках**.</span><span class="sxs-lookup"><span data-stu-id="4ffbf-121">In the following example, the [AddDelegateResponse](http://msdn.microsoft.com/library/d7e6bebb-5dbf-43c1-aacf-4b3ca6a7c429%28Office.15%29.aspx) operation has a **ResponseClass** of **Success**, but the underlying [DelegateUserResponseMessageType](http://msdn.microsoft.com/library/3dc9552c-1e2d-40ac-a137-827883c2bb88%28Office.15%29.aspx) element has a **ResponseClass** value of **Error**.</span></span>
  
```XML
<soap:Body>
  <m:AddDelegateResponse xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                         ResponseClass="Success"
                         xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
    <m:ResponseCode>NoError</m:ResponseCode>
    <m:ResponseMessages>
      <m:DelegateUserResponseMessageType ResponseClass="Error">
        <m:MessageText>The user is already a delegate for the mailbox.</m:MessageText>
        <m:ResponseCode>ErrorDelegateAlreadyExists</m:ResponseCode>
        <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
      </m:DelegateUserResponseMessageType>
    </m:ResponseMessages>
  </m:AddDelegateResponse>
</soap:Body>
```

<span data-ttu-id="4ffbf-122">Поэтому для ответы SOAP веб-служб Exchange, нельзя полагаться на **ResponseClass** операции - необходимо рассмотреть **ResponseClass** каждого сообщения ответа, чтобы определить, является ли все ошибки обработки элементов при выполнении операции.</span><span class="sxs-lookup"><span data-stu-id="4ffbf-122">So for SOAP EWS responses, you can't rely on the **ResponseClass** of the operation - you have to look at the **ResponseClass** of each response message to determine whether the operation encountered any errors processing the items.</span></span> 
  
### <a name="verifying-success"></a><span data-ttu-id="4ffbf-123">Проверка успешности</span><span class="sxs-lookup"><span data-stu-id="4ffbf-123">Verifying success</span></span>

<span data-ttu-id="4ffbf-124">Если каждый атрибут **ResponseClass** для каждого **ResponseMessage** атрибута задано значение **успешно**, операция выполнена успешно, для всех элементов, и можно перейти к следующей задаче.</span><span class="sxs-lookup"><span data-stu-id="4ffbf-124">If each **ResponseClass** attribute for each **ResponseMessage** attribute is set to **Success**, the operation completed successfully on all the items, and you can move on to your next task.</span></span>
  
<span data-ttu-id="4ffbf-125">В следующем примере показано успешного ответа на запрос операции [GetItem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) для получения отдельных элементов.</span><span class="sxs-lookup"><span data-stu-id="4ffbf-125">The following example shows a successful response to a [GetItem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) operation request to retrieve a single item.</span></span> <span data-ttu-id="4ffbf-126">Обратите внимание, что если **ResponseClass** **Успех**, связанный [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) всегда имеет значение **NoError**.</span><span class="sxs-lookup"><span data-stu-id="4ffbf-126">Note that when the **ResponseClass** is set to **Success**, the associated [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) is always set to **NoError**.</span></span>
  
```XML
<s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
             xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <m:GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
        <m:ResponseMessages>
          <m:GetItemResponseMessage ResponseClass="Success">
            <m:ResponseCode>NoError</m:ResponseCode>
            <m:Items>
              <t:Message>
                <t:ItemId Id="Er5bAAA=" 
                          ChangeKey="CQAAABYAAAD32nSTjepyT63rYH17n9THAAAhE0/M" />
                <t:Subject>Dinner Party</t:Subject>
              </t:Message>
            </m:Items>
          </m:GetItemResponseMessage>
        </m:ResponseMessages>
      </m:GetItemResponse>
    </s:Body>
```

<span data-ttu-id="4ffbf-127">Ниже приведен успешного ответа на запрос операции **GetItem** для получения нескольких элементов.</span><span class="sxs-lookup"><span data-stu-id="4ffbf-127">The following is a successful response to a **GetItem** operation request to retrieve multiple items.</span></span> <span data-ttu-id="4ffbf-128">Все элементы [GetItemResponseMessage](http://msdn.microsoft.com/library/cc583723-54d1-4a17-8c1f-6586f70fdefd%28Office.15%29.aspx) имеет **ResponseClass** **успеха**.</span><span class="sxs-lookup"><span data-stu-id="4ffbf-128">Each of the [GetItemResponseMessage](http://msdn.microsoft.com/library/cc583723-54d1-4a17-8c1f-6586f70fdefd%28Office.15%29.aspx) elements has a **ResponseClass** of **Success**.</span></span>
  
```XML
<s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
             xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <m:GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                     xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
    <m:ResponseMessages>
      <m:GetItemResponseMessage ResponseClass="Success">
        <m:ResponseCode>NoError</m:ResponseCode>
        <m:Items>
          <t:Message>
            <t:ItemId Id="Er5bAAA=" 
                      ChangeKey="CQAAABYAAAD32nSTjepyT63rYH17n9THAAAhE0/M" /
            <t:Subject>Dinner Party</t:Subject>
          </t:Message>
        </m:Items>
      </m:GetItemResponseMessage>
      <m:GetItemResponseMessage ResponseClass="Success">
        <m:ResponseCode>NoError</m:ResponseCode>
        <m:Items>
          <t:Message>
            <t:ItemId Id="3c66AAA="
                      ChangeKey="CQAAABYAAAD32nSTjepyT63rYH17n9THAAAc3kqm" />
            <t:Subject>Company Soccer Team</t:Subject>
          </t:Message>
        </m:Items>
      </m:GetItemResponseMessage>
    </m:ResponseMessages>
  </m:GetItemResponse>
</s:Body>
```

### <a name="handling-errors-and-warnings"></a><span data-ttu-id="4ffbf-129">Обработка ошибок и предупреждений</span><span class="sxs-lookup"><span data-stu-id="4ffbf-129">Handling errors and warnings</span></span>

<span data-ttu-id="4ffbf-130">Когда был получен ответ, атрибут **ResponseClass** задано значение **Ошибка**, операция не завершена успешно на один или несколько элементов.</span><span class="sxs-lookup"><span data-stu-id="4ffbf-130">When you receive a response and the **ResponseClass** attribute is set to **Error**, the operation did not complete successfully on one or more items.</span></span> <span data-ttu-id="4ffbf-131">Устраните проблему и повторите попытку запроса или частью вашего запроса с отказом.</span><span class="sxs-lookup"><span data-stu-id="4ffbf-131">Correct the issue and retry your request, or the part of your request that failed.</span></span> <span data-ttu-id="4ffbf-132">Значение атрибута **ResponseClass** значения **Предупреждение** только возвращенные операцией [ResolveNames](http://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) и указывает, что сущность не удалось разрешить уникальное удостоверение.</span><span class="sxs-lookup"><span data-stu-id="4ffbf-132">A **ResponseClass** attribute value of **Warning** value is only returned by the [ResolveNames](http://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) operation, and indicates that the entity could not be resolved to a unique identity.</span></span> <span data-ttu-id="4ffbf-133">Его можно пропустить для всех других операций.</span><span class="sxs-lookup"><span data-stu-id="4ffbf-133">You can ignore it for all other operations.</span></span> 
  
<span data-ttu-id="4ffbf-134">В следующем запросе атрибут **ResponseClass** имеет значение **ошибки**.</span><span class="sxs-lookup"><span data-stu-id="4ffbf-134">In the following response, the **ResponseClass** attribute has a value of **Error**.</span></span>
  
```XML
<m:GetItemResponseMessage ResponseClass="Error">
  <m:MessageText>Property is not valid for this object type.</m:MessageText>
  <m:ResponseCode>ErrorInvalidPropertyRequest</m:ResponseCode>
  <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
  <m:MessageXml>
    <t:FieldURI FieldURI="meeting:AssociatedCalendarItemId" />
  </m:MessageXml>
  <m:Items />
</m:GetItemResponseMessage>
```

<span data-ttu-id="4ffbf-135">В этом примере веб-служб Exchange предоставляет сведения для отладки ошибки.</span><span class="sxs-lookup"><span data-stu-id="4ffbf-135">In this example, EWS provides clues to debug the issue.</span></span> <span data-ttu-id="4ffbf-136">Если атрибут **ResponseClass** имеет значение **ошибки**, в ответ, если применимо включены следующие дополнительные элементы:</span><span class="sxs-lookup"><span data-stu-id="4ffbf-136">When the **ResponseClass** attribute has a value of **Error**, the following additional elements are included in the response when applicable:</span></span>
  
- <span data-ttu-id="4ffbf-137">[MessageText](http://msdn.microsoft.com/library/59a23bdc-0d9a-4942-8b3c-9cdb11db1ab1%28Office.15%29.aspx) — описание ошибки.</span><span class="sxs-lookup"><span data-stu-id="4ffbf-137">[MessageText](http://msdn.microsoft.com/library/59a23bdc-0d9a-4942-8b3c-9cdb11db1ab1%28Office.15%29.aspx) — Describes the error.</span></span> 
    
- <span data-ttu-id="4ffbf-138">[ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) — содержит код ошибки, который может использоваться для дополнительные ресурсы по устранению неполадок.</span><span class="sxs-lookup"><span data-stu-id="4ffbf-138">[ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) — Contains the error code, which can be used to find additional troubleshooting resources.</span></span> 
    
- <span data-ttu-id="4ffbf-139">[MessageXml](http://msdn.microsoft.com/library/bcaf9e35-d351-48f3-baad-f90c633cba8a%28Office.15%29.aspx) — определяет элементы, вызвавшей ошибку.</span><span class="sxs-lookup"><span data-stu-id="4ffbf-139">[MessageXml](http://msdn.microsoft.com/library/bcaf9e35-d351-48f3-baad-f90c633cba8a%28Office.15%29.aspx) — Identifies the elements that caused the error.</span></span> 
    
- <span data-ttu-id="4ffbf-140">[DescriptiveLinkKey](http://msdn.microsoft.com/library/f7f36749-00f3-4915-b17c-e3caa0af6e67%28Office.15%29.aspx) — неиспользуемых.</span><span class="sxs-lookup"><span data-stu-id="4ffbf-140">[DescriptiveLinkKey](http://msdn.microsoft.com/library/f7f36749-00f3-4915-b17c-e3caa0af6e67%28Office.15%29.aspx) — Unused.</span></span> 
    
<span data-ttu-id="4ffbf-141">Сведения, представленные в этих элементов можно использовать для изучения проблемы.</span><span class="sxs-lookup"><span data-stu-id="4ffbf-141">You can use the information provided in these elements to investigate your issue.</span></span> <span data-ttu-id="4ffbf-142">В предыдущем примере **MessageText** указывает, что свойство не подходит для типа объекта.</span><span class="sxs-lookup"><span data-stu-id="4ffbf-142">In the previous example, the **MessageText** indicates that the property isn't valid for the object type.</span></span> <span data-ttu-id="4ffbf-143">Запрос был получение сообщения электронной почты, но набор свойств включены **AssociatedCalendarItemId**, который допустимо только для элементов встречи.</span><span class="sxs-lookup"><span data-stu-id="4ffbf-143">The request was to get an email message, but the property set included the **AssociatedCalendarItemId**, which is only valid for appointment items.</span></span>
  
<span data-ttu-id="4ffbf-144">В следующем примере показано ошибку, которое было получено как часть пакетной операции для получения нескольких элементов электронной почты.</span><span class="sxs-lookup"><span data-stu-id="4ffbf-144">The following example shows an error that was received as part of a batched operation to get multiple email items.</span></span> <span data-ttu-id="4ffbf-145">Первый элемент был успешно извлечен, **ResponseClass** задано значение **Success**.</span><span class="sxs-lookup"><span data-stu-id="4ffbf-145">The first item was retrieved successfully and the **ResponseClass** is set to **Success**.</span></span> <span data-ttu-id="4ffbf-146">Не удалось найти второй элемент, **ResponseClass** задано значение **ошибки**.</span><span class="sxs-lookup"><span data-stu-id="4ffbf-146">The second item could not be found, and the **ResponseClass** is set to **Error**.</span></span>
  
```XML
<m:GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <m:ResponseMessages>
    <m:GetItemResponseMessage ResponseClass="Success">
      <m:ResponseCode>NoError</m:ResponseCode>
      <m:Items>
        <t:Message>
          <t:ItemId Id="Er5cAAA="
                    ChangeKey="CQAAABYAAAD32nSTjepyT63rYH17n9THAAAhE0/O" />
          <t:Subject>Business plans</t:Subject>
        </t:Message>
      </m:Items>
    </m:GetItemResponseMessage>
    <m:GetItemResponseMessage ResponseClass="Error">
      <m:MessageText>The specified object was not found in the store.</m:MessageText>
      <m:ResponseCode>ErrorItemNotFound</m:ResponseCode>
      <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
      <m:Items />
    </m:GetItemResponseMessage>
  </m:ResponseMessages>
</m:GetItemResponse>
```

<span data-ttu-id="4ffbf-147">Когда один или несколько элементов в пакетной запрос не удается обработать по запросу, возвращается сообщение об ошибке для каждого элемента, который не удалось и остальные элементы в пакете обрабатываются как ожидалось.</span><span class="sxs-lookup"><span data-stu-id="4ffbf-147">When one or more items in a batched request can't be processed as requested, an error is returned for each item that failed, and the rest of the items in the batch are processed as expected.</span></span> <span data-ttu-id="4ffbf-148">В пакетной обработке могут возникнуть ошибки при элемент был удален и таким образом не может быть отправлено, получить или обновлены, а также если элемент перемещен в другую папку, а следовательно, имеет новый идентификатор элемента.</span><span class="sxs-lookup"><span data-stu-id="4ffbf-148">Failures in batch processing can occur if the item was deleted, and therefore can't be sent, retrieved, or updated, or if the item moved to a different folder, and therefore has a new item ID.</span></span> <span data-ttu-id="4ffbf-149">Так как операция завершится для некоторых элементов и возвращает ошибку, если не удается обработать один или несколько элементов, важно проверить каждый атрибут **ResponseClass** перед переходом к следующей операции.</span><span class="sxs-lookup"><span data-stu-id="4ffbf-149">Because the operation will complete for some items and not return an error when one or more items can't be processed, it's important to check each **ResponseClass** attribute before you move on to your next operation.</span></span> 
  
<span data-ttu-id="4ffbf-150">Если сведения, предоставленные элементы ответа не помогает исправить запроса или в противном случае разблокировать вы, просмотрите [дальнейшие инструкции](#bk_nextsteps).</span><span class="sxs-lookup"><span data-stu-id="4ffbf-150">If the information provided by the response elements doesn't help you correct your request or otherwise unblock you, see [Next steps](#bk_nextsteps).</span></span>
  
## <a name="verifying-the-results-of-an-ews-managed-api-method-call"></a><span data-ttu-id="4ffbf-151">Проверка результатов для вызова метода управляемый API EWS</span><span class="sxs-lookup"><span data-stu-id="4ffbf-151">Verifying the results of an EWS Managed API method call</span></span>
<span data-ttu-id="4ffbf-152"><a name="bk_successful"> </a></span><span class="sxs-lookup"><span data-stu-id="4ffbf-152"></span></span>

<span data-ttu-id="4ffbf-153">Если вы с помощью управляемого интерфейса API веб-служб Exchange и вызов метода [ExchangeService](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) объекта, метод скорее всего возвращает объект [ServiceResponseCollection](http://msdn.microsoft.com/ru-ru/library/dd633715%28v=exchg.80%29.aspx) , который содержит коллекцию объектов [ServiceResponse](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.serviceresponse%28v=exchg.80%29.aspx) или набора объекты, производные от **ServiceResponse** объектов.</span><span class="sxs-lookup"><span data-stu-id="4ffbf-153">If you're using the EWS Managed API and calling a method on an [ExchangeService](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, your method will likely return a [ServiceResponseCollection](http://msdn.microsoft.com/ru-ru/library/dd633715%28v=exchg.80%29.aspx) object, which contains a collection of [ServiceResponse](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.serviceresponse%28v=exchg.80%29.aspx) objects, or a collection of objects derived from the **ServiceResponse** objects.</span></span> <span data-ttu-id="4ffbf-154">**ServiceResponseCollection** и включенных объектов **ServiceResponse** содержат информацию о результатов вызова метода, который можно использовать для проверки результатов.</span><span class="sxs-lookup"><span data-stu-id="4ffbf-154">The **ServiceResponseCollection** and included **ServiceResponse** objects contain information about the result of the method call, which you can use to verify your results.</span></span> 
  
<span data-ttu-id="4ffbf-155">Если вы с помощью управляемого интерфейса API веб-служб Exchange и вызов метода для объекта [элемента](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) или один из производных объектов, скорее всего метод не возвращает объект ответа для проверки успешности, но вызовет [исключение](http://msdn.microsoft.com/ru-ru/library/c18k6c59) , если метод не завершена успешно.</span><span class="sxs-lookup"><span data-stu-id="4ffbf-155">If you're using the EWS Managed API and calling a method on an [Item](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) object, or one of the derived objects, the method likely does not return a response object to check for success, but does throw an [Exception](http://msdn.microsoft.com/ru-ru/library/c18k6c59) if the method does not complete successfully.</span></span> 
  
### <a name="verifying-success"></a><span data-ttu-id="4ffbf-156">Проверка успешности</span><span class="sxs-lookup"><span data-stu-id="4ffbf-156">Verifying success</span></span>

<span data-ttu-id="4ffbf-157">Преимущество использования управляемый API EWS заключается в обеспечении общего состояния при работе с несколькими элементами в один ответ.</span><span class="sxs-lookup"><span data-stu-id="4ffbf-157">One benefit of using the EWS Managed API is that it provides an overall status when dealing with multiple items in one response.</span></span> <span data-ttu-id="4ffbf-158">Поэтому если вызывается метод возвращает **ServiceResponseCollection**, можно проверить, что свойство [OverallResult](http://msdn.microsoft.com/ru-ru/library/dd634515%28v=exchg.80%29.aspx) **ServiceResponseCollection** равен [ServiceResult.Success](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.serviceresult%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="4ffbf-158">So if the method you called returns a **ServiceResponseCollection**, you can check that the [OverallResult](http://msdn.microsoft.com/ru-ru/library/dd634515%28v=exchg.80%29.aspx) property of the **ServiceResponseCollection** is equal to [ServiceResult.Success](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.serviceresult%28v=exchg.80%29.aspx).</span></span> <span data-ttu-id="4ffbf-159">Если это так, все элементы в процессе пакетной были успешно завершена; у вас нет проверка каждого объекта **ServiceResponse** по отдельности.</span><span class="sxs-lookup"><span data-stu-id="4ffbf-159">If so, all the items in the batched process were completed successfully; you don't have to check each **ServiceResponse** object individually.</span></span> <span data-ttu-id="4ffbf-160">Если свойство **OverallResult** установлено значение **ServiceResult.Success**, необходимо [обрабатывать ошибки или предупреждения](#bk_ewsmaerrors).</span><span class="sxs-lookup"><span data-stu-id="4ffbf-160">If the **OverallResult** property is not set to **ServiceResult.Success**, you have to [handle the error or warning](#bk_ewsmaerrors).</span></span>
  
<span data-ttu-id="4ffbf-161">Метод вызова не возвращает **ServiceResponseCollection**, но возвращают объект **ServiceResponse** , необходимо проверить значение свойства **результатов** .</span><span class="sxs-lookup"><span data-stu-id="4ffbf-161">If the method you're calling does not return a **ServiceResponseCollection**, but does return a **ServiceResponse** object, you have to check the value of the **Result** property.</span></span> <span data-ttu-id="4ffbf-162">Если значение **результата** **Success**, вы знаете метод выполнен успешно.</span><span class="sxs-lookup"><span data-stu-id="4ffbf-162">If the **Result** value is set to **Success**, you know the method completed successfully.</span></span>
  
<span data-ttu-id="4ffbf-163">При вызове метода не имеет возвращаемого значения, действительно нет возможности проверки успешного выполнения с помощью управляемого интерфейса API веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="4ffbf-163">If the method you're calling has no return value, there's really no way to check for success via the EWS Managed API.</span></span> <span data-ttu-id="4ffbf-164">До тех пор, пока не исключение, можно допустить метод выполнен успешно.</span><span class="sxs-lookup"><span data-stu-id="4ffbf-164">As long as an exception is not thrown, you can assume the method completed successfully.</span></span> <span data-ttu-id="4ffbf-165">Для дополнительной проверки также можно [Проверить ответ SOAP, чтобы проверить результаты](#bk_verifysoap).</span><span class="sxs-lookup"><span data-stu-id="4ffbf-165">For additional validation, you can also [check the SOAP response to verify the results](#bk_verifysoap).</span></span>
  
### <a name="handling-errors-warnings-and-exceptions"></a><span data-ttu-id="4ffbf-166">Обработка ошибок, предупреждений и исключения</span><span class="sxs-lookup"><span data-stu-id="4ffbf-166">Handling errors, warnings, and exceptions</span></span>
<span data-ttu-id="4ffbf-167"><a name="bk_ewsmaerrors"> </a></span><span class="sxs-lookup"><span data-stu-id="4ffbf-167"></span></span>

<span data-ttu-id="4ffbf-168">Если управляемый API EWS код создает **исключение**, можно использовать значение [Exception.Message](http://msdn.microsoft.com/ru-ru/library/9btwf6wk) определить причину ошибки.</span><span class="sxs-lookup"><span data-stu-id="4ffbf-168">If your EWS Managed API code throws an **Exception**, you can use the [Exception.Message](http://msdn.microsoft.com/ru-ru/library/9btwf6wk) value to determine the source of the error.</span></span> <span data-ttu-id="4ffbf-169">Свойство **Message** содержит содержимое элемента [MessageText](http://msdn.microsoft.com/library/59a23bdc-0d9a-4942-8b3c-9cdb11db1ab1%28Office.15%29.aspx) в базовом ответа SOAP.</span><span class="sxs-lookup"><span data-stu-id="4ffbf-169">The **Message** property contains the contents of the [MessageText](http://msdn.microsoft.com/library/59a23bdc-0d9a-4942-8b3c-9cdb11db1ab1%28Office.15%29.aspx) element in the underlying SOAP response.</span></span> <span data-ttu-id="4ffbf-170">Кроме того Если исключение типа объекта [ServiceResponseException](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.serviceresponseexception%28v=exchg.80%29.aspx) , одним из наиболее распространенных исключений, вы также можете получить [код ошибки](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.serviceresponseexception.errorcode%28v=exchg.80%29.aspx) , содержащихся в элемент SOAP [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) и [ответа](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.serviceresponseexception.response%28v=exchg.80%29.aspx) свойство, которое идентифицирует связанного объекта [ServiceResponse](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.serviceresponse%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="4ffbf-170">In addition, if the exception is of type [ServiceResponseException](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.serviceresponseexception%28v=exchg.80%29.aspx) object, one of the most common exceptions, you can also retrieve the [ErrorCode](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.serviceresponseexception.errorcode%28v=exchg.80%29.aspx) contained in the underlying SOAP [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element, and the [Response](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.serviceresponseexception.response%28v=exchg.80%29.aspx) property that identifies the associated [ServiceResponse](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.serviceresponse%28v=exchg.80%29.aspx) object.</span></span> <span data-ttu-id="4ffbf-171">Приведенный ниже код показано, как для перехвата и отображение содержимого **ServiceResponseException**.</span><span class="sxs-lookup"><span data-stu-id="4ffbf-171">The following code shows how to catch and display the contents of a **ServiceResponseException**.</span></span> 
  
```cs
try
    {
         …
    }
    catch (ServiceResponseException ex)
    {
        Console.WriteLine("Error code: " + ex.ErrorCode);
        Console.WriteLine("Error message: " + ex.Message);
        Console.WriteLine("Response: " + ex.Response);
    }
```

<span data-ttu-id="4ffbf-172">Если вызывается метод возвращает **ServiceResponseCollection**, и значение свойства **OverallResult** равно **Предупреждение** или **Ошибка**, необходимо хранить выполняют цикл по каждому объекту в **ServiceResponseCollection** для Поиск ошибки.</span><span class="sxs-lookup"><span data-stu-id="4ffbf-172">If the method you called returns a **ServiceResponseCollection**, and the value of the **OverallResult** property is equal to **Warning** or **Error**, you'll have to loop through each object in the **ServiceResponseCollection** to find the error.</span></span> <span data-ttu-id="4ffbf-173">Свойство **OverallResult** имеет значение **Предупреждение** , если хотя бы один ответа у **результата** значение для **предупреждения** и всех ответов имеют их значения **результатов** , задайте значение **Success**.</span><span class="sxs-lookup"><span data-stu-id="4ffbf-173">The **OverallResult** property is set to **Warning** if at least one response has its **Result** value set to **Warning** and all other responses have their **Result** values set to **Success**.</span></span> <span data-ttu-id="4ffbf-174">Свойство **OverallResult** — это значение **ошибки** , если по крайней мере один ответа значении **результатов** **ошибки**.</span><span class="sxs-lookup"><span data-stu-id="4ffbf-174">The **OverallResult** property is set to **Error** if at least one response has its **Result** value set to **Error**.</span></span> <span data-ttu-id="4ffbf-175">Если **OverallResult** **Предупреждение** или **Ошибка**, для объектов **ServiceResponse** соответствующим образом заданы следующие свойства:</span><span class="sxs-lookup"><span data-stu-id="4ffbf-175">When the **OverallResult** is set to **Warning** or **Error**, the following properties are set on the **ServiceResponse** objects as appropriate:</span></span> 
  
- <span data-ttu-id="4ffbf-176">[Код ошибки](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.serviceresponse.errorcode%28v=exchg.80%29.aspx) — содержит код ошибки, который может использоваться для дополнительные ресурсы по устранению неполадок.</span><span class="sxs-lookup"><span data-stu-id="4ffbf-176">[ErrorCode](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.serviceresponse.errorcode%28v=exchg.80%29.aspx) — Contains the error code, which can be used to find additional troubleshooting resources.</span></span> 
    
- <span data-ttu-id="4ffbf-177">[ErrorDetails](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.serviceresponse.errordetails%28v=exchg.80%29.aspx) — содержит сведения об ошибке для некоторых **ErrorCodes**.</span><span class="sxs-lookup"><span data-stu-id="4ffbf-177">[ErrorDetails](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.serviceresponse.errordetails%28v=exchg.80%29.aspx) — Contains details about the error for some **ErrorCodes**.</span></span> <span data-ttu-id="4ffbf-178">Например при **ErrorRecurrenceHasNoOccurrence**, код ошибки **ErrorDetails** будет содержать ключи для **EffectiveStartDate** и **EffectiveEndDate**.</span><span class="sxs-lookup"><span data-stu-id="4ffbf-178">For example, when the error code is **ErrorRecurrenceHasNoOccurrence**, the **ErrorDetails** will contain keys for **EffectiveStartDate** and **EffectiveEndDate**.</span></span> 
    
- <span data-ttu-id="4ffbf-179">[Сообщение об ошибке](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.serviceresponse.errormessage%28v=exchg.80%29.aspx) , описывающее ошибку.</span><span class="sxs-lookup"><span data-stu-id="4ffbf-179">[ErrorMessage](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.serviceresponse.errormessage%28v=exchg.80%29.aspx) — Describes the error.</span></span> 
    
- <span data-ttu-id="4ffbf-180">[ErrorProperties](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.serviceresponse.errorproperties%28v=exchg.80%29.aspx) , если он доступен, определяет свойства, вызвавшей ошибку.</span><span class="sxs-lookup"><span data-stu-id="4ffbf-180">[ErrorProperties](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.serviceresponse.errorproperties%28v=exchg.80%29.aspx) — If available, identifies the properties that caused the error.</span></span> <span data-ttu-id="4ffbf-181">Например при **ErrorInvalidPropertyForOperation**код ошибки **ErrorProperties** содержит определение свойства, недопустимый для запроса.</span><span class="sxs-lookup"><span data-stu-id="4ffbf-181">For example, when the error code is **ErrorInvalidPropertyForOperation**, **ErrorProperties** contains the definition of the property that was invalid for the request.</span></span> 
    
- <span data-ttu-id="4ffbf-182">[Результат](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.serviceresponse.result%28v=exchg.80%29.aspx) — содержит **об ошибке** или **Предупреждение** при обнаружении неполадок.</span><span class="sxs-lookup"><span data-stu-id="4ffbf-182">[Result](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.serviceresponse.result%28v=exchg.80%29.aspx) — Contains **Error** or **Warning** when an issue is encountered.</span></span> 
    
<span data-ttu-id="4ffbf-183">Если сведения, предоставленные свойства **ServiceResponse** не предоставляет достаточно сведений, чтобы исправить вызова метода или разблокировать вы, просмотреть [дальнейшие действия](#bk_nextsteps) получать дополнительные сведения о значениях **код ошибки** .</span><span class="sxs-lookup"><span data-stu-id="4ffbf-183">If the information provided by the **ServiceResponse** properties doesn't provide enough information to correct your method call or unblock you, see [Next steps](#bk_nextsteps) to dig up more information on **ErrorCode** values.</span></span> 
  
## 
<span data-ttu-id="4ffbf-184"><a name="bk_nextsteps"> </a></span><span class="sxs-lookup"><span data-stu-id="4ffbf-184"></span></span>

<span data-ttu-id="4ffbf-185">Можно найти дополнительные сведения об устранении неполадок в следующих разделах:</span><span class="sxs-lookup"><span data-stu-id="4ffbf-185">You can look up additional troubleshooting information in the following topics:</span></span>
  
- <span data-ttu-id="4ffbf-186">Элемент [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="4ffbf-186">[ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element</span></span> 
    
- <span data-ttu-id="4ffbf-187">Перечисление [ServiceError](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.serviceerror%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="4ffbf-187">[ServiceError](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.serviceerror%28v=exchg.80%29.aspx) enumeration</span></span> 
    
- [<span data-ttu-id="4ffbf-188">Ошибки, связанные с свойство веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="4ffbf-188">EWS property-related errors</span></span>](ews-property-related-errors.md)
    
<span data-ttu-id="4ffbf-189">Кроме того в зависимости от того, что вы пытаетесь выполнить в вашем запросе, могут найти дополнительные полезные сведения о коде ошибки в следующих разделах:</span><span class="sxs-lookup"><span data-stu-id="4ffbf-189">In addition, depending on what you're trying to accomplish in your request, you might find additional helpful information about the error code in the following topics:</span></span>
  
- [<span data-ttu-id="4ffbf-190">Обработка сообщений об ошибках службы автообнаружения</span><span class="sxs-lookup"><span data-stu-id="4ffbf-190">Handling Autodiscover error messages</span></span>](handling-autodiscover-error-messages.md)
    
- [<span data-ttu-id="4ffbf-191">Обработка ошибок, связанных с уведомлений в веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="4ffbf-191">Handling notification-related errors in EWS in Exchange</span></span>](handling-notification-related-errors-in-ews-in-exchange.md)
    
- [<span data-ttu-id="4ffbf-192">Обработка ошибок, связанных с синхронизации в веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="4ffbf-192">Handling synchronization-related errors in EWS in Exchange</span></span>](handling-synchronization-related-errors-in-ews-in-exchange.md)
    
- [<span data-ttu-id="4ffbf-193">Обработка ошибок, связанных с удаления в веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="4ffbf-193">Handling deletion-related errors in EWS in Exchange</span></span>](handling-deletion-related-errors-in-ews-in-exchange.md)
    
## <a name="see-also"></a><span data-ttu-id="4ffbf-194">См. также</span><span class="sxs-lookup"><span data-stu-id="4ffbf-194">See also</span></span>


- [<span data-ttu-id="4ffbf-195">Разработка клиентов веб-служб для Exchange</span><span class="sxs-lookup"><span data-stu-id="4ffbf-195">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)
    
- [<span data-ttu-id="4ffbf-196">Инструменты и ресурсы для устранения неполадок приложений EWS для Exchange</span><span class="sxs-lookup"><span data-stu-id="4ffbf-196">Tools and resources for troubleshooting EWS applications for Exchange</span></span>](tools-and-resources-for-troubleshooting-ews-applications-for-exchange.md)
    

