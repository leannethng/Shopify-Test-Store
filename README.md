# Shopify Test Store

- Testing using themekit to update Shopify themes
- Working with Production and Development Environments
- Testbed to figure out the workflows to update Shopify themes


**Notes:**
- Follow the ThemeKit Getting Started Setup
- The live site can be the Production Environment
- Duplicate the theme and use it's theme id for the Development Environment
- Disable eslint and prettier for the workspace. 
- Open the them to view in the browser
    - `theme open --env=development`
    - Need to manually refresh currently
- 'Watch' the Development Env and test and make edits - all edits get pushed and will modify this theme (The date will not change on the theme page but it is changing files under the hood)
    - `theme watch --env=development`
- Once ready to make live you can 'Deploy' to the Production Env live site
  - `theme deploy -n --env=production ` (`-n` is for nodelete)
  - Or duplicate the theme in the shopify web app, rename then 'publish'.
  
- Use `theme get -p=[your-password] -s=[you-store.myshopify.com] -t=[your-theme-id]` to pull any changes down to your machine, kind of like git pull. 


