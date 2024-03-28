# Repro Steps
- `cd ./appshell` and run `npm i` and then `npm run build`
- `cd ../Pilet` and run `dotnet build`
- `cd ../piral~/Pilet` and run `pilet debug`

#  Problem
Open `http://localhost:1234/shop`.
The Layout is not shown

# Plain Blazor Example
If you cd into `./BlazorApp` and run `dotnet run`
Youl see the Blazor same App as in `./Pilet`, but now the following layouts are used:
- `.\Features\Blog\Layouts\BlogLayout.razor`
- `.\Features\Shop\Layouts\ShopLayout.razor`

They are used in all pages via the @layout notation.