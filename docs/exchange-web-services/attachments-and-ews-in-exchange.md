---
title: Вложения и веб-службах Exchange
manager: sethgros
ms.date: 7/11/2016
ms.audience: Developer
localization_priority: Normal
ms.assetid: 8e4289a4-ec9d-4502-9854-c593c95d5f98
description: Сведения о вложениях и как управляемый API EWS или веб-служб Exchange в Exchange client представляет их.
ms.openlocfilehash: e4a97873798b8252e6fc14003519ce8a0eab7ec8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760937"
---
# <a name="attachments-and-ews-in-exchange"></a>Вложения и веб-службах Exchange

Сведения о вложениях и как управляемый API EWS или веб-служб Exchange в Exchange client представляет их.
  
Как правило, вложения, связанные с электронной почты элементов, но в действительности все элементы веб-служб Exchange — по электронной почте сообщения, элементы календаря, контакты, задачи, может содержать вложения.
  
## <a name="types-of-attachments"></a>Типы для вложений

Веб-служб Exchange разделяет на категории вложений на две группы: файла вложения и вложений элемента.
  
- **Item вложения:** Строго типизированные [элементы веб-служб Exchange](folders-and-items-in-ews-in-exchange.md), таких как сообщения электронной почты и элементы календаря, подключенные к другим элементом строго типизированных веб-служб Exchange. Любой элемент строго типизированные, которое может создаваться с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange можно использовать в качестве вложения элемента. Содержимое вложения элемента — это элемент строго типизированные, который предоставляет доступ ко всем его свойствам. Вложений элемента может иметь свои собственные вложений элемента, поэтому иерархия вложений элемента (или вложенных и вложения) — это возможно.
    
- **Вложений:** Всех файлов, например .txt, .jpg, .zip, PDF-файл, или даже MSG-файл. Вложенный файл имеет только несколько свойств, одним из них является base 64 закодированное содержимое файла. 
    
- **Ссылки вложения:** Любое вложение, на который ссылается файл поставщика, например в файле, расположенном в облаке. Вложение можно из нескольких поставщиков. 
    
