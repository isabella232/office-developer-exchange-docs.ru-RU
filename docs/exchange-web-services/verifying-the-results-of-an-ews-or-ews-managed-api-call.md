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
# <a name="verifying-the-results-of-an-ews-or-ews-managed-api-call"></a>Проверка результатов вызова веб-служб Exchange или управляемый API EWS

Узнайте, как проверка результатов вызовов веб-служб Exchange или управляемый API веб-служб Exchange.
  
При действия не работает корректно, будет полезным взглянуть, что происходит изучив запросов SOAP, которые приложение передает по сети и ответы, сервер отправляет обратно. [Средства и ресурсы, необходимые для устранения неполадок приложений веб-служб Exchange](tools-and-resources-for-troubleshooting-ews-applications-for-exchange.md) статье содержатся ссылки на средства для регистрации и просмотра этих запросов SOAP. После создания запросов и ответов, как проверяется правильно обработать запрос отправки на сервере? Познакомьтесь. 
  
При отправке запросов веб-служб Exchange, которому необходимо запустить программу вашей проверки, установив атрибут **ResponseClass** для каждого сообщения ответа в ответе. Который будет указано, будет ли операция успешно завершена для каждого элемента. 
  
В зависимости от объекта, что метод вызова, если вы используете управляемый API EWS для отправки запросов, можно выполнить некоторые проверки, с помощью объектов ответа. Однако поскольку ответ SOAP содержит подмножеством возможностей, включенных в объекты ответа управляемый API веб-служб Exchange, можно рассмотреть в ответе SOAP. Так как ответ SOAP часто может содержать больше сведений, чем объекты ответа управляемый API веб-служб Exchange, начните проверить с ответа SOAP.
  
## <a name="verifying-the-results-of-a-soap-response"></a>Проверка результатов ответа SOAP
<a name="bk_verifysoap"> </a>

