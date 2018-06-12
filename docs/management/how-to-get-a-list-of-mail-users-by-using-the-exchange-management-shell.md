---
title: Ознакомьтесь со списком пользователей почты с помощью командной консоли Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8b790dc8-5c4f-4acf-bbe7-63523395fbe7
description: Использование командлетов командной консоли Exchange для создания инструмента, который возвращает список пользователей почтового ящика Exchange
ms.openlocfilehash: 6f64330a11e372bffbea2fcd88bcfa0231ec0f28
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761256"
---
# <a name="get-a-list-of-mail-users-by-using-the-exchange-management-shell"></a><span data-ttu-id="13eba-103">Ознакомьтесь со списком пользователей почты с помощью командной консоли Exchange</span><span class="sxs-lookup"><span data-stu-id="13eba-103">Get a list of mail users by using the Exchange Management Shell</span></span>

<span data-ttu-id="13eba-104">Использование командлетов командной консоли Exchange для создания инструмента, который возвращает список пользователей почтового ящика Exchange</span><span class="sxs-lookup"><span data-stu-id="13eba-104">Learn how to use Exchange Management Shell cmdlets to create a tool that returns a list of Exchange mailbox users.</span></span>
  
<span data-ttu-id="13eba-105">**Применимо к:** Exchange Online | Exchange Server 2013 | Office 365</span><span class="sxs-lookup"><span data-stu-id="13eba-105">**Applies to:** Exchange Online | Exchange Server 2013 | Office 365</span></span> 
  
<span data-ttu-id="13eba-106">Получение списка пользователей из Exchange Online, Exchange Online в составе Office 365 или версии Exchange, начиная с Exchange 2013 с помощью управляемой инструмент, который вызывает это командлет командной консоли Exchange выполняется в два этапа.</span><span class="sxs-lookup"><span data-stu-id="13eba-106">Getting a list of users from Exchange Online, Exchange Online as part of Office 365, or a version of Exchange starting with Exchange 2013 by using a managed tool that calls an Exchange Management Shell cmdlet is a two-step process.</span></span> <span data-ttu-id="13eba-107">Во-первых установить удаленного пространство на сервере Exchange; Запустите командлет для получения сведений о пользователе в удаленном пространстве.</span><span class="sxs-lookup"><span data-stu-id="13eba-107">First, you establish a remote runspace on an Exchange server; then, you run the cmdlet to retrieve the user information in the remote runspace.</span></span> 

<span data-ttu-id="13eba-108">Для подключения к удаленной пространства выполнения, необходимо выполнить проверку подлинности на сервере Exchange Server с помощью схемы проверки подлинности, который соответствует требованиям безопасности организации.</span><span class="sxs-lookup"><span data-stu-id="13eba-108">To connect to the remote runspace, you have to authenticate with the Exchange server by using the authentication scheme that meets the security requirements of your organization.</span></span> 

<span data-ttu-id="13eba-109">В этой статье приведены примеры кода, которые можно использовать для настройки удаленных пространства выполнения и запустите это командлет командной консоли Exchange для получения списка пользователей с сервера Exchange.</span><span class="sxs-lookup"><span data-stu-id="13eba-109">This article provides code examples that you can use to set up a remote runspace and run an Exchange Management Shell cmdlet to get a list of users from an Exchange server.</span></span>

<span data-ttu-id="13eba-110"><a name="bk_prerequisites"> </a></span><span class="sxs-lookup"><span data-stu-id="13eba-110"></span></span>

## <a name="prerequisites-for-getting-a-list-of-mailbox-users"></a><span data-ttu-id="13eba-111">Необходимые условия для получения списка пользователей почтового ящика</span><span class="sxs-lookup"><span data-stu-id="13eba-111">Prerequisites for getting a list of mailbox users</span></span>

<span data-ttu-id="13eba-112">Для выполнения этой задачи требуется ссылка на следующие пространства имен:</span><span class="sxs-lookup"><span data-stu-id="13eba-112">To perform this task, you need a reference to the following namespaces:</span></span>
  
