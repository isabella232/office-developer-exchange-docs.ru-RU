---
title: Получение фотографий с помощью веб-служб Exchange в Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: f86d1099-1f57-47dc-abf2-4d5ae4e900a9
description: Узнайте, как получить пользовательские фотографии, которые связаны с почтовым ящиком или контактов с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.
ms.openlocfilehash: f0f5cddd41fc563fb9ed38e75b505830a3992411
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761045"
---
# <a name="get-user-photos-by-using-ews-in-exchange"></a><span data-ttu-id="2faab-103">Получение фотографий с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="2faab-103">Get user photos by using EWS in Exchange</span></span>

<span data-ttu-id="2faab-104">Узнайте, как получить пользовательские фотографии, которые связаны с почтовым ящиком или контактов с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.</span><span class="sxs-lookup"><span data-stu-id="2faab-104">Learn how to get user photos that are associated with a mailbox or contact by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="2faab-105">Приятно поместить фрагмент с именем.</span><span class="sxs-lookup"><span data-stu-id="2faab-105">It's nice to put a face to a name.</span></span> <span data-ttu-id="2faab-106">Если для помещения имен граней пользователей, приложение может запрашивать изображения, обычно фотографии, Exchange, который представляет учетную запись электронной почты.</span><span class="sxs-lookup"><span data-stu-id="2faab-106">If your users like to put names to faces, your application can request an image, typically a photo, from Exchange that represents an email account.</span></span> <span data-ttu-id="2faab-107">Можно получить фото пользователя, хранящиеся на сервере Exchange server для почтовых ящиков, либо вы можете получить фотографий контактов на контакты, хранятся в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="2faab-107">You can get a user photo stored on an Exchange server for a mailbox, or you can get a contact photo from contacts stored in your mailbox.</span></span>
  
<span data-ttu-id="2faab-108">Несколько новых технологий можно использовать для получения фотографии из почтовых ящиков или доменных служб Active Directory (AD DS).</span><span class="sxs-lookup"><span data-stu-id="2faab-108">You can use several different technologies to get photos from mailboxes or Active Directory Domain Services (AD DS).</span></span> <span data-ttu-id="2faab-109">Лучший способ получить фотографию зависит от типа контакта, которого требуется получать фотографию с.</span><span class="sxs-lookup"><span data-stu-id="2faab-109">The best way to get a photo depends on the type of contact that you want to get a photo from.</span></span> 
  
<span data-ttu-id="2faab-110">**В таблице 1. Технологии использовать для получения фотографии пользователя на основе типа контакта**</span><span class="sxs-lookup"><span data-stu-id="2faab-110">**Table 1. Technologies to use to get user photos based on contact type**</span></span>

