# .NET Core September 2018 Update

Today, we are releasing the .NET Core September 2018 Update. This update includes [.NET Core 2.1.4 and .NET Core SDK 2.1.402](https://www.microsoft.com/net/download/dotnet-core/2.1#sdk-2.1.402) and contains important reliability fixes.

## Security

[CVE-2018-8409:](https://portal.msrc.microsoft.com/en-us/security-guidance/advisory/CVE-2018-8409) .NET Core Denial Of Service Vulnerability
A denial of service vulnerability exists in .NET Core 2.1 when System.IO.Pipelines improperly handles requests. An attacker who successfully exploited this vulnerability could cause a denial of service against an application that is leveraging System.IO.Pipelines. The vulnerability can be exploited remotely, without authentication. A remote unauthenticated attacker could exploit this vulnerability by providing specially crafted requests to the application.

[CVE-2018-8409:](https://portal.msrc.microsoft.com/en-us/security-guidance/advisory/CVE-2018-8409) ASP.NET Core Denial Of Service Vulnerability
A denial of service vulnerability exists in ASP.NET Core 2.1 that improperly handles web requests. An attacker who successfully exploited this vulnerability could cause a denial of service against an ASP.NET Core web application. The vulnerability can be exploited remotely, without authentication. A remote unauthenticated attacker could exploit this vulnerability by providing a specially crafted web requests to the ASP.NET Core application.

Additional details, such as how to update vulnerable applications, can be found in the [ASP.NET Core](https://github.com/aspnet/Announcements/issues/316) and [.NET Core](https://github.com/dotnet/announcements/issues/83) repo announcements.

## Getting the Update

The latest .NET Core updates are available on the [.NET Core download page](https://www.microsoft.com/net/download/all). This update is also included in the Visual Studio 15.8.4 update, which is also releasing today.

See the [.NET Core 2.1.4 release notes](https://github.com/dotnet/core/blob/master/release-notes/2.1/2.1.4/2.1.4.md) for details on the release including a detailed commit list.

## Docker Images

.NET Docker images have been updated for today’s release. The following repos have been updated.

[microsoft/dotnet](https://hub.docker.com/r/microsoft/dotnet/)
[microsoft/dotnet-samples](https://hub.docker.com/r/microsoft/dotnet-samples/)
[microsoft/aspnetcore](microsoft/aspnetcore)
[microsoft/aspnetcore-build](https://hub.docker.com/r/microsoft/aspnetcore-build/)

**Note:** Look at the “Tags” view in each repository to see the updated Docker image tags.

**Note:** You must re-pull base images in order to get updates. The Docker client does not pull updates automatically.

Azure App Services deployment

Deployment of .NET Core 2.1.4 to Azure App Services has begun and the West Central US region will be live this morning. Remaining regions will be updated over the next few days and deployment progress can be tracked in this [Azure App Service announcement](https://github.com/Azure/app-service-announcements/issues/133).

## Previous .NET Core Updates

The last few .NET Core updates follow:

[August 2018 Update](https://blogs.msdn.microsoft.com/dotnet/2018/08/21/net-core-august-2018-update/)
[July 2018 Update](https://blogs.msdn.microsoft.com/dotnet/2018/07/10/net-core-july-2018-update/)
[June 2018 Update](https://blogs.msdn.microsoft.com/dotnet/2018/06/22/net-core-2-1-june-update/)
[May 2018 Update](https://blogs.msdn.microsoft.com/dotnet/2018/05/08/net-core-may-2018-update/)