---
title: Получение списка пользователей почты с помощью командной консоли Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8b790dc8-5c4f-4acf-bbe7-63523395fbe7
description: Использование командлетов командной консоли Exchange для создания инструмента, который возвращает список пользователей почтового ящика Exchange
ms.openlocfilehash: e9493571e98760e5a11674db9a552111c1ec29b2
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354003"
---
# <a name="get-a-list-of-mail-users-by-using-the-exchange-management-shell"></a><span data-ttu-id="433d0-103">Получение списка пользователей почты с помощью командной консоли Exchange</span><span class="sxs-lookup"><span data-stu-id="433d0-103">Get a list of mail users by using the Exchange Management Shell</span></span>

<span data-ttu-id="433d0-104">Использование командлетов командной консоли Exchange для создания инструмента, который возвращает список пользователей почтового ящика Exchange</span><span class="sxs-lookup"><span data-stu-id="433d0-104">Learn how to use Exchange Management Shell cmdlets to create a tool that returns a list of Exchange mailbox users.</span></span>
  
<span data-ttu-id="433d0-105">**Применимо к:** Exchange Online | Exchange Server 2013 | Office 365</span><span class="sxs-lookup"><span data-stu-id="433d0-105">**Applies to:** Exchange Online | Exchange Server 2013 | Office 365</span></span> 
  
<span data-ttu-id="433d0-106">Получение списка пользователей из Exchange Online, Exchange Online в составе Office 365 или версий Exchange начиная с Exchange 2013 с помощью управляемого инструмента для вызова командлета командной консоли Exchange — это двухэтапный процесс.</span><span class="sxs-lookup"><span data-stu-id="433d0-106">Getting a list of users from Exchange Online, Exchange Online as part of Office 365, or a version of Exchange starting with Exchange 2013 by using a managed tool that calls an Exchange Management Shell cmdlet is a two-step process.</span></span> <span data-ttu-id="433d0-107">Сначала необходимо создать удаленное пространство выполнения на сервере Exchange, а затем запустить командлет для получения сведений о пользователях в удаленном пространстве выполнения.</span><span class="sxs-lookup"><span data-stu-id="433d0-107">First, you establish a remote runspace on an Exchange server; then, you run the cmdlet to retrieve the user information in the remote runspace.</span></span> 

<span data-ttu-id="433d0-108">Для подключения к удаленному пространству выполнения необходимо пройти проверку подлинности на сервере Exchange согласно схеме, принятой в соответствии с требованиями безопасности вашей организации.</span><span class="sxs-lookup"><span data-stu-id="433d0-108">To connect to the remote runspace, you have to authenticate with the Exchange server by using the authentication scheme that meets the security requirements of your organization.</span></span> 

<span data-ttu-id="433d0-109">В этой статье приведены примеры кодов, которые можно использовать для создания удаленного пространства выполнения, запуска командлета командной консоли Exchange и получения списка пользователей с сервера Exchange.</span><span class="sxs-lookup"><span data-stu-id="433d0-109">This article provides code examples that you can use to set up a remote runspace and run an Exchange Management Shell cmdlet to get a list of users from an Exchange server.</span></span>

<span data-ttu-id="433d0-110"><a name="bk_prerequisites"> </a></span><span class="sxs-lookup"><span data-stu-id="433d0-110"><a name="bk_prerequisites"> </a></span></span>

## <a name="prerequisites-for-getting-a-list-of-mailbox-users"></a><span data-ttu-id="433d0-111">Необходимые условия для получения списка пользователей почтового ящика</span><span class="sxs-lookup"><span data-stu-id="433d0-111">Prerequisites for getting a list of mailbox users</span></span>

<span data-ttu-id="433d0-112">Для выполнения этой задачи требуется ссылка на следующие пространства имен:</span><span class="sxs-lookup"><span data-stu-id="433d0-112">To perform this task, you need a reference to the following namespaces:</span></span>
  
