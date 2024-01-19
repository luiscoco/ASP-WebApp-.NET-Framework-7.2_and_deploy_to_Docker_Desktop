# How to create a ASP WebApp .NET Framework 7.2

We run Visual Studio 2022 Community Edition and we create a new project

We select the project template

![image](https://github.com/luiscoco/ASP-WebApp-.NET-Framework-7.2/assets/32194879/66a42969-3cdb-42a1-b6ed-adf974f5d8d9)

We input the location and the project name

![image](https://github.com/luiscoco/ASP-WebApp-.NET-Framework-7.2/assets/32194879/83e3097a-c322-4bb8-b499-7fb48cbf78c8)

We chose the new project main features

![image](https://github.com/luiscoco/ASP-WebApp-.NET-Framework-7.2/assets/32194879/9dff42cd-5778-413e-aef1-cd28a8dbb981)

When we run the application the first file we start is **Global.asax**

```
using System;
using System.Collections.Generic;
using System.Linq;
using System.Web;
using System.Web.Mvc;
using System.Web.Optimization;
using System.Web.Routing;

namespace WebApplication1
{
    public class MvcApplication : System.Web.HttpApplication
    {
        protected void Application_Start()
        {
            AreaRegistration.RegisterAllAreas();
            FilterConfig.RegisterGlobalFilters(GlobalFilters.Filters);
            RouteConfig.RegisterRoutes(RouteTable.Routes);
            BundleConfig.RegisterBundles(BundleTable.Bundles);
        }
    }
}
```
