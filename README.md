# Blazor To-do list app:computer:
To-do list app is Blazor Server app, which use in practice:<br/>
- Creation of Blazor app<br/>
- Modify Razor components<br/>
- Use event handling and data binding in components<br/>
- Use routing in a Blazor app<br/>
## How to run To-do list Blazor app
1. Navigate to the folder directory in cmd **cd Thenameofyourapp**
2. Run the app with command **dotnet watch run**
3. The app is now running on **http://localhost:5000**
4. Stop the app by pressing **CTRL + C** in cmd
## The features and purpose
The purpose of this app was to create my first Blazor Server app. I followed [Microsoft tutorial](https://docs.microsoft.com/en-us/aspnet/core/tutorials/build-a-blazor-app?view=aspnetcore-5.0).<br/>
Within this app user can add items, edit items, and mark todo items done.
## Interesting part of the code
### Creation of the app
Before we start to create a Blazor Server app, we have to make sure that we have already installed **.NET 5.0 SDK** or later.<br/>
With the following command, we create folder named TodoList with the -o|--output option to hold the app.
```shell
dotnet new blazorserver -o TodoList
 ```
### Adding components
Inside of TodoList folder, we can add new **Razor component**. Razor components are building blocks of Blazor application, they have extension **.razor** and start with capital letter.<br/>
This is how we created our Todo component.<br/>
```shell
dotnet new razorcomponent -n Todo -o Pages
 ```
 **-n|--name** specifies name of the component
 
### Navmenu
Navmenu it is menu user can see on the screen.
```yml
<ul class="nav flex-column">

    ...

    <li class="nav-item px-3">
        <NavLink class="nav-link" href="todo">
            <span class="oi oi-list-rich" aria-hidden="true"></span> Todo
        </NavLink>
    </li>
</ul>
 ```
 You can see that we added list item **li** and **Navlink compoments**, to unordered list **ul**. Navlink components provides a cue in the UI when the component URL is loaded by app.


