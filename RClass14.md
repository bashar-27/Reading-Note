##  Navigation Properties and Routing

<h2>Routing within MVC</h2>
In MVC, routing is a process of mapping the browser request to the controller action and return response back.
Each MVC application has default routing for the default HomeController.
We can set custom routing for newly created controller.

```
public class RouteConfig
{
    public static void RegisterRoutes(RouteCollection routes)
    {
        routes.MapRoute(
            name: "Default",
            url: "{controller}/{action}/{id}",
            defaults: new { controller = "Home", action = "Index", id = UrlParameter.Optional }
        );
    }
}

```

<hr>

<h2>Routing within Core</h2>
Routing in ASP.NET Core is the process of mapping incoming requests to application logic that resides in controllers and methods.

ASP.NET Core maps the incoming request based on the routes that you configure in your application, and for each route, you can set specific configurations, 
such as default values, message handlers, constraints, and so on.

* Conventional routing: The route is determined based on conventions that are defined in route templates that, at runtime, will map requests to controllers and actions (methods).
*  Attribute-based routing: The route is determined based on attributes that you set on your controllers and methods. These will define the mapping to the controller’s actions.

 ```
  public class Startup
{
    public void Configure(IApplicationBuilder app)
    {
        app.UseRouting();
        app.UseEndpoints(endpoints =>
        {
            endpoints.MapControllerRoute(
                name: "default",
                pattern: "{controller=Home}/{action=Index}/{id?}");
        });
    }
}
 
   ```
