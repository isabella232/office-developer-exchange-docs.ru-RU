---
title: Работать с скрытыми папками с помощью EWS в Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 7ae7c045-cd90-4c9f-baf5-0464d5058f45
description: Сведения о том, как сделать папку скрытой и найти скрытые папки с помощью управляемого API EWS или EWS в Exchange.
ms.openlocfilehash: 72efc16ecc247d307b7300526e7d345fe6bdd3ac
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761136"
---
# <a name="work-with-hidden-folders-by-using-ews-in-exchange"></a><span data-ttu-id="1b4d7-103">Работать с скрытыми папками с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="1b4d7-103">Work with hidden folders by using EWS in Exchange</span></span>

<span data-ttu-id="1b4d7-104">Сведения о том, как сделать папку скрытой и найти скрытые папки с помощью управляемого API EWS или EWS в Exchange.</span><span class="sxs-lookup"><span data-stu-id="1b4d7-104">Learn how to make a folder hidden and find hidden folders by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="1b4d7-105">С одним исключением папки в корне почтового ящика Exchange (поддерево без IPM) скрыты от пользователя.</span><span class="sxs-lookup"><span data-stu-id="1b4d7-105">With one exception, folders in the root of an Exchange mailbox (the non-IPM subtree) are hidden from the user.</span></span> <span data-ttu-id="1b4d7-106">И наоборот, все папки в **мсгфолдеррут** (поддерево IPM) видимы пользователю.</span><span class="sxs-lookup"><span data-stu-id="1b4d7-106">Conversely, all folders in the **MsgFolderRoot** (the IPM subtree) are visible to the user.</span></span> <span data-ttu-id="1b4d7-107">Как скрыть папку в **мсгфолдеррут**?</span><span class="sxs-lookup"><span data-stu-id="1b4d7-107">So how do you hide a folder under the **MsgFolderRoot**?</span></span> <span data-ttu-id="1b4d7-108">Это не то, что очень просто — он передается только одному свойству, расширенному свойству [пидтагаттрибутехидден](http://msdn.microsoft.com/en-us/library/cc433490%28v=exchg.80%29.aspx) (0x10F4000B).</span><span class="sxs-lookup"><span data-stu-id="1b4d7-108">It's not that tricky — it comes down to just one property, the [PidTagAttributeHidden](http://msdn.microsoft.com/en-us/library/cc433490%28v=exchg.80%29.aspx) (0x10F4000B) extended property.</span></span> <span data-ttu-id="1b4d7-109">Если для этого свойства задано **значение true**, Outlook или другой клиент, использующий свойство для определения видимости папки, будет скрывать эту папку из представления пользователя.</span><span class="sxs-lookup"><span data-stu-id="1b4d7-109">When this property is set to **true**, Outlook or another client that uses the property to determine folder visibility will hide the folder from the user's view.</span></span> <span data-ttu-id="1b4d7-110">Так как это расширенное свойство, оно более сложно использовать, чем свойство среднего значения папки, поэтому в этой статье рассматриваются основные сценарии.</span><span class="sxs-lookup"><span data-stu-id="1b4d7-110">Because this is an extended property, it's more complex to use than your average folder property, so this article will walk you through the main scenarios.</span></span>
  
<span data-ttu-id="1b4d7-111">**Таблица 1. Методы управляемого API EWS и операции EWS для работы с скрытыми папками**</span><span class="sxs-lookup"><span data-stu-id="1b4d7-111">**Table 1. EWS Managed API methods and EWS operations for working with hidden folders**</span></span>

|<span data-ttu-id="1b4d7-112">**Задача**</span><span class="sxs-lookup"><span data-stu-id="1b4d7-112">**Task**</span></span>|<span data-ttu-id="1b4d7-113">**Метод управляемого API EWS**</span><span class="sxs-lookup"><span data-stu-id="1b4d7-113">**EWS Managed API method**</span></span>|<span data-ttu-id="1b4d7-114">**Операция EWS**</span><span class="sxs-lookup"><span data-stu-id="1b4d7-114">**EWS operation**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="1b4d7-115">Скрытие папки</span><span class="sxs-lookup"><span data-stu-id="1b4d7-115">Hide a folder</span></span>  <br/> |<span data-ttu-id="1b4d7-116">[Folder. Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) , за которым следует [Папка. Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="1b4d7-116">[Folder.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) followed by [Folder.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx)</span></span> <br/> |<span data-ttu-id="1b4d7-117">[Папка](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) , за которой следует [операцию UpdateFolder](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="1b4d7-117">[GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) followed by [UpdateFolder](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx)</span></span> <br/> |
|<span data-ttu-id="1b4d7-118">Поиск скрытых папок</span><span class="sxs-lookup"><span data-stu-id="1b4d7-118">Find hidden folders</span></span>  <br/> |[<span data-ttu-id="1b4d7-119">финдфолдерс</span><span class="sxs-lookup"><span data-stu-id="1b4d7-119">FindFolders</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="1b4d7-120">FindFolder</span><span class="sxs-lookup"><span data-stu-id="1b4d7-120">FindFolder</span></span>](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) <br/> |
   
<span data-ttu-id="1b4d7-121">Хотите узнать, что такое одно исключение — то есть какая папка в корне видна пользователям?</span><span class="sxs-lookup"><span data-stu-id="1b4d7-121">Are you wondering what the one exception is — that is, what folder in the root IS visible to users?</span></span> <span data-ttu-id="1b4d7-122">Это папка Finder (также называемая значением перечисления **SearchFolders**[веллкновнфолдер](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) или значением **SearchFolders**[дистингуишедфолдерид](http://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) ), которая содержит папки поиска пользователей.</span><span class="sxs-lookup"><span data-stu-id="1b4d7-122">It's the Finder folder (also known as the **SearchFolders**[WellKnownFolder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) enumeration value, or the **searchfolders**[DistinguishedFolderId](http://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) element value), which contains users' search folders.</span></span> <span data-ttu-id="1b4d7-123">Папки поиска, созданные в папке Finder, видимы для пользователей Outlook.</span><span class="sxs-lookup"><span data-stu-id="1b4d7-123">Search folders created in the Finder folder are visible to Outlook users.</span></span> <span data-ttu-id="1b4d7-124">Если вам нужно создать папку поиска, невидимую для пользователей, переместите ее в корневую папку, чтобы скрыть ее.</span><span class="sxs-lookup"><span data-stu-id="1b4d7-124">If you need to create a search folder that is not visible to users, move it under the root folder to hide it.</span></span> <span data-ttu-id="1b4d7-125">В отличие от других папок, если задать **PidTagAttributeHidden** для свойства пидтагаттрибутехидден **значение true** , папка поиска в папке Finder не будет скрыта.</span><span class="sxs-lookup"><span data-stu-id="1b4d7-125">Unlike for other folders, setting the **PidTagAttributeHidden** property to **true** will not hide a search folder in the Finder folder.</span></span> 
  
## <a name="hide-a-folder-by-using-the-ews-managed-api"></a><span data-ttu-id="1b4d7-126">Скрытие папки с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="1b4d7-126">Hide a folder by using the EWS Managed API</span></span>
<span data-ttu-id="1b4d7-127"><a name="bk_hideewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="1b4d7-127"><a name="bk_hideewsma"> </a></span></span>

<span data-ttu-id="1b4d7-128">Можно [сделать существующую папку](how-to-work-with-folders-by-using-ews-in-exchange.md#bk_createfolderewsma) скрытой, изменив расширенное свойство [пидтагаттрибутехидден](http://msdn.microsoft.com/en-us/library/cc433490%28v=exchg.80%29.aspx) на **true**.</span><span class="sxs-lookup"><span data-stu-id="1b4d7-128">You can [make an existing folder](how-to-work-with-folders-by-using-ews-in-exchange.md#bk_createfolderewsma) a hidden folder by changing the [PidTagAttributeHidden](http://msdn.microsoft.com/en-us/library/cc433490%28v=exchg.80%29.aspx) extended property to **true**.</span></span> <span data-ttu-id="1b4d7-129">Сначала создайте [Определение расширенного свойства для свойства](properties-and-extended-properties-in-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="1b4d7-129">First, create an [extended property definition for the property](properties-and-extended-properties-in-ews-in-exchange.md).</span></span> <span data-ttu-id="1b4d7-130">Затем используйте метод [BIND](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) для получения папки, а затем обновите значение свойства **пидтагаттрибутехидден** на true и используйте метод [Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) для сохранения изменений.</span><span class="sxs-lookup"><span data-stu-id="1b4d7-130">Next, use the [Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) method to get to the folder, then update the value of the **PidTagAttributeHidden** property to true, and use the [Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) method to save the changes.</span></span> 
  
<span data-ttu-id="1b4d7-131">В этом примере предполагается, что **Служба** является допустимым объектом [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) для владельца почтового ящика, что пользователь прошел проверку подлинности на сервере Exchange, а **FolderId** — допустимый [Folder.ID](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx) , определяющий папку для скрытия.</span><span class="sxs-lookup"><span data-stu-id="1b4d7-131">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object for the mailbox owner, that the user has been authenticated to an Exchange server, and that **folderId** is a valid [Folder.Id](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx) that identifies the folder to hide.</span></span> 
  
```cs
private static void MakeHidden(FolderId folderId, ExchangeService service)
{
    // Create an extended property definition for the PidTagAttributeHidden property.
    ExtendedPropertyDefinition isHiddenProp = new ExtendedPropertyDefinition(0x10f4, MapiPropertyType.Boolean);
    PropertySet propSet = new PropertySet(isHiddenProp);
    // Bind to a folder and retrieve the PidTagAttributeHidden property.
    Folder folder = Folder.Bind(service, folderId, propSet);
    // Set the PidTagAttributeHidden property to true.
    folder.SetExtendedProperty(isHiddenProp, true);
    // Save the changes.
    folder.Update();
}
```

## <a name="hide-a-folder-by-using-ews"></a><span data-ttu-id="1b4d7-132">Скрытие папки с помощью EWS</span><span class="sxs-lookup"><span data-stu-id="1b4d7-132">Hide a folder by using EWS</span></span>
<span data-ttu-id="1b4d7-133"><a name="bk_hideews"> </a></span><span class="sxs-lookup"><span data-stu-id="1b4d7-133"><a name="bk_hideews"> </a></span></span>

<span data-ttu-id="1b4d7-134">С помощью EWS можно [сделать существующую папку](how-to-work-with-folders-by-using-ews-in-exchange.md#bk_createfolderewsma) скрытой, изменив свойство [пидтагаттрибутехидден](http://msdn.microsoft.com/en-us/library/cc433490%28v=exchg.80%29.aspx) расширенного свойства на **true**.</span><span class="sxs-lookup"><span data-stu-id="1b4d7-134">You can use EWS to [make an existing folder](how-to-work-with-folders-by-using-ews-in-exchange.md#bk_createfolderewsma) a hidden folder by changing the [PidTagAttributeHidden](http://msdn.microsoft.com/en-us/library/cc433490%28v=exchg.80%29.aspx) extended property to **true**.</span></span> <span data-ttu-id="1b4d7-135">Сначала [используйте операцию GetSetting для получения папки,](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) а затем извлеките свойство **пидтагаттрибутехидден** , включив элемент [екстендедфиелдури](http://msdn.microsoft.com/library/b3c6ea3a-9ead-44b9-9d99-64ecf12bde23%28Office.15%29.aspx) , и установите для параметра **Пропертитаг** значение 4340, а для параметра **propertyType** значение — Boolean.</span><span class="sxs-lookup"><span data-stu-id="1b4d7-135">First, use the [GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) operation to get to the folder, then retrieve the **PidTagAttributeHidden** property by including the [ExtendedFieldURI](http://msdn.microsoft.com/library/b3c6ea3a-9ead-44b9-9d99-64ecf12bde23%28Office.15%29.aspx) element, and setting the **PropertyTag** value to 4340 and the **PropertyType** value to Boolean.</span></span> 
  
<span data-ttu-id="1b4d7-136">Это также запрос XML, который отправляет управляемый API EWS при использовании метода **BIND** для получения папки перед тем, как [сделать ее скрытой папкой](#bk_hideewsma).</span><span class="sxs-lookup"><span data-stu-id="1b4d7-136">This is also the XML request that the EWS Managed API sends when you use the **Bind** method to get a folder before [making it a hidden folder](#bk_hideewsma).</span></span>
  
<span data-ttu-id="1b4d7-137">Значение [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) укорачивается для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="1b4d7-137">The [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) value is shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:GetFolder>
      <m:FolderShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:ExtendedFieldURI PropertyTag="4340"
                              PropertyType="Boolean" />
        </t:AdditionalProperties>
      </m:FolderShape>
      <m:FolderIds>
        <t:FolderId Id="IQywAAAA==" />
      </m:FolderIds>
    </m:GetFolder>
  </soap:Body>
</soap:Envelope>
```

Сервер отвечает на запрос к **папке** жетфолдерреспонсе с сообщением [GetFolderResponse](http://msdn.microsoft.com/library/47abeec8-78dd-4297-8525-099174ec880d%28Office.15%29.aspx) , которое содержит значение **ошибки**элемента [респонсекоде](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) , которое указывает, что папка была получена успешно. В ответ также включается [значение](http://msdn.microsoft.com/library/196278d4-5e77-4e0a-8af6-8ac065610510%28Office.15%29.aspx) для параметра [ExtendedProperty](http://msdn.microsoft.com/library/f9701409-b620-4afe-b9ee-4c1e95507af7%28Office.15%29.aspx). <span data-ttu-id="1b4d7-140">В этом примере **значение** равно **false**, что означает, что папка в настоящее время не скрыта.</span><span class="sxs-lookup"><span data-stu-id="1b4d7-140">In this example, the **Value** is set to **false**, which means that the folder is currently not hidden.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="898"
                         MinorBuildNumber="23"
                         Version="V2_10"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Folders>
            <t:Folder>
              <t:FolderId Id="IQywAAAA=="
                          ChangeKey="AQAAABYAAAD32nSTjepyT63rYH17n9THAAAAABED" />
              <t:ExtendedProperty>
                <t:ExtendedFieldURI PropertyTag="0x10f4"
                                    PropertyType="Boolean" />
                <t:Value>false</t:Value>
              </t:ExtendedProperty>
            </t:Folder>
          </m:Folders>
        </m:GetFolderResponseMessage>
      </m:ResponseMessages>
    </m:GetFolderResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="1b4d7-141">Чтобы изменить значение свойства **ExtendedProperty** на true, используйте операцию [операцию UpdateFolder](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="1b4d7-141">To change the value of the **ExtendedProperty** to true, use the [UpdateFolder](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) operation.</span></span> <span data-ttu-id="1b4d7-142">Включите элементы **ExtendedProperty**, **екстендедфиелдури**и **value** для расширенного свойства **Пидтагаттрибутехидден** и присвойте элементу **value значение** **true** , чтобы скрыть папку.</span><span class="sxs-lookup"><span data-stu-id="1b4d7-142">Include the **ExtendedProperty**, **ExtendedFieldURI**, and **Value** elements for the **PidTagAttributeHidden** extended property, and set the **Value** element to **true** to hide the folder.</span></span> 
  
<span data-ttu-id="1b4d7-143">Это также запрос XML, который отправляет управляемый API EWS при использовании метода **Update** для обновления папки, чтобы [сделать ее скрытой папкой](#bk_hideewsma).</span><span class="sxs-lookup"><span data-stu-id="1b4d7-143">This is also the XML request that the EWS Managed API sends when you use the **Update** method to update a folder to [make it a hidden folder](#bk_hideewsma).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:UpdateFolder>
      <m:FolderChanges>
        <t:FolderChange>
          <t:FolderId Id="IQywAAAA=="
                      ChangeKey="AQAAABYAAAD32nSTjepyT63rYH17n9THAAAAABED" />
          <t:Updates>
            <t:SetFolderField>
              <t:ExtendedFieldURI PropertyTag="4340"
                                  PropertyType="Boolean" />
              <t:Folder>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="4340"
                                      PropertyType="Boolean" />
                  <t:Value>true</t:Value>
                </t:ExtendedProperty>
              </t:Folder>
            </t:SetFolderField>
          </t:Updates>
        </t:FolderChange>
      </m:FolderChanges>
    </m:UpdateFolder>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="1b4d7-144">Сервер отвечает на запрос **операцию UpdateFolder** с сообщением [упдатефолдерреспонсе](http://msdn.microsoft.com/library/31f47739-dc9c-46ba-9e3f-cce25dc85e6e%28Office.15%29.aspx) , которое содержит значение **ошибки**элемента [респонсекоде](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) , которое указывает на то, что папка успешно обновлена, и теперь скрыта.</span><span class="sxs-lookup"><span data-stu-id="1b4d7-144">The server responds to the **UpdateFolder** request with an [UpdateFolderResponse](http://msdn.microsoft.com/library/31f47739-dc9c-46ba-9e3f-cce25dc85e6e%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the folder was updated successfully, and is now hidden.</span></span>
  
## <a name="find-all-hidden-folders-by-using-the-ews-managed-api"></a><span data-ttu-id="1b4d7-145">Поиск всех скрытых папок с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="1b4d7-145">Find all hidden folders by using the EWS Managed API</span></span>
<span data-ttu-id="1b4d7-146"><a name="bk_findhiddenewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="1b4d7-146"><a name="bk_findhiddenewsma"> </a></span></span>

<span data-ttu-id="1b4d7-147">Все скрытые папки можно найти в родительской папке, создав [Определение расширенного свойства](properties-and-extended-properties-in-ews-in-exchange.md) для расширенного свойства **пидтагаттрибутехидден** , а затем используя метод [финдфолдерс](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx) для поиска папок со значением **пидтагаттрибутехидден** , равным **true**.</span><span class="sxs-lookup"><span data-stu-id="1b4d7-147">You can find all hidden folders under a parent folder by creating an [extended property definition](properties-and-extended-properties-in-ews-in-exchange.md) for the **PidTagAttributeHidden** extended property, and then using the [FindFolders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx) method to find folders with a **PidTagAttributeHidden** value that is set to **true**.</span></span> <span data-ttu-id="1b4d7-148">В этом примере используется Мсгфолдеррут, также называемый верхней частью банка данных или поддерево IPM, в качестве родительской папки для поиска в.</span><span class="sxs-lookup"><span data-stu-id="1b4d7-148">This example uses the MsgFolderRoot, also known as the Top of Information Store, or IPM Subtree, as the parent folder to search under.</span></span>
  
<span data-ttu-id="1b4d7-149">В этом примере предполагается, что **Служба** является допустимым объектом [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) для владельца почтового ящика и что пользователь прошел проверку подлинности на сервере Exchange.</span><span class="sxs-lookup"><span data-stu-id="1b4d7-149">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object for the mailbox owner, and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
private static void FindHiddenFolders(ExchangeService service)
{
    // Create an extended property definition for the PidTagAttributeHidden property.
    ExtendedPropertyDefinition isHiddenProp = new ExtendedPropertyDefinition(0x10f4, MapiPropertyType.Boolean);
    // Create a folder view to retrieve up to 100 folders and 
    // retrieve only the PidTagAttributeHidden and the display name.
    FolderView folderView = new FolderView(100);
    folderView.PropertySet = new PropertySet(isHiddenProp, FolderSchema.DisplayName);
    // Indicate a Traversal value of Deep, so that all subfolders are retrieved.
    folderView.Traversal = FolderTraversal.Deep;
    // Find all hidden folders under the MsgFolderRoot.
    // This call results in a FindFolder call to EWS.
    FindFoldersResults findFolder = service.FindFolders(WellKnownFolderName.MsgFolderRoot,
            new SearchFilter.IsEqualTo(isHiddenProp, true), folderView);
    // Display the folder ID and display name of each hidden folder.
    foreach (Folder folder in findFolder)
    {
        Console.WriteLine("FolderId: {0}", folder.Id);
        Console.WriteLine("DisplayName: {0}", folder.DisplayName);
        Console.WriteLine("\r\n");
    }
}
```

## <a name="find-all-hidden-folders-by-using-ews"></a><span data-ttu-id="1b4d7-150">Поиск всех скрытых папок с помощью EWS</span><span class="sxs-lookup"><span data-stu-id="1b4d7-150">Find all hidden folders by using EWS</span></span>
<span data-ttu-id="1b4d7-151"><a name="bk_findhiddenews"> </a></span><span class="sxs-lookup"><span data-stu-id="1b4d7-151"><a name="bk_findhiddenews"> </a></span></span>

<span data-ttu-id="1b4d7-152">С помощью EWS можно найти все скрытые папки в существующей папке, вызвав операцию [FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) и выполнив поиск папок, у которых расширенное свойство [пидтагаттрибутехидден](http://msdn.microsoft.com/en-us/library/cc433490%28v=exchg.80%29.aspx) имеет значение **true**.</span><span class="sxs-lookup"><span data-stu-id="1b4d7-152">You can use EWS to find all hidden folders under an existing folder by calling the [FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) operation and searching for folders whose [PidTagAttributeHidden](http://msdn.microsoft.com/en-us/library/cc433490%28v=exchg.80%29.aspx) extended property is set to **true**.</span></span> <span data-ttu-id="1b4d7-153">Для этого включите[ограничение](http://msdn.microsoft.com/library/77f19014-d112-4999-8e83-ecc32a117a73%28Office.15%29.aspx) [исекуалто](http://msdn.microsoft.com/library/48e7e067-049c-4184-8026-071e6f558e8a%28Office.15%29.aspx), которое выполняет поиск элемента [Екстендедфиелдури](http://msdn.microsoft.com/library/b3c6ea3a-9ead-44b9-9d99-64ecf12bde23%28Office.15%29.aspx) для свойства **пидтагаттрибутехидден** ( **пропертитаг** значение равным 4243, а значение **propertyType** — Boolean), как показано в следующем запросе.</span><span class="sxs-lookup"><span data-stu-id="1b4d7-153">To do this, include an [IsEqualTo](http://msdn.microsoft.com/library/48e7e067-049c-4184-8026-071e6f558e8a%28Office.15%29.aspx)[Restriction](http://msdn.microsoft.com/library/77f19014-d112-4999-8e83-ecc32a117a73%28Office.15%29.aspx) that searches for the [ExtendedFieldURI](http://msdn.microsoft.com/library/b3c6ea3a-9ead-44b9-9d99-64ecf12bde23%28Office.15%29.aspx) element for the **PidTagAttributeHidden** property ( **PropertyTag** value to 4243 and the **PropertyType** value to Boolean), as shown in the following request.</span></span> <span data-ttu-id="1b4d7-154">В этом примере используется Мсгфолдеррут, также называемый верхней частью банка данных или поддерево IPM, в качестве родительской папки для поиска в.</span><span class="sxs-lookup"><span data-stu-id="1b4d7-154">This example uses the MsgFolderRoot, also known as the Top of Information Store, or IPM Subtree, as the parent folder to search under.</span></span> 
  
<span data-ttu-id="1b4d7-155">Это также запрос XML, который отправляет управляемый API EWS при использовании метода **финдфолдерс** для [поиска всех скрытых папок](#bk_findhiddenewsma).</span><span class="sxs-lookup"><span data-stu-id="1b4d7-155">This is also the XML request that the EWS Managed API sends when you use the **FindFolders** method to [find all hidden folders](#bk_findhiddenewsma).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Central Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:FindFolder Traversal="Deep">
      <m:FolderShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:ExtendedFieldURI PropertyTag="4340"
                              PropertyType="Boolean" />
          <t:FieldURI FieldURI="folder:DisplayName" />
        </t:AdditionalProperties>
      </m:FolderShape>
      <m:IndexedPageFolderView MaxEntriesReturned="100"
                               Offset="0"
                               BasePoint="Beginning" />
      <m:Restriction>
        <t:IsEqualTo>
          <t:ExtendedFieldURI PropertyTag="4340"
                              PropertyType="Boolean" />
          <t:FieldURIOrConstant>
            <t:Constant Value="true" />
          </t:FieldURIOrConstant>
        </t:IsEqualTo>
      </m:Restriction>
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="msgfolderroot" />
      </m:ParentFolderIds>
    </m:FindFolder>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="1b4d7-156">Сервер отвечает на запрос **FindFolder** с сообщением [финдфолдерреспонсе](http://msdn.microsoft.com/library/f5dd813c-9698-4a39-8fca-3a825df365ed%28Office.15%29.aspx) , которое содержит значение **ошибки**элемента [респонсекоде](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) , которое указывает, что поиск в папке выполнен успешно, а также все скрытые папки в корневой папке сообщений.</span><span class="sxs-lookup"><span data-stu-id="1b4d7-156">The server responds to the **FindFolder** request with a [FindFolderResponse](http://msdn.microsoft.com/library/f5dd813c-9698-4a39-8fca-3a825df365ed%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the folder search was successful, as well as all the hidden folders under the root message folder.</span></span>
  
<span data-ttu-id="1b4d7-157">Значения [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) сокращаются для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="1b4d7-157">The [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) values are shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="898"
                         MinorBuildNumber="23"
                         Version="V2_10"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="6"
                        TotalItemsInView="6"
                        IncludesLastItemInRange="true">
            <t:Folders>
              <t:ContactsFolder>
                <t:FolderId Id="IBHgAAAA=="
                            ChangeKey="AwAAABYAAAD32nSTjepyT63rYH17n9THAAAAAACz" />
                <t:DisplayName>{06967759-274D-40B2-A3EB-D7F9E73727D7}</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x10f4"
                                      PropertyType="Boolean" />
                  <t:Value>true</t:Value>
                </t:ExtendedProperty>
              </t:ContactsFolder>
              <t:ContactsFolder>
                <t:FolderId Id="IBHwAAAA=="
                            ChangeKey="AwAAABYAAAD32nSTjepyT63rYH17n9THAAAAAAC7" />
                <t:DisplayName>{A9E2BC46-B3A0-4243-B315-60D991004455}</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x10f4"
                                      PropertyType="Boolean" />
                  <t:Value>true</t:Value>
                </t:ExtendedProperty>
              </t:ContactsFolder>
              <t:ContactsFolder>
                <t:FolderId Id="IBIQAAAA=="
                            ChangeKey="AwAAABYAAAD32nSTjepyT63rYH17n9THAAAAAADO" />
                <t:DisplayName>GAL Contacts</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x10f4"
                                      PropertyType="Boolean" />
                  <t:Value>true</t:Value>
                </t:ExtendedProperty>
              </t:ContactsFolder>
              <t:ContactsFolder>
                <t:FolderId Id="IBHQAAAA=="
                            ChangeKey="AwAAABYAAAD32nSTjepyT63rYH17n9THAAAAAACa" />
                <t:DisplayName>Recipient Cache</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x10f4"
                                      PropertyType="Boolean" />
                  <t:Value>true</t:Value>
                </t:ExtendedProperty>
              </t:ContactsFolder>
              <t:Folder>
                <t:FolderId Id="HAAAAA=="
                            ChangeKey="AQAAABYAAAD32nSTjepyT63rYH17n9THAAAAAACS" />
                <t:DisplayName>Conversation Action Settings</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x10f4"
                                      PropertyType="Boolean" />
                  <t:Value>true</t:Value>
                </t:ExtendedProperty>
              </t:Folder>
              <t:Folder>
                <t:FolderId Id="IQywAAAA=="
                            ChangeKey="AQAAABYAAAD32nSTjepyT63rYH17n9THAAAeZIBf" />
                <t:DisplayName>TestFolder</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x10f4"
                                      PropertyType="Boolean" />
                  <t:Value>true</t:Value>
                </t:ExtendedProperty>
              </t:Folder>
            </t:Folders>
          </m:RootFolder>
        </m:FindFolderResponseMessage>
      </m:ResponseMessages>
    </m:FindFolderResponse>
  </s:Body>
</s:Envelope>
```

## 
<span data-ttu-id="1b4d7-158"><a name="bk_findhiddenews"> </a></span><span class="sxs-lookup"><span data-stu-id="1b4d7-158"><a name="bk_findhiddenews"> </a></span></span>

<span data-ttu-id="1b4d7-159">После скрытия или скрытия папок может потребоваться получить иерархию папок или [синхронизировать иерархию папок](how-to-synchronize-folders-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="1b4d7-159">After you have hidden or unhidden folders, you might want to get the folder hierarchy or [synchronize the folder hierarchy](how-to-synchronize-folders-by-using-ews-in-exchange.md).</span></span> <span data-ttu-id="1b4d7-160">В примерах, показывающих, как [получить иерархию папок с помощью управляемого API EWS](how-to-work-with-folders-by-using-ews-in-exchange.md#bk_getfolderhierarchyewsma) или [получения иерархии папок с помощью EWS](how-to-work-with-folders-by-using-ews-in-exchange.md#bk_getfolderhierarchyews) , также указываются скрытые папки в иерархии.</span><span class="sxs-lookup"><span data-stu-id="1b4d7-160">The examples that show you how to [get a folder hierarchy by using the EWS Managed API](how-to-work-with-folders-by-using-ews-in-exchange.md#bk_getfolderhierarchyewsma) or [get a folder hierarchy by using EWS](how-to-work-with-folders-by-using-ews-in-exchange.md#bk_getfolderhierarchyews) also indicate which folders in the hierarchy are hidden.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="1b4d7-161">См. также</span><span class="sxs-lookup"><span data-stu-id="1b4d7-161">See also</span></span>


- [<span data-ttu-id="1b4d7-162">Папки и элементы в веб-службах Exchange</span><span class="sxs-lookup"><span data-stu-id="1b4d7-162">Folders and items in EWS in Exchange</span></span>](folders-and-items-in-ews-in-exchange.md)
    
- [<span data-ttu-id="1b4d7-163">Работа с папками с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="1b4d7-163">Work with folders by using EWS in Exchange</span></span>](how-to-work-with-folders-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="1b4d7-164">Работайте с папками поиска с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="1b4d7-164">Work with search folders by using EWS in Exchange</span></span>](how-to-work-with-search-folders-by-using-ews-in-exchange.md)
    

