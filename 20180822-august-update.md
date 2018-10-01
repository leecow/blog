# .NET Core August 2018 Update

Today, we are releasing the .NET Core August 2018 Update. This update includes [.NET Core 2.1.3 and .NET Core SDK 2.1.401](https://www.microsoft.com/net/download/dotnet-core/2.1#sdk-2.1.401).

## Getting the Update

The latest .NET Core updates are available on the [.NET Core download page](https://www.microsoft.com/net/download/all).

See the [.NET Core 2.1.3 release notes](https://github.com/dotnet/core/blob/master/release-notes/2.1/2.1.3/2.1.3.md) for details on the release including a detailed commit list.

## Docker Images

.NET Docker images have been updated for today’s release. The following repos have been updated.

[microsoft/dotnet](https://hub.docker.com/r/microsoft/dotnet/)
[microsoft/dotnet-samples](https://hub.docker.com/r/microsoft/dotnet-samples/)
[microsoft/aspnetcore](microsoft/aspnetcore)
[microsoft/aspnetcore-build](https://hub.docker.com/r/microsoft/aspnetcore-build/)

**Note:** Look at the “Tags” view in each repository to see the updated Docker image tags.

**Note:** You must re-pull base images in order to get updates. The Docker client does not pull updates automatically.

## 2.1 declared LTS

As mentioned in a [previous blog post](https://blogs.msdn.microsoft.com/dotnet/2018/06/20/net-core-2-0-will-reach-end-of-life-on-september-1-2018/), we have been working toward declaring .NET Core 2.1 as LTS. With the August Update, we're pleased to announce that 2.1.3 begins the .NET Core 2.1 LTS lifecycle. We'll continue to update 2.1 with important fixes to address security and reliability issues as wells as add support for new operating system versions. Details on the .NET Core lifecycle can be seen in the [.NET Core support policy](https://www.microsoft.com/net/support/policy).

### What's covered? 

The LTS designation covers all packages referenced by `Microsoft.NETCore.App` and `Microsoft.AspNetCore.App`. To ensure that applications running on 2.1 remain on the LTS supported updates, it's important to reference these 'meta-packages' rather than individual 'loose' packages. This will enable the applications to properly utilize 2.1 updates when they are released and installed.

The .NET Core SDK is not included as part of the LTS designation. SDK fixes will continue to be released in the lastest version 'train' which supports maintaining and building applicaitons for .NET Core 2.1.

See [.NET Core Supported OS Lifecycle Policy](https://github.com/dotnet/core/blob/master/os-lifecycle-policy.md) to learn about Windows, macOS and Linux versions that are supported for each .NET Core release.


## Previous .NET Core Updates

The last few .NET Core updates follow:

[July 2018 Update](https://blogs.msdn.microsoft.com/dotnet/2018/07/10/net-core-july-2018-update/)
[June 2018 Update](https://blogs.msdn.microsoft.com/dotnet/2018/06/22/net-core-2-1-june-update/)
[May 2018 Update](https://blogs.msdn.microsoft.com/dotnet/2018/05/08/net-core-may-2018-update/)