- <span data-ttu-id="13eba-113">**System.Collections.ObjectModel**</span><span class="sxs-lookup"><span data-stu-id="13eba-113">**System.Collections.ObjectModel**</span></span>
- <span data-ttu-id="13eba-114">**System.Management.Automation**</span><span class="sxs-lookup"><span data-stu-id="13eba-114">**System.Management.Automation**</span></span>
- <span data-ttu-id="13eba-115">**System.Management.Automation.Remoting**</span><span class="sxs-lookup"><span data-stu-id="13eba-115">**System.Management.Automation.Remoting**</span></span>
- <span data-ttu-id="13eba-116">**System.Management.Automation.Runspaces**</span><span class="sxs-lookup"><span data-stu-id="13eba-116">**System.Management.Automation.Runspaces**</span></span>
    
> [!NOTE]
>  <span data-ttu-id="13eba-p102">При создании приложения с помощью Visual Studio необходимо добавить к проекту ссылку на сборку System.Management.Automation.dll. Найти сборку можно, пройдя по одной из следующих ссылок:</span><span class="sxs-lookup"><span data-stu-id="13eba-p102">When you are using Visual Studio to create an application, you must add a reference to the System.Management.Automation.dll assembly to the project. The assembly can be found in one of the following locations:</span></span>
> - <span data-ttu-id="13eba-119">Для ОС Windows XP и Windows Vista — каталог установки Windows PowerShell ($PSHOME).</span><span class="sxs-lookup"><span data-stu-id="13eba-119">For Windows XP and Windows Vista operating systems, the Windows PowerShell installation directory ($PSHOME).</span></span>
> - <span data-ttu-id="13eba-120">Для ОС Windows 7 и Windows 8 — папка Windows\assembly\GAC_MSIL\System.Management.Automation.</span><span class="sxs-lookup"><span data-stu-id="13eba-120">For the Windows 7 and Windows 8 operating systems, the following folder: Windows\assembly\GAC_MSIL\System.Management.Automation.</span></span> 
  
<span data-ttu-id="13eba-121">Не загружать оснастку управления Exchange 2013 в пространстве на компьютерах, работающих под управлением приложений, которые автоматизируют командлетам командной консоли Exchange.</span><span class="sxs-lookup"><span data-stu-id="13eba-121">Do not load the Exchange 2013 Management snap-in into the runspace on computers that are running applications that automate Exchange Management Shell cmdlets.</span></span> <span data-ttu-id="13eba-122">В приложении вместо этого необходимо создать удаленный пространства выполнения, как описано далее в этой статье.</span><span class="sxs-lookup"><span data-stu-id="13eba-122">The application should instead create a remote runspace, as described later in this article.</span></span>

<span data-ttu-id="13eba-123"><a name="bk_gettinglistmailbox"> </a></span><span class="sxs-lookup"><span data-stu-id="13eba-123"></span></span>

## <a name="connect-to-a-remote-runspace-on-an-exchange-server"></a><span data-ttu-id="13eba-124">Создание удаленного пространства выполнения на сервере Exchange</span><span class="sxs-lookup"><span data-stu-id="13eba-124">Connect to a remote runspace on an Exchange server</span></span>

<span data-ttu-id="13eba-p104">Метод подключения к удаленному пространству выполнения, в котором будет использован командлет командной консоли Exchange, зависит от выбранной схемы проверки подлинности. В этом разделе приведены примеры кодов для подключения к удаленному пространству выполнения при использовании одного из методов проверки подлинности, перечисленных в таблице ниже.</span><span class="sxs-lookup"><span data-stu-id="13eba-p104">The method that you use to connect to a remote runspace to use an Exchange Management Shell cmdlet varies based on the authentication scheme that you are using. This section provides code examples that show how to connect to a remote runspace when you are using an authentication method listed in the following table.</span></span>
  