При получении ответа SOAP в первую очередь необходимо рассмотреть является атрибутом **ResponseClass** . Этот атрибут включается в каждый экземпляр **ResponseMessageType** в элементе [ResponseMessages](http://msdn.microsoft.com/library/2071bed8-ea66-4627-aa4f-a1d9a025cf3d%28Office.15%29.aspx) , как показано в следующем примере. 
  
```XML
<s:Body>
      <m:GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
        <m:ResponseMessages>
          <m:GetItemResponseMessage ResponseClass="Success">
          …
```

Ответ SOAP может содержать несколько сообщений ответа в один ответ SOAP, важно проверить каждого сообщения ответа по отдельности.
  
Если вы работаете с операции, которая включает в себя **ResponseClass** как часть ответа операции следующим образом, может возникнуть желание только проверка **ResponseClass** операции. 
  
```XML
<soap:Body>
  <m:AddDelegateResponse xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                         ResponseClass="Success"
                         xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
  …

```

Тем не менее состояние операции только отражает фигуры верхнего уровня ответа и не зависит от состояния всех ответов отдельных сообщений. В следующем примере [AddDelegateResponse](http://msdn.microsoft.com/library/d7e6bebb-5dbf-43c1-aacf-4b3ca6a7c429%28Office.15%29.aspx) операция имеет **ResponseClass** **Успех**, но базовый элемент [DelegateUserResponseMessageType](http://msdn.microsoft.com/library/3dc9552c-1e2d-40ac-a137-827883c2bb88%28Office.15%29.aspx) имеет значение **ResponseClass** **об ошибках**.
  
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

Поэтому для ответы SOAP веб-служб Exchange, нельзя полагаться на **ResponseClass** операции - необходимо рассмотреть **ResponseClass** каждого сообщения ответа, чтобы определить, является ли все ошибки обработки элементов при выполнении операции. 
  
### <a name="verifying-success"></a>Проверка успешности

Если каждый атрибут **ResponseClass** для каждого **ResponseMessage** атрибута задано значение **успешно**, операция выполнена успешно, для всех элементов, и можно перейти к следующей задаче.
  
В следующем примере показано успешного ответа на запрос операции [GetItem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) для получения отдельных элементов. Обратите внимание, что если **ResponseClass** **Успех**, связанный [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) всегда имеет значение **NoError**.
  
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

Ниже приведен успешного ответа на запрос операции **GetItem** для получения нескольких элементов. Все элементы [GetItemResponseMessage](http://msdn.microsoft.com/library/cc583723-54d1-4a17-8c1f-6586f70fdefd%28Office.15%29.aspx) имеет **ResponseClass** **успеха**.
  
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

### <a name="handling-errors-and-warnings"></a>Обработка ошибок и предупреждений

Когда был получен ответ, атрибут **ResponseClass** задано значение **Ошибка**, операция не завершена успешно на один или несколько элементов. Устраните проблему и повторите попытку запроса или частью вашего запроса с отказом. Значение атрибута **ResponseClass** значения **Предупреждение** только возвращенные операцией [ResolveNames](http://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) и указывает, что сущность не удалось разрешить уникальное удостоверение. Его можно пропустить для всех других операций. 
  
В следующем запросе атрибут **ResponseClass** имеет значение **ошибки**.
  
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

В этом примере веб-служб Exchange предоставляет сведения для отладки ошибки. Если атрибут **ResponseClass** имеет значение **ошибки**, в ответ, если применимо включены следующие дополнительные элементы:
  
- [MessageText](http://msdn.microsoft.com/library/59a23bdc-0d9a-4942-8b3c-9cdb11db1ab1%28Office.15%29.aspx) — описание ошибки. 
    
- [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) — содержит код ошибки, который может использоваться для дополнительные ресурсы по устранению неполадок. 
    
- [MessageXml](http://msdn.microsoft.com/library/bcaf9e35-d351-48f3-baad-f90c633cba8a%28Office.15%29.aspx) — определяет элементы, вызвавшей ошибку. 
    
- [DescriptiveLinkKey](http://msdn.microsoft.com/library/f7f36749-00f3-4915-b17c-e3caa0af6e67%28Office.15%29.aspx) — неиспользуемых. 
    
Сведения, представленные в этих элементов можно использовать для изучения проблемы. В предыдущем примере **MessageText** указывает, что свойство не подходит для типа объекта. Запрос был получение сообщения электронной почты, но набор свойств включены **AssociatedCalendarItemId**, который допустимо только для элементов встречи.
  
В следующем примере показано ошибку, которое было получено как часть пакетной операции для получения нескольких элементов электронной почты. Первый элемент был успешно извлечен, **ResponseClass** задано значение **Success**. Не удалось найти второй элемент, **ResponseClass** задано значение **ошибки**.
  
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

Когда один или несколько элементов в пакетной запрос не удается обработать по запросу, возвращается сообщение об ошибке для каждого элемента, который не удалось и остальные элементы в пакете обрабатываются как ожидалось. В пакетной обработке могут возникнуть ошибки при элемент был удален и таким образом не может быть отправлено, получить или обновлены, а также если элемент перемещен в другую папку, а следовательно, имеет новый идентификатор элемента. Так как операция завершится для некоторых элементов и возвращает ошибку, если не удается обработать один или несколько элементов, важно проверить каждый атрибут **ResponseClass** перед переходом к следующей операции. 
  
Если сведения, предоставленные элементы ответа не помогает исправить запроса или в противном случае разблокировать вы, просмотрите [дальнейшие инструкции](#bk_nextsteps).
  
## <a name="verifying-the-results-of-an-ews-managed-api-method-call"></a>Проверка результатов для вызова метода управляемый API EWS
<a name="bk_successful"> </a>

Если вы с помощью управляемого интерфейса API веб-служб Exchange и вызов метода [ExchangeService](http://msdn.microsoft.com/EN-US/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) объекта, метод скорее всего возвращает объект [ServiceResponseCollection](http://msdn.microsoft.com/EN-US/library/dd633715%28v=exchg.80%29.aspx) , который содержит коллекцию объектов [ServiceResponse](http://msdn.microsoft.com/EN-US/library/microsoft.exchange.webservices.data.serviceresponse%28v=exchg.80%29.aspx) или набора объекты, производные от **ServiceResponse** объектов. **ServiceResponseCollection** и включенных объектов **ServiceResponse** содержат информацию о результатов вызова метода, который можно использовать для проверки результатов. 
  
Если вы с помощью управляемого интерфейса API веб-служб Exchange и вызов метода для объекта [элемента](http://msdn.microsoft.com/EN-US/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) или один из производных объектов, скорее всего метод не возвращает объект ответа для проверки успешности, но вызовет [исключение](http://msdn.microsoft.com/EN-US/library/c18k6c59) , если метод не завершена успешно. 
  
### <a name="verifying-success"></a>Проверка успешности

Преимущество использования управляемый API EWS заключается в обеспечении общего состояния при работе с несколькими элементами в один ответ. Поэтому если вызывается метод возвращает **ServiceResponseCollection**, можно проверить, что свойство [OverallResult](http://msdn.microsoft.com/en-us/library/dd634515%28v=exchg.80%29.aspx) **ServiceResponseCollection** равен [ServiceResult.Success](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresult%28v=exchg.80%29.aspx). Если это так, все элементы в процессе пакетной были успешно завершена; у вас нет проверка каждого объекта **ServiceResponse** по отдельности. Если свойство **OverallResult** установлено значение **ServiceResult.Success**, необходимо [обрабатывать ошибки или предупреждения](#bk_ewsmaerrors).
  
Метод вызова не возвращает **ServiceResponseCollection**, но возвращают объект **ServiceResponse** , необходимо проверить значение свойства **результатов** . Если значение **результата** **Success**, вы знаете метод выполнен успешно.
  
При вызове метода не имеет возвращаемого значения, действительно нет возможности проверки успешного выполнения с помощью управляемого интерфейса API веб-служб Exchange. До тех пор, пока не исключение, можно допустить метод выполнен успешно. Для дополнительной проверки также можно [Проверить ответ SOAP, чтобы проверить результаты](#bk_verifysoap).
  
### <a name="handling-errors-warnings-and-exceptions"></a>Обработка ошибок, предупреждений и исключения
<a name="bk_ewsmaerrors"> </a>

Если управляемый API EWS код создает **исключение**, можно использовать значение [Exception.Message](http://msdn.microsoft.com/EN-US/library/9btwf6wk) определить причину ошибки. Свойство **Message** содержит содержимое элемента [MessageText](http://msdn.microsoft.com/library/59a23bdc-0d9a-4942-8b3c-9cdb11db1ab1%28Office.15%29.aspx) в базовом ответа SOAP. Кроме того Если исключение типа объекта [ServiceResponseException](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponseexception%28v=exchg.80%29.aspx) , одним из наиболее распространенных исключений, вы также можете получить [код ошибки](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponseexception.errorcode%28v=exchg.80%29.aspx) , содержащихся в элемент SOAP [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) и [ответа](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponseexception.response%28v=exchg.80%29.aspx) свойство, которое идентифицирует связанного объекта [ServiceResponse](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse%28v=exchg.80%29.aspx) . Приведенный ниже код показано, как для перехвата и отображение содержимого **ServiceResponseException**. 
  
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

Если вызывается метод возвращает **ServiceResponseCollection**, и значение свойства **OverallResult** равно **Предупреждение** или **Ошибка**, необходимо хранить выполняют цикл по каждому объекту в **ServiceResponseCollection** для Поиск ошибки. Свойство **OverallResult** имеет значение **Предупреждение** , если хотя бы один ответа у **результата** значение для **предупреждения** и всех ответов имеют их значения **результатов** , задайте значение **Success**. Свойство **OverallResult** — это значение **ошибки** , если по крайней мере один ответа значении **результатов** **ошибки**. Если **OverallResult** **Предупреждение** или **Ошибка**, для объектов **ServiceResponse** соответствующим образом заданы следующие свойства: 
  
- [Код ошибки](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse.errorcode%28v=exchg.80%29.aspx) — содержит код ошибки, который может использоваться для дополнительные ресурсы по устранению неполадок. 
    
- [ErrorDetails](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse.errordetails%28v=exchg.80%29.aspx) — содержит сведения об ошибке для некоторых **ErrorCodes**. Например при **ErrorRecurrenceHasNoOccurrence**, код ошибки **ErrorDetails** будет содержать ключи для **EffectiveStartDate** и **EffectiveEndDate**. 
    
- [Сообщение об ошибке](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse.errormessage%28v=exchg.80%29.aspx) , описывающее ошибку. 
    
- [ErrorProperties](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse.errorproperties%28v=exchg.80%29.aspx) , если он доступен, определяет свойства, вызвавшей ошибку. Например при **ErrorInvalidPropertyForOperation**код ошибки **ErrorProperties** содержит определение свойства, недопустимый для запроса. 
    
- [Результат](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse.result%28v=exchg.80%29.aspx) — содержит **об ошибке** или **Предупреждение** при обнаружении неполадок. 
    
Если сведения, предоставленные свойства **ServiceResponse** не предоставляет достаточно сведений, чтобы исправить вызова метода или разблокировать вы, просмотреть [дальнейшие действия](#bk_nextsteps) получать дополнительные сведения о значениях **код ошибки** . 
  
## 
<a name="bk_nextsteps"> </a>

Можно найти дополнительные сведения об устранении неполадок в следующих разделах:
  
- Элемент [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) 
    
- Перечисление [ServiceError](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceerror%28v=exchg.80%29.aspx) 
    
- [Ошибки, связанные с свойство веб-служб Exchange](ews-property-related-errors.md)
    
Кроме того в зависимости от того, что вы пытаетесь выполнить в вашем запросе, могут найти дополнительные полезные сведения о коде ошибки в следующих разделах:
  
- [Обработка сообщений об ошибках службы автообнаружения](handling-autodiscover-error-messages.md)
    
- [Обработка ошибок, связанных с уведомлений в веб-служб Exchange в Exchange](handling-notification-related-errors-in-ews-in-exchange.md)
    
- [Обработка ошибок, связанных с синхронизации в веб-служб Exchange в Exchange](handling-synchronization-related-errors-in-ews-in-exchange.md)
    
- [Обработка ошибок, связанных с удаления в веб-служб Exchange в Exchange](handling-deletion-related-errors-in-ews-in-exchange.md)
    
## <a name="see-also"></a>См. также


- [Разработка клиентов веб-служб для Exchange](develop-web-service-clients-for-exchange.md)
    
- [Инструменты и ресурсы для устранения неполадок приложений EWS для Exchange](tools-and-resources-for-troubleshooting-ews-applications-for-exchange.md)
    