- <span data-ttu-id="433d0-113">**System. Collections. ObjectModel**</span><span class="sxs-lookup"><span data-stu-id="433d0-113">**System.Collections.ObjectModel**</span></span>
- <span data-ttu-id="433d0-114">**System. Management. Automation**</span><span class="sxs-lookup"><span data-stu-id="433d0-114">**System.Management.Automation**</span></span>
- <span data-ttu-id="433d0-115">**System. Management. Automation. Remoting**</span><span class="sxs-lookup"><span data-stu-id="433d0-115">**System.Management.Automation.Remoting**</span></span>
- <span data-ttu-id="433d0-116">**System. Management. Automation. пространства**</span><span class="sxs-lookup"><span data-stu-id="433d0-116">**System.Management.Automation.Runspaces**</span></span>
    
> [!NOTE]
>  <span data-ttu-id="433d0-p102">При создании приложения с помощью Visual Studio необходимо добавить к проекту ссылку на сборку System.Management.Automation.dll. Найти сборку можно, пройдя по одной из следующих ссылок:</span><span class="sxs-lookup"><span data-stu-id="433d0-p102">When you are using Visual Studio to create an application, you must add a reference to the System.Management.Automation.dll assembly to the project. The assembly can be found in one of the following locations:</span></span>
> - <span data-ttu-id="433d0-119">Для ОС Windows XP и Windows Vista — каталог установки Windows PowerShell ($PSHOME).</span><span class="sxs-lookup"><span data-stu-id="433d0-119">For Windows XP and Windows Vista operating systems, the Windows PowerShell installation directory ($PSHOME).</span></span>
> - <span data-ttu-id="433d0-120">Для ОС Windows 7 и Windows 8 — папка Windows\assembly\GAC_MSIL\System.Management.Automation.</span><span class="sxs-lookup"><span data-stu-id="433d0-120">For the Windows 7 and Windows 8 operating systems, the following folder: Windows\assembly\GAC_MSIL\System.Management.Automation.</span></span> 
  
<span data-ttu-id="433d0-121">Не загружайте оснастку управления Exchange 2013 в пространство выполнения на компьютерах, где запущены приложения, автоматизирующие командлеты командной консоли Exchange.</span><span class="sxs-lookup"><span data-stu-id="433d0-121">Do not load the Exchange 2013 Management snap-in into the runspace on computers that are running applications that automate Exchange Management Shell cmdlets.</span></span> <span data-ttu-id="433d0-122">Вместо этого приложение должно создать удаленное пространство выполнения так, как будет описано ниже.</span><span class="sxs-lookup"><span data-stu-id="433d0-122">The application should instead create a remote runspace, as described later in this article.</span></span>

<span data-ttu-id="433d0-123"><a name="bk_gettinglistmailbox"> </a></span><span class="sxs-lookup"><span data-stu-id="433d0-123"><a name="bk_gettinglistmailbox"> </a></span></span>

## <a name="connect-to-a-remote-runspace-on-an-exchange-server"></a><span data-ttu-id="433d0-124">Создание удаленного пространства выполнения на сервере Exchange</span><span class="sxs-lookup"><span data-stu-id="433d0-124">Connect to a remote runspace on an Exchange server</span></span>

<span data-ttu-id="433d0-p104">Метод подключения к удаленному пространству выполнения, в котором будет использован командлет командной консоли Exchange, зависит от выбранной схемы проверки подлинности. В этом разделе приведены примеры кодов для подключения к удаленному пространству выполнения при использовании одного из методов проверки подлинности, перечисленных в таблице ниже.</span><span class="sxs-lookup"><span data-stu-id="433d0-p104">The method that you use to connect to a remote runspace to use an Exchange Management Shell cmdlet varies based on the authentication scheme that you are using. This section provides code examples that show how to connect to a remote runspace when you are using an authentication method listed in the following table.</span></span>
  