При добавлении или получения вложений из элемента, он будет выполняться по-разному в зависимости от того, будет ли это вложенный файл или элемент вложения. Например чтобы добавить подключение файла к элементу, достаточно передавать в расположение файла. Чтобы добавить существующий элемент как вложение элемента, нужно скопировать свойства или содержимого MIME существующий элемент вложение элемента; только что не удается выполнить привязку к существующий элемент. Важно, так что различения двух типов вложений. В статьи [в этом разделе](#bk_inthissection)рассматриваются дополнительные сведения о различиях между вложений элемента и вложенных файлов.
  
## <a name="how-are-attachments-represented-programmatically"></a>Как вложения представлены программным способом?

Вложения хранятся в коллекции для элемента веб-служб Exchange. Коллекция вложений состоит из файлов вложений и/или вложений элемента. Метаданные о коллекции вложений доступен, если вы получаете элемента с помощью метода управляемый API EWS [Item.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) или операции EWS [GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) , но необходимые дополнительные вызовы для извлечения содержимого вложения. 
  
**В таблице 1. Метаданные о вложениях**

|**Объект метаданных**|**Свойство управляемый API EWS**|**Элемент веб-служб Exchange**|
|:-----|:-----|:-----|
|Значок вложения (не помечает встроенные вложения)  <br/> |[Item.HasAttachments](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.hasattachments%28v=exchg.80%29.aspx) <br/> |[HasAttachments](http://msdn.microsoft.com/library/538b7a85-11d7-4daa-8458-09b540760e8b%28Office.15%29.aspx) <br/> |
|Коллекция вложений  <br/> |[Item.Attachments](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.attachments%28v=exchg.80%29.aspx) <br/> |[Вложения](http://msdn.microsoft.com/library/b470e614-34bb-44f0-8790-7ddbdcbbd29d%28Office.15%29.aspx) <br/> |
|Идентификатор вложения  <br/> |[Attachment.Id](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.attachment.id%28v=exchg.80%29.aspx) <br/> |[Идентификатора вложения AttachmentId](http://msdn.microsoft.com/library/55a5fd77-60d1-40fa-8144-770600cedc6a%28Office.15%29.aspx) <br/> |
   
**В таблице 2. Сущности вложения**

|**Тип вложения**|**Управляемый API EWS класс**|**Элемент веб-служб Exchange**|
|:-----|:-----|:-----|
|Вложенный файл  <br/> |[FileAttachment](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.fileattachment%28v=exchg.80%29.aspx) <br/> |[FileAttachment](http://msdn.microsoft.com/library/3ecea174-73d1-47fd-8917-6065cef1d565%28Office.15%29.aspx) <br/> |
|Вложение элемента  <br/> |[ItemAttachment](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemattachment%28v=exchg.80%29.aspx) <br/> [ItemAttachment\<TItem\>](http://msdn.microsoft.com/en-us/library/dd635165%28v=exchg.80%29.aspx) <br/> |[ItemAttachment](http://msdn.microsoft.com/library/089ee599-f45e-46f5-a18a-5cfb3d2851ff%28Office.15%29.aspx) <br/> |
|Вложение в виде ссылки  <br/> |[ReferenceAttachmentType complexType (EWS)](http://msdn.microsoft.com/library/18bfa012-e903-d7f3-528a-31ccceb65463%28Office.15%29.aspx) <br/> |[ReferenceAttachment](http://msdn.microsoft.com/library/b9bde862-6b75-4a81-8033-00a47be4dc2f%28Office.15%29.aspx) <br/> |
   
## <a name="inline-attachments"></a>Встроенные вложения

Встроенные вложения — это специальные поколения вложения. Оба файла вложения и вложений элемента может быть встроенные вложения. Встроенным появится как часть содержимое текста запроса и сохраняет его положение относительно остального содержимого в элементе. 
  
Вложение является встроенным, если свойство управляемый API EWS [IsInline](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.attachment.isinline%28v=exchg.80%29.aspx) или элемент веб-служб Exchange [IsInline](http://msdn.microsoft.com/library/5e7712c8-372a-4a16-be64-360c5ff3961a%28Office.15%29.aspx) задано значение true. Встроенные вложения используются следующие дополнительные свойства и элементы для определения местоположения встроенным: 
  
- Управляемый API EWS — [ContentId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.attachment.contentid%28v=exchg.80%29.aspx) или [ContentLocation](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.attachment.contentlocation%28v=exchg.80%29.aspx) свойств. 
    
- Веб-служб Exchange — Элемент [ContentId](http://msdn.microsoft.com/library/bc59100d-6079-414b-a6e0-7c15feaa3184%28Office.15%29.aspx) или [ContentLocation](http://msdn.microsoft.com/library/d91cf587-24e3-4c13-8784-5ca29787cca7%28Office.15%29.aspx) . 
    
Обратите внимание, что свойство управляемый API EWS [HasAttachments](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.hasattachments%28v=exchg.80%29.aspx) и веб-служб Exchange [HasAttachments](http://msdn.microsoft.com/library/538b7a85-11d7-4daa-8458-09b540760e8b%28Office.15%29.aspx) элемент не отражают существование встроенные вложения, и почему также называются встроенные вложения скрыты вложения. Поэтому если задать свойство управляемый API EWS [IsInline](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.attachment.isinline%28v=exchg.80%29.aspx) или элемент веб-служб Exchange [IsInline](http://msdn.microsoft.com/library/5e7712c8-372a-4a16-be64-360c5ff3961a%28Office.15%29.aspx) имеет значение true, а у элемента есть не другие вложения, **HasAttachments** будет иметь значение false. Если ваш клиент использует **HasAttachments** для заполнения значок вложения или значок на сообщения электронной почты, обратите внимание, что значок будет отображаться для сообщений электронной почты с вложениями встроенного. 
  
## <a name="in-this-section"></a>В этом разделе
<a name="bk_inthissection"> </a>

- [Добавление вложения с помощью веб-служб Exchange в Exchange](how-to-add-attachments-by-using-ews-in-exchange.md)
    
- [Получение вложений с помощью веб-служб Exchange в Exchange](how-to-get-attachments-by-using-ews-in-exchange.md)
    
- [Удаление вложений с помощью веб-служб Exchange в Exchange](how-to-delete-attachments-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a>См. также
<a name="bk_additionalresources"> </a>

- [Разработка клиентов веб-служб для Exchange](develop-web-service-clients-for-exchange.md)
    
- [Папки и элементы в веб-службах Exchange](folders-and-items-in-ews-in-exchange.md)
    
- [Электронная почта и веб-службах Exchange](email-and-ews-in-exchange.md)
    