|<span data-ttu-id="13eba-127">**Метод проверки подлинности**</span><span class="sxs-lookup"><span data-stu-id="13eba-127">**Authentication method**</span></span>|<span data-ttu-id="13eba-128">**Применимо к**</span><span class="sxs-lookup"><span data-stu-id="13eba-128">**Applies to**</span></span>|<span data-ttu-id="13eba-129">**Универсальный код ресурса (URI)**</span><span class="sxs-lookup"><span data-stu-id="13eba-129">**URI**</span></span>|
|:-----|:-----|:-----|
|[<span data-ttu-id="13eba-130">Подключение к удаленной пространства выполнения на Exchange Online с помощью обычной проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="13eba-130">Connect to a remote runspace on Exchange Online by using basic authentication</span></span>](#bk_basic) <br/> |<span data-ttu-id="13eba-131">Серверы Exchange Online</span><span class="sxs-lookup"><span data-stu-id="13eba-131">Exchange Online servers</span></span>  <br/> |`https://outlook.office365.com/PowerShell-LiveID`<br/><br/>`https://<server>/PowerShell-LiveID`  <br/> |
|[<span data-ttu-id="13eba-132">Подключение к удаленной пространства выполнения с помощью проверки подлинности сертификата</span><span class="sxs-lookup"><span data-stu-id="13eba-132">Connect to a remote runspace by using certificate authentication</span></span>](#bk_cert) <br/> |<span data-ttu-id="13eba-133">Серверы Exchange Online и локальные серверы Exchange</span><span class="sxs-lookup"><span data-stu-id="13eba-133">Exchange Online and Exchange on-premises servers</span></span>  <br/> |`https://outlook.office365.com/PowerShell`<br/><br/>`https://<server>/PowerShell`<br/><br/>`http://<server>/PowerShell`  <br/> |
|[<span data-ttu-id="13eba-134">Подключение к удаленной пространство на сервере Exchange с помощью проверки подлинности Kerberos</span><span class="sxs-lookup"><span data-stu-id="13eba-134">Connect to a remote runspace on an Exchange server by using Kerberos authentication</span></span>](#bk_Kerberos) <br/> |<span data-ttu-id="13eba-135">Серверы Exchange Online и локальные серверы Exchange</span><span class="sxs-lookup"><span data-stu-id="13eba-135">Exchange Online and Exchange on-premises servers</span></span>  <br/> |`https://<server>/PowerShell`<br/><br/>`http://<server>/PowerShell`  <br/> |

<span data-ttu-id="13eba-136"><a name="bk_basic"> </a></span><span class="sxs-lookup"><span data-stu-id="13eba-136"></span></span>

### <a name="connect-to-a-remote-runspace-on-exchange-online-by-using-basic-authentication"></a><span data-ttu-id="13eba-137">Подключение к удаленному пространству выполнения на сервере Exchange Online с помощью обычной проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="13eba-137">Connect to a remote runspace on Exchange Online by using basic authentication</span></span>

<span data-ttu-id="13eba-138">В следующем примере кода определяется метод **GetUsersUsingBasicAuth** , который создает пространства выполнения Командная консоль Exchange на удаленном сервере Exchange Online с помощью обычной проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="13eba-138">The following code example defines the **GetUsersUsingBasicAuth** method, which creates an Exchange Management Shell runspace on a remote Exchange Online server by using basic authentication.</span></span> <span data-ttu-id="13eba-139">Метод затем вызывает метод **GetUserInformation** , как определено в раздел, [Ознакомьтесь со списком пользователей почтовых ящиков из удаленного пространства выполнения](#bk_remote), чтобы получить список пользователей на удаленном сервере.</span><span class="sxs-lookup"><span data-stu-id="13eba-139">The method then calls the **GetUserInformation** method, as defined in the section [Get a list of mailbox users from a remote runspace](#bk_remote), to return a list of users on the remote server.</span></span>
  
<span data-ttu-id="13eba-140">Для этого метода требуются следующие параметры:</span><span class="sxs-lookup"><span data-stu-id="13eba-140">This method requires the following parameters:</span></span>
  
-  <span data-ttu-id="13eba-141">**liveIDConnectionUri** &ndash; Строка, содержащая URI сервера Exchange Online, на котором будет выполнена проверка подлинности приложения.</span><span class="sxs-lookup"><span data-stu-id="13eba-141">**liveIDConnectionUri** &ndash; A string that contains the URI of the Exchange Online server that will authenticate the application.</span></span> <span data-ttu-id="13eba-142">Если запущен Exchange Online в Office 365 — это URI https://outlook.office365.com/PowerShell-LiveID; в противном случае — URI https://\<имя_сервера\>/PowerShell-LiveID.</span><span class="sxs-lookup"><span data-stu-id="13eba-142">If Exchange Online is running in Office 365, the URI is https://outlook.office365.com/PowerShell-LiveID; otherwise, the URI is https://\<servername\>/PowerShell-LiveID.</span></span> 
    
-  <span data-ttu-id="13eba-143">**schemaUri** &ndash; Строка, содержащая URI документа схемы, который определяет схему Командная консоль Exchange.</span><span class="sxs-lookup"><span data-stu-id="13eba-143">**schemaUri** &ndash; A string that contains the URI of the schema document that defines the Exchange Management Shell schema.</span></span> <span data-ttu-id="13eba-144">Схема URI — это http://schemas.microsoft.com/powershell/Microsoft.Exchange.</span><span class="sxs-lookup"><span data-stu-id="13eba-144">The schema URI is http://schemas.microsoft.com/powershell/Microsoft.Exchange.</span></span> 
    
-  <span data-ttu-id="13eba-145">**учетные данные** &ndash; Объект [PSCredential](http://msdn.microsoft.com/en-us/library/system.management.automation.pscredential%28VS.85%29.aspx) , содержащий учетные данные пользователя, который выполняется приложение.</span><span class="sxs-lookup"><span data-stu-id="13eba-145">**credentials** &ndash; A [PSCredential](http://msdn.microsoft.com/en-us/library/system.management.automation.pscredential%28VS.85%29.aspx) object that contains the credentials of the user who is running the application.</span></span> 
    
-  <span data-ttu-id="13eba-146">**Count** &ndash; Число пользователей почтовых ящиков Exchange для возврата.</span><span class="sxs-lookup"><span data-stu-id="13eba-146">**count** &ndash; The number of Exchange mailbox users to return.</span></span> 
    
```cs
public Collection<PSObject> GetUsersUsingBasicAuth(
    string liveIDConnectionUri, string schemaUri, PSCredential credentials, int count)
{
    WSManConnectionInfo connectionInfo = new WSManConnectionInfo(
        new Uri(liveIDConnectionUri),
        schemaUri, credentials);
    connectionInfo.AuthenticationMechanism = AuthenticationMechanism.Basic;
    using (Runspace runspace = RunspaceFactory.CreateRunspace(connectionInfo))
    {
        return GetUserInformation(count, runspace);
    }
}
```


```vb
  Function GetUsersUsingBasicAuth( _
    ByVal LiveIDConnectionUri As String, ByVal ScehmaUri As String, _
    ByVal Credentials As PSCredential, ByVal Count As Integer) As Collection(Of PSObject)
    Dim ConnectionInfo As WSManConnectionInfo = _
        New WSManConnectionInfo(New Uri(LiveIDConnectionUri), ScehmaUri, Credentials)
    ConnectionInfo.AuthenticationMechanism = AuthenticationMechanism.Basic
    Dim RemoteRunspace As Runspace
    RemoteRunspace = RunspaceFactory.CreateRunspace(ConnectionInfo)
    Return GetUserInformation(Count, RemoteRunspace)
  End Function

```

<span data-ttu-id="13eba-147"><a name="bk_cert"> </a></span><span class="sxs-lookup"><span data-stu-id="13eba-147"></span></span>

### <a name="connect-to-a-remote-runspace-by-using-certificate-authentication"></a><span data-ttu-id="13eba-148">Подключение к удаленному пространству выполнения с помощью проверки подлинности на основе сертификата</span><span class="sxs-lookup"><span data-stu-id="13eba-148">Connect to a remote runspace by using certificate authentication</span></span>

<span data-ttu-id="13eba-149">В следующем примере кода определяется метод **GetUsersUsingCertificate** , который создает пространства выполнения Командная консоль Exchange на удаленном сервере с помощью сертификата.</span><span class="sxs-lookup"><span data-stu-id="13eba-149">The following code example defines the **GetUsersUsingCertificate** method, which creates an Exchange Management Shell runspace on a remote server by using a certificate.</span></span> <span data-ttu-id="13eba-150">Метод затем вызывает метод **GetUserInformation** , как определено в раздел, [Ознакомьтесь со списком пользователей почтовых ящиков из удаленного пространства выполнения](#bk_remote), чтобы получить список пользователей на удаленном сервере.</span><span class="sxs-lookup"><span data-stu-id="13eba-150">The method then calls the **GetUserInformation** method, as defined in the section [Get a list of mailbox users from a remote runspace](#bk_remote), to return a list of users on the remote server.</span></span>
  
<span data-ttu-id="13eba-151">Для этого метода требуются следующие параметры:</span><span class="sxs-lookup"><span data-stu-id="13eba-151">This method requires the following parameters:</span></span>
  
-  <span data-ttu-id="13eba-152">**отпечаток** &ndash; Строка, содержащая отпечаток сертификата, который используется для проверки подлинности в приложении.</span><span class="sxs-lookup"><span data-stu-id="13eba-152">**thumbprint** &ndash; A string that contains the thumbprint of the certificate that is used to authenticate the application.</span></span> 
    
-  <span data-ttu-id="13eba-153">**certConnectionUri** &ndash; Строка, содержащая URI сервера, на котором будет выполнена проверка подлинности сертификата.</span><span class="sxs-lookup"><span data-stu-id="13eba-153">**certConnectionUri** &ndash; A string that contains the URI of the server that will authenticate the certificate.</span></span> <span data-ttu-id="13eba-154">URI будет одно из перечисленных в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="13eba-154">The URI will be one of those listed in the following table.</span></span> 
    
    <span data-ttu-id="13eba-155">**В таблице 1. certConnectionUri коды URI**</span><span class="sxs-lookup"><span data-stu-id="13eba-155">**Table 1. certConnectionUri URIs**</span></span>

    |<span data-ttu-id="13eba-156">**Сервер**</span><span class="sxs-lookup"><span data-stu-id="13eba-156">**Server**</span></span>|<span data-ttu-id="13eba-157">**Универсальный код ресурса (URI)**</span><span class="sxs-lookup"><span data-stu-id="13eba-157">**URI**</span></span>|
    |:-----|:-----|
    |<span data-ttu-id="13eba-158">Сервер Exchange, не использующий протокол SSL</span><span class="sxs-lookup"><span data-stu-id="13eba-158">Exchange server without using SSL</span></span>  <br/> |`http://<servername>/PowerShell`  <br/> |
    |<span data-ttu-id="13eba-159">Сервер Exchange, использующий протокол SSL</span><span class="sxs-lookup"><span data-stu-id="13eba-159">Exchange server using SSL</span></span>  <br/> |`https://<servername>/PowerShell`  <br/> |
    |<span data-ttu-id="13eba-160">Exchange Online в составе Office 365</span><span class="sxs-lookup"><span data-stu-id="13eba-160">Exchange Online as part of Office 365</span></span>  <br/> |`https://outlook.office365.com/PowerShell`  <br/> |
   
- <span data-ttu-id="13eba-161">**schemaUri** &ndash; Строка, содержащая URI документа схемы, который определяет схему Командная консоль Exchange.</span><span class="sxs-lookup"><span data-stu-id="13eba-161">**schemaUri** &ndash; A string that contains the URI of the schema document that defines the Exchange Management Shell schema.</span></span> <span data-ttu-id="13eba-162">Схема URI — это http://schemas.microsoft.com/powershell/Microsoft.Exchange.</span><span class="sxs-lookup"><span data-stu-id="13eba-162">The schema URI is http://schemas.microsoft.com/powershell/Microsoft.Exchange.</span></span> 
    
- <span data-ttu-id="13eba-163">**Count** &ndash; Число пользователей почтовых ящиков Exchange для возврата.</span><span class="sxs-lookup"><span data-stu-id="13eba-163">**count** &ndash; The number of Exchange mailbox users to return.</span></span> 
    
```cs
public Collection<PSObject> GetUsersUsingCertificate(
    string thumbprint, string certConnectionUri, string schemaUri, int count)
{
    WSManConnectionInfo connectionInfo = new WSManConnectionInfo(
        new Uri(certConnectionUri),
        schemaUri,
        thumbprint)
    using (Runspace runspace = RunspaceFactory.CreateRunspace(connectionInfo))
    {
        return GetUserInformation(count, runspace);
    }
}
```


```vb
  Function GetUsersUsingCertificate( _
    ByVal Thumbprint As String, ByVal CertConnectionUri As String, _
    ByVal SchemaUri As String, ByVal Count As Integer) As Collection(Of PSObject)
    Dim ConnectionInfo As WSManConnectionInfo
    ConnectionInfo = New WSManConnectionInfo(New Uri(CertConnectionUri), SchemaUri, Thumbprint)
    Dim RemoteRunspace As Runspace
    RemoteRunspace = RunspaceFactory.CreateRunspace(ConnectionInfo)
    Return GetUserInformation(Count, RemoteRunspace)
  End Function

```

<span data-ttu-id="13eba-164"><a name="bk_Kerberos"> </a></span><span class="sxs-lookup"><span data-stu-id="13eba-164"></span></span>

### <a name="connect-to-a-remote-runspace-on-an-exchange-server-by-using-kerberos-authentication"></a><span data-ttu-id="13eba-165">Подключение к удаленному пространству выполнения на сервере Exchange с помощью проверки подлинности Kerberos</span><span class="sxs-lookup"><span data-stu-id="13eba-165">Connect to a remote runspace on an Exchange server by using Kerberos authentication</span></span>

<span data-ttu-id="13eba-166">В следующем примере кода определяется метод **GetUsersUsingKerberos** , который создает пространства выполнения Командная консоль Exchange на удаленном сервере с использованием проверки подлинности Kerberos.</span><span class="sxs-lookup"><span data-stu-id="13eba-166">The following code example defines the **GetUsersUsingKerberos** method, which creates an Exchange Management Shell runspace on a remote server by using Kerberos authentication.</span></span> <span data-ttu-id="13eba-167">Метод затем вызывает метод **GetUserInformation** , как определено в раздел, [Ознакомьтесь со списком пользователей почтовых ящиков из удаленного пространства выполнения](#bk_remote), чтобы получить список пользователей на удаленном сервере.</span><span class="sxs-lookup"><span data-stu-id="13eba-167">The method then calls the **GetUserInformation** method, as defined in the section [Get a list of mailbox users from a remote runspace](#bk_remote), to return a list of users on the remote server.</span></span>
  
<span data-ttu-id="13eba-168">Для этого метода требуются следующие параметры:</span><span class="sxs-lookup"><span data-stu-id="13eba-168">This method requires the following parameters:</span></span>
  
- <span data-ttu-id="13eba-169">**kerberosUri** &ndash; Строка, содержащая URI сервера Kerberos, который будет выполнять проверку подлинности приложения.</span><span class="sxs-lookup"><span data-stu-id="13eba-169">**kerberosUri** &ndash; A string that contains the URI of the Kerberos server that will authenticate the application.</span></span> <span data-ttu-id="13eba-170">URI будет одно из перечисленных в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="13eba-170">The URI will be one of those listed in the following table.</span></span> 
    
    <span data-ttu-id="13eba-171">**В таблице 2. kerberosUri коды URI**</span><span class="sxs-lookup"><span data-stu-id="13eba-171">**Table 2. kerberosUri URIs**</span></span>

    |<span data-ttu-id="13eba-172">**Сервер**</span><span class="sxs-lookup"><span data-stu-id="13eba-172">**Server**</span></span>|<span data-ttu-id="13eba-173">**Универсальный код ресурса (URI)**</span><span class="sxs-lookup"><span data-stu-id="13eba-173">**URI**</span></span>|
    |:-----|:-----|
    |<span data-ttu-id="13eba-174">Сервер Exchange, не использующий протокол SSL</span><span class="sxs-lookup"><span data-stu-id="13eba-174">Exchange server without using SSL</span></span>  <br/> |`http://<servername>/PowerShell`  <br/> |
    |<span data-ttu-id="13eba-175">Сервер Exchange, использующий протокол SSL</span><span class="sxs-lookup"><span data-stu-id="13eba-175">Exchange server using SSL</span></span>  <br/> |`https://<servername>/PowerShell`  <br/> |
   
- <span data-ttu-id="13eba-176">**schemaUri** &ndash; Строка, содержащая URI документа схемы, который определяет схему Командная консоль Exchange.</span><span class="sxs-lookup"><span data-stu-id="13eba-176">**schemaUri** &ndash; A string that contains the URI of the schema document that defines the Exchange Management Shell schema.</span></span> <span data-ttu-id="13eba-177">Схема URI — это http://schemas.microsoft.com/powershell/Microsoft.Exchange.</span><span class="sxs-lookup"><span data-stu-id="13eba-177">The schema URI is http://schemas.microsoft.com/powershell/Microsoft.Exchange.</span></span> 
    
- <span data-ttu-id="13eba-178">**учетные данные** &ndash; Объект [PSCredential](http://msdn.microsoft.com/en-us/library/system.management.automation.pscredential%28VS.85%29.aspx) , содержащий учетные данные пользователя, который выполняется приложение.</span><span class="sxs-lookup"><span data-stu-id="13eba-178">**credentials** &ndash; A [PSCredential](http://msdn.microsoft.com/en-us/library/system.management.automation.pscredential%28VS.85%29.aspx) object that contains the credentials of the user who is running the application.</span></span> 
    
- <span data-ttu-id="13eba-179">**Count** &ndash; Число пользователей почтовых ящиков Exchange для возврата.</span><span class="sxs-lookup"><span data-stu-id="13eba-179">**count** &ndash; The number of Exchange mailbox users to return.</span></span> 
    
```cs
public Collection<PSObject> GetUsersUsingKerberos(
    string kerberosUri, string schemaUri, PSCredential credentials, int count)
{
    WSManConnectionInfo connectionInfo = new WSManConnectionInfo(
        new Uri(kerberosUri),
        schemaUri, credentials);
    connectionInfo.AuthenticationMechanism = AuthenticationMechanism.Kerberos;
    using (Runspace runspace = RunspaceFactory.CreateRunspace(connectionInfo))
    {
        return GetUserInformation(count, runspace);
    }
}
```

```vb
  Function GetUsersUsingKerberos( _
    ByVal KerberosUri As String, ByVal ScehmaUri As String, _
    ByVal Credentials As PSCredential, ByVal Count As Integer) As Collection(Of PSObject)
    Dim ConnectionInfo As WSManConnectionInfo = _
        New WSManConnectionInfo(New Uri(KerberosUri), ScehmaUri, Credentials)
    ConnectionInfo.AuthenticationMechanism = AuthenticationMechanism.Kerberos
    Dim RemoteRunspace As Runspace
    RemoteRunspace = RunspaceFactory.CreateRunspace(ConnectionInfo)
    Return GetUserInformation(Count, RemoteRunspace)
  End Function

```

<span data-ttu-id="13eba-180"><a name="bk_remote"> </a></span><span class="sxs-lookup"><span data-stu-id="13eba-180"></span></span>

## <a name="get-a-list-of-mailbox-users-from-a-remote-runspace"></a><span data-ttu-id="13eba-181">Получение списка пользователей почтового ящика из удаленного пространства</span><span class="sxs-lookup"><span data-stu-id="13eba-181">Get a list of mailbox users from a remote runspace</span></span>

<span data-ttu-id="13eba-182">В следующем примере кода определяется метод **GetUserInformation** , который возвращает коллекцию экземпляров [PSObject](http://msdn.microsoft.com/en-us/library/system.management.automation.pscredential%28VS.85%29.aspx) , которые представляют почтовых ящиков пользователей Exchange.</span><span class="sxs-lookup"><span data-stu-id="13eba-182">The following code example defines the **GetUserInformation** method, which returns a collection of [PSObject](http://msdn.microsoft.com/en-us/library/system.management.automation.pscredential%28VS.85%29.aspx) instances that represent Exchange mailbox users.</span></span> <span data-ttu-id="13eba-183">Этот метод вызывается с помощью методов **GetUsersUsingBasicAuth**, **GetUsersUsingCertificate**и **GetUsersUsingKerberos** для возвращения списка пользователей с удаленного сервера.</span><span class="sxs-lookup"><span data-stu-id="13eba-183">This method is called by the **GetUsersUsingBasicAuth**, **GetUsersUsingCertificate**, and **GetUsersUsingKerberos** methods to return the list of users from the remote server.</span></span> 
  
<span data-ttu-id="13eba-184">Для этого метода требуются следующие параметры:</span><span class="sxs-lookup"><span data-stu-id="13eba-184">This method requires the following parameters:</span></span>
  
- <span data-ttu-id="13eba-185">**Count** &ndash; Число пользователей почтовых ящиков Exchange для возврата.</span><span class="sxs-lookup"><span data-stu-id="13eba-185">**count** &ndash; The number of Exchange mailbox users to return.</span></span> 
    
- <span data-ttu-id="13eba-186">**пространства выполнения** &ndash; Удаленного пространства выполнения, который указывается для удаленного сервера Exchange.</span><span class="sxs-lookup"><span data-stu-id="13eba-186">**runspace** &ndash; The remote runspace that is established for the remote Exchange server.</span></span> 
    
```cs
public Collection<PSObject> GetUserInformation(int count, Runspace runspace)
{
    using (PowerShell powershell = PowerShell.Create())
    {
        powershell.AddCommand("Get-Users");
        powershell.AddParameter("ResultSize", count);
        runspace.Open();
        powershell.Runspace = runspace;
        return powershell.Invoke();
    }
}
```

```vb
Function GetUserInformation(ByVal Count As Integer, ByVal RemoteRunspace As Runspace) As Collection(Of PSObject)
    Dim RemotePowerShell As PowerShell = PowerShell.Create
    RemotePowerShell.AddCommand("Get-Users")
    RemotePowerShell.AddParameter("ResultSize", Count)
    ' Open the remote runspace on the server.
    RemoteRunspace.Open()
    ' Associate the runspace with the Exchange Management Shell.
    RemotePowerShell.Runspace = RemoteRunspace
    ' Invoke the Exchange Management Shell to run the command.
    Return RemotePowerShell.Invoke
End Function

```

<span data-ttu-id="13eba-187">Метод **GetUserInformation** возвращает не более чем _количество_ почтовых ящиков пользователей.</span><span class="sxs-lookup"><span data-stu-id="13eba-187">The **GetUserInformation** method will return no more than  _count_ mailbox users.</span></span> <span data-ttu-id="13eba-188">Для упрощения кода в данном примере, метод не фильтровать или в противном случае ограничение пользователей почтовых ящиков, которые возвращаются.</span><span class="sxs-lookup"><span data-stu-id="13eba-188">To simplify the code for this example, the method does not filter or otherwise limit the mailbox users that are returned.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="13eba-189">См. также</span><span class="sxs-lookup"><span data-stu-id="13eba-189">See also</span></span>

- [<span data-ttu-id="13eba-190">Создание средств управления Exchange</span><span class="sxs-lookup"><span data-stu-id="13eba-190">Create Exchange Management Shell tools</span></span>](create-exchange-management-shell-tools.md)   
- [<span data-ttu-id="13eba-191">Использование ответа командлет командной консоли Exchange</span><span class="sxs-lookup"><span data-stu-id="13eba-191">Use the Exchange Management Shell cmdlet response</span></span>](how-to-use-the-exchange-management-shell-cmdlet-response.md)
    