|<span data-ttu-id="433d0-127">**Метод проверки подлинности**</span><span class="sxs-lookup"><span data-stu-id="433d0-127">**Authentication method**</span></span>|<span data-ttu-id="433d0-128">**Относится к**</span><span class="sxs-lookup"><span data-stu-id="433d0-128">**Applies to**</span></span>|<span data-ttu-id="433d0-129">**URI**</span><span class="sxs-lookup"><span data-stu-id="433d0-129">**URI**</span></span>|
|:-----|:-----|:-----|
|[<span data-ttu-id="433d0-130">Подключение к удаленному пространству выполнения на сервере Exchange Online с помощью обычной проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="433d0-130">Connect to a remote runspace on Exchange Online by using basic authentication</span></span>](#bk_basic) <br/> |<span data-ttu-id="433d0-131">Серверы Exchange Online</span><span class="sxs-lookup"><span data-stu-id="433d0-131">Exchange Online servers</span></span>  <br/> |`https://outlook.office365.com/PowerShell-LiveID`<br/><br/>`https://<server>/PowerShell-LiveID`  <br/> |
|[<span data-ttu-id="433d0-132">Подключение к удаленному пространству выполнения с помощью проверки подлинности на основе сертификата</span><span class="sxs-lookup"><span data-stu-id="433d0-132">Connect to a remote runspace by using certificate authentication</span></span>](#bk_cert) <br/> |<span data-ttu-id="433d0-133">Серверы Exchange Online и локальные серверы Exchange</span><span class="sxs-lookup"><span data-stu-id="433d0-133">Exchange Online and Exchange on-premises servers</span></span>  <br/> |`https://outlook.office365.com/PowerShell`<br/><br/>`https://<server>/PowerShell`<br/><br/>`http://<server>/PowerShell`  <br/> |
|[<span data-ttu-id="433d0-134">Подключение к удаленному пространству выполнения на сервере Exchange с помощью проверки подлинности Kerberos</span><span class="sxs-lookup"><span data-stu-id="433d0-134">Connect to a remote runspace on an Exchange server by using Kerberos authentication</span></span>](#bk_Kerberos) <br/> |<span data-ttu-id="433d0-135">Серверы Exchange Online и локальные серверы Exchange</span><span class="sxs-lookup"><span data-stu-id="433d0-135">Exchange Online and Exchange on-premises servers</span></span>  <br/> |`https://<server>/PowerShell`<br/><br/>`http://<server>/PowerShell`  <br/> |

<span data-ttu-id="433d0-136"><a name="bk_basic"> </a></span><span class="sxs-lookup"><span data-stu-id="433d0-136"><a name="bk_basic"> </a></span></span>

### <a name="connect-to-a-remote-runspace-on-exchange-online-by-using-basic-authentication"></a><span data-ttu-id="433d0-137">Подключение к удаленному пространству выполнения на сервере Exchange Online с помощью обычной проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="433d0-137">Connect to a remote runspace on Exchange Online by using basic authentication</span></span>

<span data-ttu-id="433d0-138">Следующий код определяет метод **GetUsersUsingBasicAuth**, с помощью которого на удаленном сервере Exchange Online создается пространство выполнения для командной консоли Exchange с помощью обычной проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="433d0-138">The following code example defines the **GetUsersUsingBasicAuth** method, which creates an Exchange Management Shell runspace on a remote Exchange Online server by using basic authentication.</span></span> <span data-ttu-id="433d0-139">Затем этот метод вызывает **GetUserInformation**, как это описано в разделе [Получение списка пользователей почтового ящика из удаленного пространства](#bk_remote), для возврата списка пользователей на удаленном сервере.</span><span class="sxs-lookup"><span data-stu-id="433d0-139">The method then calls the **GetUserInformation** method, as defined in the section [Get a list of mailbox users from a remote runspace](#bk_remote), to return a list of users on the remote server.</span></span>
  
<span data-ttu-id="433d0-140">Для этого метода требуются следующие параметры:</span><span class="sxs-lookup"><span data-stu-id="433d0-140">This method requires the following parameters:</span></span>
  
-  <span data-ttu-id="433d0-141">**ливеидконнектионури** &ndash; строка, содержащая URI сервера Exchange Online, который будет выполнять проверку подлинности приложения.</span><span class="sxs-lookup"><span data-stu-id="433d0-141">**liveIDConnectionUri** &ndash; A string that contains the URI of the Exchange Online server that will authenticate the application.</span></span> <span data-ttu-id="433d0-142">Если Exchange Online работает в Office 365, URI имеет `https://outlook.office365.com/PowerShell-LiveID`значение; в противном случае URI `https://<servername>/PowerShell-LiveID`—.</span><span class="sxs-lookup"><span data-stu-id="433d0-142">If Exchange Online is running in Office 365, the URI is `https://outlook.office365.com/PowerShell-LiveID`; otherwise, the URI is `https://<servername>/PowerShell-LiveID`.</span></span> 
    
-  <span data-ttu-id="433d0-143">**счемаури** &ndash; строка, содержащая URI документа схемы, который определяет схему командной консоли Exchange.</span><span class="sxs-lookup"><span data-stu-id="433d0-143">**schemaUri** &ndash; A string that contains the URI of the schema document that defines the Exchange Management Shell schema.</span></span> <span data-ttu-id="433d0-144">URI схемы `http://schemas.microsoft.com/powershell/Microsoft.Exchange`.</span><span class="sxs-lookup"><span data-stu-id="433d0-144">The schema URI is `http://schemas.microsoft.com/powershell/Microsoft.Exchange`.</span></span> 
    
-  <span data-ttu-id="433d0-145">**Credentials** &ndash; объект [PSCredential](http://msdn.microsoft.com/en-us/library/system.management.automation.pscredential%28VS.85%29.aspx) , содержащий учетные данные пользователя, запустившего приложение.</span><span class="sxs-lookup"><span data-stu-id="433d0-145">**credentials** &ndash; A [PSCredential](http://msdn.microsoft.com/en-us/library/system.management.automation.pscredential%28VS.85%29.aspx) object that contains the credentials of the user who is running the application.</span></span> 
    
-  <span data-ttu-id="433d0-146">**подсчитайте** &ndash; количество возвращаемых пользователей почтовых ящиков Exchange.</span><span class="sxs-lookup"><span data-stu-id="433d0-146">**count** &ndash; The number of Exchange mailbox users to return.</span></span> 
    
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

<span data-ttu-id="433d0-147"><a name="bk_cert"> </a></span><span class="sxs-lookup"><span data-stu-id="433d0-147"><a name="bk_cert"> </a></span></span>

### <a name="connect-to-a-remote-runspace-by-using-certificate-authentication"></a><span data-ttu-id="433d0-148">Подключение к удаленному пространству выполнения с помощью проверки подлинности на основе сертификата</span><span class="sxs-lookup"><span data-stu-id="433d0-148">Connect to a remote runspace by using certificate authentication</span></span>

<span data-ttu-id="433d0-149">Следующий код определяет метод **GetUsersUsingCertificate**, с помощью которого на удаленном сервере Exchange Online создается пространство выполнения для командной консоли Exchange с помощью проверки подлинности на основе сертификата.</span><span class="sxs-lookup"><span data-stu-id="433d0-149">The following code example defines the **GetUsersUsingCertificate** method, which creates an Exchange Management Shell runspace on a remote server by using a certificate.</span></span> <span data-ttu-id="433d0-150">Затем этот метод вызывает **GetUserInformation**, как это описано в разделе [Получение списка пользователей почтового ящика из удаленного пространства](#bk_remote), для возврата списка пользователей на удаленном сервере.</span><span class="sxs-lookup"><span data-stu-id="433d0-150">The method then calls the **GetUserInformation** method, as defined in the section [Get a list of mailbox users from a remote runspace](#bk_remote), to return a list of users on the remote server.</span></span>
  
<span data-ttu-id="433d0-151">Для этого метода требуются следующие параметры:</span><span class="sxs-lookup"><span data-stu-id="433d0-151">This method requires the following parameters:</span></span>
  
-  <span data-ttu-id="433d0-152">**Thumbprint** &ndash; строка, содержащая отпечаток сертификата, используемого для проверки подлинности приложения.</span><span class="sxs-lookup"><span data-stu-id="433d0-152">**thumbprint** &ndash; A string that contains the thumbprint of the certificate that is used to authenticate the application.</span></span> 
    
-  <span data-ttu-id="433d0-153">**цертконнектионури** &ndash; строка, содержащая URI сервера, который будет выполнять проверку подлинности сертификата.</span><span class="sxs-lookup"><span data-stu-id="433d0-153">**certConnectionUri** &ndash; A string that contains the URI of the server that will authenticate the certificate.</span></span> <span data-ttu-id="433d0-154">Необходимо использовать один из универсальных кодов, приведенных в таблице ниже.</span><span class="sxs-lookup"><span data-stu-id="433d0-154">The URI will be one of those listed in the following table.</span></span> 
    
    <span data-ttu-id="433d0-155">**Таблица 1. URI Цертконнектионури**</span><span class="sxs-lookup"><span data-stu-id="433d0-155">**Table 1. certConnectionUri URIs**</span></span>

    |<span data-ttu-id="433d0-156">**Server**</span><span class="sxs-lookup"><span data-stu-id="433d0-156">**Server**</span></span>|<span data-ttu-id="433d0-157">**URI**</span><span class="sxs-lookup"><span data-stu-id="433d0-157">**URI**</span></span>|
    |:-----|:-----|
    |<span data-ttu-id="433d0-158">Сервер Exchange, не использующий протокол SSL</span><span class="sxs-lookup"><span data-stu-id="433d0-158">Exchange server without using SSL</span></span>  <br/> |`http://<servername>/PowerShell`  <br/> |
    |<span data-ttu-id="433d0-159">Сервер Exchange, использующий протокол SSL</span><span class="sxs-lookup"><span data-stu-id="433d0-159">Exchange server using SSL</span></span>  <br/> |`https://<servername>/PowerShell`  <br/> |
    |<span data-ttu-id="433d0-160">Exchange Online в составе Office 365</span><span class="sxs-lookup"><span data-stu-id="433d0-160">Exchange Online as part of Office 365</span></span>  <br/> |`https://outlook.office365.com/PowerShell`  <br/> |
   
- <span data-ttu-id="433d0-161">**счемаури** &ndash; строка, содержащая URI документа схемы, который определяет схему командной консоли Exchange.</span><span class="sxs-lookup"><span data-stu-id="433d0-161">**schemaUri** &ndash; A string that contains the URI of the schema document that defines the Exchange Management Shell schema.</span></span> <span data-ttu-id="433d0-162">URI схемы http://schemas.microsoft.com/powershell/Microsoft.Exchange.</span><span class="sxs-lookup"><span data-stu-id="433d0-162">The schema URI is http://schemas.microsoft.com/powershell/Microsoft.Exchange.</span></span> 
    
- <span data-ttu-id="433d0-163">**подсчитайте** &ndash; количество возвращаемых пользователей почтовых ящиков Exchange.</span><span class="sxs-lookup"><span data-stu-id="433d0-163">**count** &ndash; The number of Exchange mailbox users to return.</span></span> 
    
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

<span data-ttu-id="433d0-164"><a name="bk_Kerberos"> </a></span><span class="sxs-lookup"><span data-stu-id="433d0-164"><a name="bk_Kerberos"> </a></span></span>

### <a name="connect-to-a-remote-runspace-on-an-exchange-server-by-using-kerberos-authentication"></a><span data-ttu-id="433d0-165">Подключение к удаленному пространству выполнения на сервере Exchange с помощью проверки подлинности Kerberos</span><span class="sxs-lookup"><span data-stu-id="433d0-165">Connect to a remote runspace on an Exchange server by using Kerberos authentication</span></span>

<span data-ttu-id="433d0-166">Следующий код определяет метод **GetUsersUsingKerberos**, с помощью которого на удаленном сервере создается пространство выполнения для командной консоли Exchange с помощью проверки подлинности Kerberos.</span><span class="sxs-lookup"><span data-stu-id="433d0-166">The following code example defines the **GetUsersUsingKerberos** method, which creates an Exchange Management Shell runspace on a remote server by using Kerberos authentication.</span></span> <span data-ttu-id="433d0-167">Затем этот метод вызывает **GetUserInformation**, как это описано в разделе [Получение списка пользователей почтового ящика из удаленного пространства](#bk_remote), для возврата списка пользователей на удаленном сервере.</span><span class="sxs-lookup"><span data-stu-id="433d0-167">The method then calls the **GetUserInformation** method, as defined in the section [Get a list of mailbox users from a remote runspace](#bk_remote), to return a list of users on the remote server.</span></span>
  
<span data-ttu-id="433d0-168">Для этого метода требуются следующие параметры:</span><span class="sxs-lookup"><span data-stu-id="433d0-168">This method requires the following parameters:</span></span>
  
- <span data-ttu-id="433d0-169">**керберосури** &ndash; строка, содержащая URI сервера Kerberos, который будет выполнять проверку подлинности для приложения.</span><span class="sxs-lookup"><span data-stu-id="433d0-169">**kerberosUri** &ndash; A string that contains the URI of the Kerberos server that will authenticate the application.</span></span> <span data-ttu-id="433d0-170">Необходимо использовать один из универсальных кодов, приведенных в таблице ниже.</span><span class="sxs-lookup"><span data-stu-id="433d0-170">The URI will be one of those listed in the following table.</span></span> 
    
    <span data-ttu-id="433d0-171">**Таблица 2. URI Керберосури**</span><span class="sxs-lookup"><span data-stu-id="433d0-171">**Table 2. kerberosUri URIs**</span></span>

    |<span data-ttu-id="433d0-172">**Server**</span><span class="sxs-lookup"><span data-stu-id="433d0-172">**Server**</span></span>|<span data-ttu-id="433d0-173">**URI**</span><span class="sxs-lookup"><span data-stu-id="433d0-173">**URI**</span></span>|
    |:-----|:-----|
    |<span data-ttu-id="433d0-174">Сервер Exchange, не использующий протокол SSL</span><span class="sxs-lookup"><span data-stu-id="433d0-174">Exchange server without using SSL</span></span>  <br/> |`http://<servername>/PowerShell`  <br/> |
    |<span data-ttu-id="433d0-175">Сервер Exchange, использующий протокол SSL</span><span class="sxs-lookup"><span data-stu-id="433d0-175">Exchange server using SSL</span></span>  <br/> |`https://<servername>/PowerShell`  <br/> |
   
- <span data-ttu-id="433d0-176">**счемаури** &ndash; строка, содержащая URI документа схемы, который определяет схему командной консоли Exchange.</span><span class="sxs-lookup"><span data-stu-id="433d0-176">**schemaUri** &ndash; A string that contains the URI of the schema document that defines the Exchange Management Shell schema.</span></span> <span data-ttu-id="433d0-177">URI схемы http://schemas.microsoft.com/powershell/Microsoft.Exchange.</span><span class="sxs-lookup"><span data-stu-id="433d0-177">The schema URI is http://schemas.microsoft.com/powershell/Microsoft.Exchange.</span></span> 
    
- <span data-ttu-id="433d0-178">**Credentials** &ndash; объект [PSCredential](http://msdn.microsoft.com/en-us/library/system.management.automation.pscredential%28VS.85%29.aspx) , содержащий учетные данные пользователя, запустившего приложение.</span><span class="sxs-lookup"><span data-stu-id="433d0-178">**credentials** &ndash; A [PSCredential](http://msdn.microsoft.com/en-us/library/system.management.automation.pscredential%28VS.85%29.aspx) object that contains the credentials of the user who is running the application.</span></span> 
    
- <span data-ttu-id="433d0-179">**подсчитайте** &ndash; количество возвращаемых пользователей почтовых ящиков Exchange.</span><span class="sxs-lookup"><span data-stu-id="433d0-179">**count** &ndash; The number of Exchange mailbox users to return.</span></span> 
    
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

<span data-ttu-id="433d0-180"><a name="bk_remote"> </a></span><span class="sxs-lookup"><span data-stu-id="433d0-180"><a name="bk_remote"> </a></span></span>

## <a name="get-a-list-of-mailbox-users-from-a-remote-runspace"></a><span data-ttu-id="433d0-181">Получение списка пользователей почтового ящика из удаленного пространства</span><span class="sxs-lookup"><span data-stu-id="433d0-181">Get a list of mailbox users from a remote runspace</span></span>

<span data-ttu-id="433d0-182">В следующем примере кода определяется метод **жетусеринформатион** , который возвращает коллекцию экземпляров [PSObject](http://msdn.microsoft.com/en-us/library/system.management.automation.pscredential%28VS.85%29.aspx) , представляющих пользователей почтовых ящиков Exchange.</span><span class="sxs-lookup"><span data-stu-id="433d0-182">The following code example defines the **GetUserInformation** method, which returns a collection of [PSObject](http://msdn.microsoft.com/en-us/library/system.management.automation.pscredential%28VS.85%29.aspx) instances that represent Exchange mailbox users.</span></span> <span data-ttu-id="433d0-183">Этот метод вызывается с помощью методов **GetUsersUsingBasicAuth**, **GetUsersUsingCertificate** и **GetUsersUsingKerberos** для возврата списка пользователей на удаленном сервере.</span><span class="sxs-lookup"><span data-stu-id="433d0-183">This method is called by the **GetUsersUsingBasicAuth**, **GetUsersUsingCertificate**, and **GetUsersUsingKerberos** methods to return the list of users from the remote server.</span></span> 
  
<span data-ttu-id="433d0-184">Для этого метода требуются следующие параметры:</span><span class="sxs-lookup"><span data-stu-id="433d0-184">This method requires the following parameters:</span></span>
  
- <span data-ttu-id="433d0-185">**подсчитайте** &ndash; количество возвращаемых пользователей почтовых ящиков Exchange.</span><span class="sxs-lookup"><span data-stu-id="433d0-185">**count** &ndash; The number of Exchange mailbox users to return.</span></span> 
    
- <span data-ttu-id="433d0-186">**пространство выполнения** &ndash; — удаленное пространство выполнения, установленное для удаленного сервера Exchange.</span><span class="sxs-lookup"><span data-stu-id="433d0-186">**runspace** &ndash; The remote runspace that is established for the remote Exchange server.</span></span> 
    
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

<span data-ttu-id="433d0-187">Метод **жетусеринформатион** будет возвращать не больше, чем _количество_ пользователей почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="433d0-187">The **GetUserInformation** method will return no more than  _count_ mailbox users.</span></span> <span data-ttu-id="433d0-188">Чтобы упростить код в этом примере, не выполняется фильтрация либо же другим способом ограничивается количество возвращаемых пользователей.</span><span class="sxs-lookup"><span data-stu-id="433d0-188">To simplify the code for this example, the method does not filter or otherwise limit the mailbox users that are returned.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="433d0-189">См. также</span><span class="sxs-lookup"><span data-stu-id="433d0-189">See also</span></span>

- [<span data-ttu-id="433d0-190">Создание средств командной консоли Exchange</span><span class="sxs-lookup"><span data-stu-id="433d0-190">Create Exchange Management Shell tools</span></span>](create-exchange-management-shell-tools.md)   
- [<span data-ttu-id="433d0-191">Использование ответа командлета командной консоли Exchange</span><span class="sxs-lookup"><span data-stu-id="433d0-191">Use the Exchange Management Shell cmdlet response</span></span>](how-to-use-the-exchange-management-shell-cmdlet-response.md)
    