|<span data-ttu-id="2faab-111">**Тип контакта**</span><span class="sxs-lookup"><span data-stu-id="2faab-111">**Contact type**</span></span>|<span data-ttu-id="2faab-112">**Технологии использовать**</span><span class="sxs-lookup"><span data-stu-id="2faab-112">**Technologies to use**</span></span>|
|:-----|:-----|
|<span data-ttu-id="2faab-113">Фото пользователя почтового ящика</span><span class="sxs-lookup"><span data-stu-id="2faab-113">Mailbox user photo</span></span>  <br/> |[<span data-ttu-id="2faab-114">Получение фото пользователя почтового ящика с помощью REST</span><span class="sxs-lookup"><span data-stu-id="2faab-114">Get a mailbox user photo by using REST</span></span>](#bk_REST)<br/><br/> [<span data-ttu-id="2faab-115">Получение фото пользователя с помощью веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="2faab-115">Get a user photo by using EWS</span></span>](#bk_EWS) <br/> |
|<span data-ttu-id="2faab-116">Фотографии контактов пользователя</span><span class="sxs-lookup"><span data-stu-id="2faab-116">Contact user photo</span></span>  <br/> |[<span data-ttu-id="2faab-117">Получение фотографий контактов пользователя с помощью управляемого интерфейса API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="2faab-117">Get a contact user photo by using EWS Managed API</span></span>](#bk_EWSMA)<br/><br/> [<span data-ttu-id="2faab-118">Получение фото пользователя с помощью веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="2faab-118">Get a user photo by using EWS</span></span>](#bk_EWS) <br/> |

<span data-ttu-id="2faab-119"><a name="bk_REST"> </a></span><span class="sxs-lookup"><span data-stu-id="2faab-119"></span></span>

## <a name="get-a-mailbox-user-photo-by-using-rest"></a><span data-ttu-id="2faab-120">Получение фото пользователя почтового ящика с помощью REST</span><span class="sxs-lookup"><span data-stu-id="2faab-120">Get a mailbox user photo by using REST</span></span>

<span data-ttu-id="2faab-121">Можно запросить фотографии пользователя с сервера Exchange с помощью стандартного запроса HTTPS, **Получение** .</span><span class="sxs-lookup"><span data-stu-id="2faab-121">You can request user photos from an Exchange server by using a standard HTTPS **GET** request.</span></span> <span data-ttu-id="2faab-122">В запросе укажите адрес электронной почты учетной записи и кода размер изображения, как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="2faab-122">In the request, specify the email account address and a size code for the image, as shown in the following example.</span></span> 
  
```HTML
https://Exchange Server/ews/Exchange.asmx/s/GetUserPhoto?email=email address&amp;size=size code
```

<span data-ttu-id="2faab-123">Используйте операцию [GetUserSettings](how-to-get-user-settings-from-exchange-by-using-autodiscover.md) службы автообнаружения для получения параметр **ExternalEwsUrl** , который содержит URL-адрес конечной точки веб-служб Exchange (EWS) и расположение обработчик **Exchange.asmx** HTTP, который возвращает фотографии пользователя.</span><span class="sxs-lookup"><span data-stu-id="2faab-123">Use the Autodiscover service [GetUserSettings](how-to-get-user-settings-from-exchange-by-using-autodiscover.md) operation to retrieve the **ExternalEwsUrl** setting, which contains the URL of the Exchange Web Services (EWS) endpoint and the location of the **Exchange.asmx** HTTP handler that returns the user photos.</span></span> 
  
<span data-ttu-id="2faab-124">Код каждого размер указывает высоту и ширину изображения в пикселях.</span><span class="sxs-lookup"><span data-stu-id="2faab-124">Each size code indicates the height and width of the image in pixels.</span></span> <span data-ttu-id="2faab-125">Например код размер **HR48x48** возвращает изображение, которое является 48 пикселов в высоту и 48 пикселей в высоту.</span><span class="sxs-lookup"><span data-stu-id="2faab-125">For example, the size code **HR48x48** returns an image that is 48 pixels high by 48 pixels wide.</span></span> <span data-ttu-id="2faab-126">Возможные значения для параметра кода размер совпадают с возможными значениями для элемента [SizeRequested](http://msdn.microsoft.com/library/e86f98b6-83b5-4530-80eb-dc5df42e2c62%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="2faab-126">The possible values for the size code parameter are the same as the possible values for the [SizeRequested](http://msdn.microsoft.com/library/e86f98b6-83b5-4530-80eb-dc5df42e2c62%28Office.15%29.aspx) element.</span></span> <span data-ttu-id="2faab-127">Если запрос указывает размер, который не поддерживается, будут возвращены наибольшее доступных фотографий.</span><span class="sxs-lookup"><span data-stu-id="2faab-127">If the request specifies a size that is not available, the largest available photo will be returned.</span></span> <span data-ttu-id="2faab-128">Если нет фотографий хранится на сервере Exchange, будут возвращены эскизное изображение, хранящиеся в AD DS для учетной записи.</span><span class="sxs-lookup"><span data-stu-id="2faab-128">If no photo is stored on the Exchange server, the thumbnail image stored in AD DS for the account will be returned.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="2faab-129">Код размера **HR48x48** всегда возвращает эскизное изображение Доменные службы Active Directory, если он доступен.</span><span class="sxs-lookup"><span data-stu-id="2faab-129">The **HR48x48** size code always returns the AD DS thumbnail image if it is available.</span></span> 
  
<span data-ttu-id="2faab-130">В следующем примере показано, как использовать запрос GET для извлечения фото пользователя для Sadie и сохраните его на локальный компьютер.</span><span class="sxs-lookup"><span data-stu-id="2faab-130">The following example shows how you can use the GET request to retrieve the user photo for Sadie and save it to your local computer.</span></span>
  
```cs
// Create the web request with the REST URL.
HttpWebRequest request = 
   WebRequest.Create("https://www.contoso.com/ews/exchange.asmx/s/GetUserPhoto?email=sadie@contoso.com&amp;size=HR240x240") 
   as HttpWebRequest;
// Submit the request.
using (HttpWebResponse resp = request.GetResponse() as HttpWebResponse)
{
   // Take the response and save it as an image.
   Bitmap image = new Bitmap(resp.GetResponseStream());
   image.Save("Sadie.jpg");
}

```

<span data-ttu-id="2faab-131">Запрос возвращает HTTP-ответа.</span><span class="sxs-lookup"><span data-stu-id="2faab-131">The request will return an HTTP response.</span></span> 
  
<span data-ttu-id="2faab-132">**В таблице 2. Коды ответа на запрос GetUserPhoto**</span><span class="sxs-lookup"><span data-stu-id="2faab-132">**Table 2. Response codes for a GetUserPhoto request**</span></span>

|<span data-ttu-id="2faab-133">**Код ответа**</span><span class="sxs-lookup"><span data-stu-id="2faab-133">**Response code**</span></span>|<span data-ttu-id="2faab-134">**Описание**</span><span class="sxs-lookup"><span data-stu-id="2faab-134">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="2faab-135">200</span><span class="sxs-lookup"><span data-stu-id="2faab-135">200</span></span>  <br/> |<span data-ttu-id="2faab-136">Изображение доступен для учетной записи электронной почты указанного и двоичные изображение находится в ответе.</span><span class="sxs-lookup"><span data-stu-id="2faab-136">An image is available for the specified email account and the binary image is contained in the response.</span></span>  <br/> |
|<span data-ttu-id="2faab-137">304</span><span class="sxs-lookup"><span data-stu-id="2faab-137">304</span></span>  <br/> |<span data-ttu-id="2faab-138">Изображение не был изменен с момента последнего **ETag** был возвращен в приложение.</span><span class="sxs-lookup"><span data-stu-id="2faab-138">The image has not changed since the last time the **ETag** was returned to the application.</span></span>  <br/> |
|<span data-ttu-id="2faab-139">404</span><span class="sxs-lookup"><span data-stu-id="2faab-139">404</span></span>  <br/> |<span data-ttu-id="2faab-140">Изображение не доступна для учетной записи электронной почты указанного.</span><span class="sxs-lookup"><span data-stu-id="2faab-140">No image is available for the specified email account.</span></span>  <br/> |

<span data-ttu-id="2faab-141"><a name="bk_REST"> </a></span><span class="sxs-lookup"><span data-stu-id="2faab-141"></span></span>

## <a name="cache-user-photos"></a><span data-ttu-id="2faab-142">Фотографии пользователя кэша</span><span class="sxs-lookup"><span data-stu-id="2faab-142">Cache user photos</span></span>

<span data-ttu-id="2faab-143">Exchange возвращает данные с типом контента изображение/jpeg, а также коллекцию значений заголовка.</span><span class="sxs-lookup"><span data-stu-id="2faab-143">Exchange returns the data with a content type of image/jpeg, along with a collection of header values.</span></span> <span data-ttu-id="2faab-144">Заголовок **ETag** аналогична изменить ключ.</span><span class="sxs-lookup"><span data-stu-id="2faab-144">The **ETag** header is similar to a change key.</span></span> <span data-ttu-id="2faab-145">Значение — это строка, представляющая время последнего обновления фотографии.</span><span class="sxs-lookup"><span data-stu-id="2faab-145">The value is a string that represents the last time the photo was updated.</span></span> <span data-ttu-id="2faab-146">**ETag** остаются неизменными для фото пользователя, пока не будет изменено фотографии.</span><span class="sxs-lookup"><span data-stu-id="2faab-146">The **ETag** remains the same for the user photo until the photo is changed.</span></span> <span data-ttu-id="2faab-147">Это значение **ETag** можно отправлять на сервер в запросе на **Получение** HTTPS в заголовок **If-None-Match** .</span><span class="sxs-lookup"><span data-stu-id="2faab-147">You can send this **ETag** value to the server in the HTTPS **GET** request in an **If-None-Match** header.</span></span> <span data-ttu-id="2faab-148">Если фотографии не изменилось с момента последнего запроса, сервер отправляет ответ HTTP 304, которое указывает, таким образом.</span><span class="sxs-lookup"><span data-stu-id="2faab-148">If the photo hasn't changed since the last request, the server will respond with an HTTP 304 response that indicates as such.</span></span> <span data-ttu-id="2faab-149">Это означает, что можно использовать фото пользователя, который ранее был запрошен и сохранения вместо обработки новый.</span><span class="sxs-lookup"><span data-stu-id="2faab-149">This means that you can use the user photo that you previously requested and saved rather than processing a new one.</span></span> 

<span data-ttu-id="2faab-150"><a name="bk_EWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="2faab-150"></span></span>

## <a name="get-a-contact-user-photo-by-using-ews-managed-api"></a><span data-ttu-id="2faab-151">Получение фотографий контактов пользователя с помощью управляемого интерфейса API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="2faab-151">Get a contact user photo by using EWS Managed API</span></span>

<span data-ttu-id="2faab-152">Приложение может использовать управляемый API EWS для получения фотографии контактов, если контакт хранится в папке контактов в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="2faab-152">Your application can use the EWS Managed API to retrieve photos for contacts, if the contact is stored in a contact folder in the user's mailbox.</span></span> <span data-ttu-id="2faab-153">Для этого сначала найдите **идентификатор элемента** для контакта требуется использовать.</span><span class="sxs-lookup"><span data-stu-id="2faab-153">To do this, first, find the **ItemId** for the contact you want use.</span></span> <span data-ttu-id="2faab-154">Затем после привязки к этому контакту, загрузите его в коллекцию вложений.</span><span class="sxs-lookup"><span data-stu-id="2faab-154">Then, after you bind to that contact, load it to the attachments collection.</span></span> <span data-ttu-id="2faab-155">Если у контакта фотографии, фотография будет вложений.</span><span class="sxs-lookup"><span data-stu-id="2faab-155">If the contact has a photo, the photo will be one of the attachments.</span></span> <span data-ttu-id="2faab-156">Просмотрите коллекцию вложений, проверки значения свойства **IsContactPhoto** .</span><span class="sxs-lookup"><span data-stu-id="2faab-156">Loop through the attachments collection, checking the value of the **IsContactPhoto** property.</span></span> <span data-ttu-id="2faab-157">Найдя фотографий контактов, можно сохранить его на локальный компьютер и приложение может получить доступ к.</span><span class="sxs-lookup"><span data-stu-id="2faab-157">When you find the contact photo, you can save it to your local computer, and your application can access it.</span></span> 
  
<span data-ttu-id="2faab-158">В следующем примере показано выполнение этого процесса.</span><span class="sxs-lookup"><span data-stu-id="2faab-158">The following example shows this process.</span></span> <span data-ttu-id="2faab-159">В этом примере предполагается, что эта **Служба** является допустимым объектом [ExchangeService](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) и пользователь прошел проверку подлинности на сервере Exchange.</span><span class="sxs-lookup"><span data-stu-id="2faab-159">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
private static void GetContactPhoto(ExchangeService service, string ItemId)
{
   // Bind to an existing contact by using the ItemId passed into this function.
   Contact contact = Contact.Bind(service, ItemId);
   // Load the contact to get access to the collection of attachments.
   contact.Load(new PropertySet(ContactSchema.Attachments));
   // Loop through the attachments looking for a contact photo.
   foreach (Attachment attachment in contact.Attachments)
   {
      if ((attachment as FileAttachment).IsContactPhoto)
      {
         // Load the attachment to access the content.
         attachment.Load();
      }
   }
   FileAttachment photo = contact.GetContactPictureAttachment();
   // Create a file stream and save the contact photo to your computer.
   using (FileStream file = new FileStream(photo.Name, FileMode.Create, System.IO.FileAccess.Write))
   {
      photo.Load(file);
   }
}

```

<span data-ttu-id="2faab-160"><a name="bk_EWS"> </a></span><span class="sxs-lookup"><span data-stu-id="2faab-160"></span></span>

## <a name="get-a-user-photo-by-using-ews"></a><span data-ttu-id="2faab-161">Получение фото пользователя с помощью веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="2faab-161">Get a user photo by using EWS</span></span>

<span data-ttu-id="2faab-162">Они будут фото пользователя из Доменные службы Active Directory, можно использовать операцию [GetUserPhoto](http://msdn.microsoft.com/library/f6e8143d-4235-428e-8f9c-ab6e9b1cfa6e%28Office.15%29.aspx) (Если вы знаете адрес электронной почты) или операции [ResolveNames](http://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) (Если вы не знаете адрес электронной почты).</span><span class="sxs-lookup"><span data-stu-id="2faab-162">If you're getting a user photo from AD DS, you can use the [GetUserPhoto](http://msdn.microsoft.com/library/f6e8143d-4235-428e-8f9c-ab6e9b1cfa6e%28Office.15%29.aspx) operation (if you know the email address) or the [ResolveNames](http://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) operation (if you don't know the email address).</span></span> <span data-ttu-id="2faab-163">Если они будут фото пользователя из папки "Контакты" в почтовом ящике, с помощью операции [GetItem](http://msdn.microsoft.com/library/6b96dace-1260-4b83-869a-7c31c5583daa%28Office.15%29.aspx) , следуют операции [GetAttachment](http://msdn.microsoft.com/library/24d10a15-b942-415e-9024-a6375708f326%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="2faab-163">If you're getting a user photo from a contacts folder in the mailbox, use the [GetItem](http://msdn.microsoft.com/library/6b96dace-1260-4b83-869a-7c31c5583daa%28Office.15%29.aspx) operation followed by the [GetAttachment](http://msdn.microsoft.com/library/24d10a15-b942-415e-9024-a6375708f326%28Office.15%29.aspx) operation.</span></span> <span data-ttu-id="2faab-164">В любом случае фотографии возвращается как строка в кодировке Base64 в ответе XML.</span><span class="sxs-lookup"><span data-stu-id="2faab-164">In either case, the photo is returned as a Base64-encoded string in the XML response.</span></span> 
  
### <a name="get-a-mailbox-user-photo-by-using-the-getuserphoto-operation"></a><span data-ttu-id="2faab-165">Получение фото пользователя почтового ящика с помощью операции GetUserPhoto</span><span class="sxs-lookup"><span data-stu-id="2faab-165">Get a mailbox user photo by using the GetUserPhoto operation</span></span>

<span data-ttu-id="2faab-166">С помощью операции **GetUserPhoto** не вызывает затруднений.</span><span class="sxs-lookup"><span data-stu-id="2faab-166">Using the **GetUserPhoto** operation is straightforward.</span></span> <span data-ttu-id="2faab-167">В XML-запрос укажите адрес электронной почты пользователя и [размер фотографии](http://msdn.microsoft.com/library/e86f98b6-83b5-4530-80eb-dc5df42e2c62%28Office.15%29.aspx) для возврата (в элементе [SizeRequested](http://msdn.microsoft.com/library/e86f98b6-83b5-4530-80eb-dc5df42e2c62%28Office.15%29.aspx) ).</span><span class="sxs-lookup"><span data-stu-id="2faab-167">In the XML request, specify the email address of the user, and the [size of the photo](http://msdn.microsoft.com/library/e86f98b6-83b5-4530-80eb-dc5df42e2c62%28Office.15%29.aspx) to return (in the [SizeRequested](http://msdn.microsoft.com/library/e86f98b6-83b5-4530-80eb-dc5df42e2c62%28Office.15%29.aspx) element).</span></span> <span data-ttu-id="2faab-168">В следующем примере запрос XML показано, как получить фотографию для Sadie Daniels, который является 360 пикселов 360 пикселей.</span><span class="sxs-lookup"><span data-stu-id="2faab-168">The following XML request example shows how to get a photo for Sadie Daniels that's 360 pixels wide by 360 pixels high.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013 "/>
   </soap:Header>
   <soap:Body>
      <m:GetUserPhoto>
         <m:Email>sadie@contoso.com</m:Email>
         <m:SizeRequested>HR360x360</m:SizeRequested>
      </m:GetUserPhoto>
   </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="2faab-169">Ниже приведен XML-ответ.</span><span class="sxs-lookup"><span data-stu-id="2faab-169">The following is the XML response.</span></span> <span data-ttu-id="2faab-170">Photo кодировки Base64 содержится в элементе [Свойства](http://msdn.microsoft.com/library/1124eac3-ebf2-4b81-96d3-96838c840433%28Office.15%29.aspx) (содержимое URL были сокращены для удобства чтения).</span><span class="sxs-lookup"><span data-stu-id="2faab-170">The Base64-encoded photo is contained in the [PictureData](http://msdn.microsoft.com/library/1124eac3-ebf2-4b81-96d3-96838c840433%28Office.15%29.aspx) element (the content has been shortened for readability).</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
         xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetUserPhotoResponse ResponseClass="Success" 
         xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <HasChanged>true</HasChanged>
      <PictureData>/9j/4AAQSkZJRgABAQEAYABgAAD/2wBDAAg... wATRRRSuB//2Q==</PictureData>
    </GetUserPhotoResponse>
  </s:Body>
</s:Envelope>

```

### <a name="get-a-mailbox-user-photo-by-using-the-resolvenames-operation"></a><span data-ttu-id="2faab-171">Получение фото пользователя почтового ящика с помощью операции ResolveNames</span><span class="sxs-lookup"><span data-stu-id="2faab-171">Get a mailbox user photo by using the ResolveNames operation</span></span>

<span data-ttu-id="2faab-172">Если вы не знаете адрес электронной почты пользователя, для которого вы получаете фотографию, можно [использовать операцию ResolveNames](how-to-resolve-ambiguous-names-by-using-ews-in-exchange-2013.md) , чтобы получить кандидатов для возможно соответствие.</span><span class="sxs-lookup"><span data-stu-id="2faab-172">If you don't know the email address of the user for whom you are getting a photo, you can [use the ResolveNames operation](how-to-resolve-ambiguous-names-by-using-ews-in-exchange-2013.md) to get candidates for a possible match.</span></span> <span data-ttu-id="2faab-173">При указании «AllProperties» для атрибута **ContactDataShape** элемента [ResolveNames](http://msdn.microsoft.com/library/c85207e1-1315-443b-94ec-2b58f405076b%28Office.15%29.aspx) большого объема данных, включая пользовательские фотографии, будут возвращены для каждого кандидата.</span><span class="sxs-lookup"><span data-stu-id="2faab-173">If you specify "AllProperties" for the **ContactDataShape** attribute of the [ResolveNames](http://msdn.microsoft.com/library/c85207e1-1315-443b-94ec-2b58f405076b%28Office.15%29.aspx) element, a lot of data, including user photos, will be returned for each candidate.</span></span> <span data-ttu-id="2faab-174">В следующем примере показано XML-запрос для разрешения имени «Sadie» и получить все свойства для каждого кандидата.</span><span class="sxs-lookup"><span data-stu-id="2faab-174">The following example shows the XML request to resolve the name "Sadie" and return all the properties for each candidate.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
<soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
  </soap:Header>  
<soap:Body>
  <m:ResolveNames ReturnFullContactData="true" ContactDataShape="AllProperties">
      <m:UnresolvedEntry>sadie</m:UnresolvedEntry>
    </m:ResolveNames>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="2faab-175">В ответе будут возвращены большого объема данных.</span><span class="sxs-lookup"><span data-stu-id="2faab-175">A lot of data will be returned in the response.</span></span> <span data-ttu-id="2faab-176">В следующем примере показано только данные, относящиеся к фото пользователя.</span><span class="sxs-lookup"><span data-stu-id="2faab-176">The following example shows only the data that is relevant to the user photo.</span></span> <span data-ttu-id="2faab-177">Элемент **фотографий** содержит кодировки Base64 фото пользователя (содержимое URL были сокращены для удобства чтения).</span><span class="sxs-lookup"><span data-stu-id="2faab-177">The **Photo** element contains the Base64-encoded user photo (the content has been shortened for readability).</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
         xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:ResolveNamesResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:ResolveNamesResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:ResolutionSet TotalItemsInView="1" IncludesLastItemInRange="true">
            <t:Resolution>
              <t:Mailbox>
                <t:Name>Sadie Daniels</t:Name>
                <t:EmailAddress>sadie@contoso.com</t:EmailAddress>
                <t:RoutingType>SMTP</t:RoutingType>
                <t:MailboxType>Mailbox</t:MailboxType>
              </t:Mailbox>
              <t:Contact>
                <t:DisplayName>Sadie Daniels</t:DisplayName>
                <t:GivenName>Sadie</t:GivenName>
                <t:Initials/>
                <t:CompanyName>CONTOSO</t:CompanyName>
......
                <t:Photo>/9j/4AAQSkZJRgABAQE...qKKKAP/2Q==</t:Photo>
......
              </t:Contact>
            </t:Resolution>
          </m:ResolutionSet>
        </m:ResolveNamesResponseMessage>
      </m:ResponseMessages>
    </m:ResolveNamesResponse>
  </s:Body>
</s:Envelope>

```

### <a name="get-a-contact-user-photo-by-using-the-getattachment-operation"></a><span data-ttu-id="2faab-178">Получение фотографий контактов пользователя с помощью операции GetAttachment</span><span class="sxs-lookup"><span data-stu-id="2faab-178">Get a contact user photo by using the GetAttachment operation</span></span>

<span data-ttu-id="2faab-179">Можно использовать веб-служб Exchange для получения фотографии с контактами, хранятся в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="2faab-179">You can use EWS to get photos from contacts stored in your mailbox.</span></span> <span data-ttu-id="2faab-180">Во-первых используйте операции **GetItem** для возврата всех свойств, поэтому можно искать фотографии.</span><span class="sxs-lookup"><span data-stu-id="2faab-180">First, you use the **GetItem** operation to return all properties so you can look for photos.</span></span> <span data-ttu-id="2faab-181">В следующем примере показано XML-запрос для получения элемента контакта.</span><span class="sxs-lookup"><span data-stu-id="2faab-181">The following example shows an XML request to get a contact item.</span></span> <span data-ttu-id="2faab-182">Идентификатор элемента был усечен для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="2faab-182">The item ID has been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetItem xmlns='http://schemas.microsoft.com/exchange/services/2006/messages'>
      <ItemShape>
        <t:BaseShape>AllProperties</t:BaseShape>
      </ItemShape>
      <ItemIds>
        <t:ItemId Id="AAAAGECXAAA=" ChangeKey="EQAAABYAAAD2WuN+TpqwSrNP9JCCMKC0AABLzXRv"/>
      </ItemIds>
    </GetItem>
  </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="2faab-183">Найдите элемент [HasPicture](http://msdn.microsoft.com/library/922a43fe-01bd-49f2-9261-e00e4699b8da%28Office.15%29.aspx) чтобы убедиться, что контакт находится связанных фотографий.</span><span class="sxs-lookup"><span data-stu-id="2faab-183">Look for the [HasPicture](http://msdn.microsoft.com/library/922a43fe-01bd-49f2-9261-e00e4699b8da%28Office.15%29.aspx) element to verify that the contact has an associated photo.</span></span> <span data-ttu-id="2faab-184">Найдите через коллекцию вложений, которая имеет значение true для элемента [IsContactPhoto](http://msdn.microsoft.com/library/ae36b5f9-a787-4863-9dbc-258ad724801d%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="2faab-184">Then look through the collection of attachments for one that has a value of true for the [IsContactPhoto](http://msdn.microsoft.com/library/ae36b5f9-a787-4863-9dbc-258ad724801d%28Office.15%29.aspx) element.</span></span> <span data-ttu-id="2faab-185">В следующем примере ответа показано только нужные данные.</span><span class="sxs-lookup"><span data-stu-id="2faab-185">The following response example shows only the relevant data.</span></span> <span data-ttu-id="2faab-186">Значения Идентификаторов сокращаются для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="2faab-186">The ID values are shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
         xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Contact>
              <t:ItemId Id="AAAAGECXAAA=" ChangeKey="EQAAABYAAAD2WuN+TpqwSrNP9JCCMKC0AABLzXRv"/>
              <t:ParentFolderId Id="nIxIAAA=" ChangeKey="AQAAAA=="/>
              <t:ItemClass>IPM.Contact</t:ItemClass>
              <t:Subject>Hope Gross</t:Subject>
              <t:Sensitivity>Normal</t:Sensitivity>
......
              <t:Attachments>
                <t:FileAttachment>
                  <t:AttachmentId Id="1LGlhgpgoA="/>
                  <t:Name>ContactPicture.jpg</t:Name>
                  <t:Size>6260</t:Size>
                  <t:LastModifiedTime>2011-03-09T16:55:55</t:LastModifiedTime>
                  <t:IsInline>false</t:IsInline>
                  <t:IsContactPhoto>true</t:IsContactPhoto>
                </t:FileAttachment>
              </t:Attachments>
......
              <t:HasPicture>true</t:HasPicture>
            </t:Contact>
          </m:Items>
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </m:GetItemResponse>
  </s:Body>
</s:Envelope>

```

Затем используйте операции **GetAttachment** с помощью **идентификатора вложения AttachmentId** для запроса вложения с фотографий контактов. В следующем примере показано запроса XML для получения вложения. <span data-ttu-id="2faab-189">Идентификатор сокращение для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="2faab-189">The ID is shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
xmlns:xsd="http://www.w3.org/2001/XMLSchema"
xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetAttachment xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <AttachmentShape/>
      <AttachmentIds>
         <t:AttachmentId Id="1LGlhgpgoA="/>
      </AttachmentIds>
    </GetAttachment>
  </soap:Body>
</soap:Envelope>

```

В следующем примере показано XML-ответ со сведениями о вложении запрошенного. <span data-ttu-id="2faab-191">Элемент [содержимого](http://msdn.microsoft.com/library/24f8c54a-505f-4fc0-b7e7-93ad50b97070%28Office.15%29.aspx) содержит строку в кодировке Base64 для фото пользователя, сокращение в этом примере для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="2faab-191">The [Content](http://msdn.microsoft.com/library/24f8c54a-505f-4fc0-b7e7-93ad50b97070%28Office.15%29.aspx) element contains the Base64-encoded string for the user photo, shortened in this example for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
         xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetAttachmentResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetAttachmentResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Attachments>
            <t:FileAttachment>
              <t:AttachmentId Id="+KsDBEr1LGlhgpgoA="/>
              <t:Name>ContactPicture.jpg</t:Name>
              <t:Content>/9j/4AAQSkZJRgABAQEAYABgAAD/2wBDAAg...D//2Q==</t:Content>
            </t:FileAttachment>
          </m:Attachments>
        </m:GetAttachmentResponseMessage>
      </m:ResponseMessages>
    </m:GetAttachmentResponse>
  </s:Body>
</s:Envelope>

```

<span data-ttu-id="2faab-192"><a name="bk_EWS"> </a></span><span class="sxs-lookup"><span data-stu-id="2faab-192"></span></span>

## <a name="decode-a-base64-encoded-string"></a><span data-ttu-id="2faab-193">Декодирования строка в кодировке Base64</span><span class="sxs-lookup"><span data-stu-id="2faab-193">Decode a Base64-encoded string</span></span>

<span data-ttu-id="2faab-194">Независимо от того, операция, которую можно использовать для получения фото пользователя вам потребуются для декодирования эту строку, чтобы можно было использовать в приложении.</span><span class="sxs-lookup"><span data-stu-id="2faab-194">Regardless of the operation you use to get a user photo, you'll need to decode that string so you can use it in your application.</span></span> <span data-ttu-id="2faab-195">Следующем примере показано, как декодировать строки, а затем сохраните на локальный компьютер, поэтому приложения могут обращаться к ней позже.</span><span class="sxs-lookup"><span data-stu-id="2faab-195">The following example shows how to decode the string, and then save it to your local computer so you application can access it later.</span></span>
  
```cs
// Convert the encoded string into a byte array.
byte[] data = System.Convert.FromBase64String(Photo);
// Create a memory stream to read the data.
MemoryStream ms = new MemoryStream(data);
// Save the data on your local computer as a JPG image.
using (FileStream file = new FileStream(ContactName + ".jpg", FileMode.Create, System.IO.FileAccess.Write))
{
   byte[] bytes = new byte[ms.Length];
   ms.Read(bytes, 0, (int)ms.Length);
   file.Write(bytes, 0, bytes.Length);
   ms.Close();
}

```

## <a name="see-also"></a><span data-ttu-id="2faab-196">См. также</span><span class="sxs-lookup"><span data-stu-id="2faab-196">See also</span></span>

- [<span data-ttu-id="2faab-197">Пользователи и контакты в EWS для Exchange</span><span class="sxs-lookup"><span data-stu-id="2faab-197">People and contacts in EWS in Exchange</span></span>](people-and-contacts-in-ews-in-exchange.md)    
- [<span data-ttu-id="2faab-198">Разрешения неоднозначных имен с помощью веб-служб Exchange в Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="2faab-198">Resolve ambiguous names by using EWS in Exchange 2013</span></span>](how-to-resolve-ambiguous-names-by-using-ews-in-exchange-2013.md)    
- [<span data-ttu-id="2faab-199">Процесс контакты партиями с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="2faab-199">Process contacts in batches by using EWS in Exchange</span></span>](how-to-process-contacts-in-batches-by-using-ews-in-exchange.md)
    

