# React TypeScript Style Guide

## Folder Structure

###  1. Simple Project Folder Structure

```

├───.storybook
├───cypress
├───docker
│   └───nginx.conf
├───public
├───src
│   ├───routes
│   │   └───index.ts
│   │
│   ├───components
│   │   ├───Button
│   │   │   ├───__snapshots__
│   │   │   │   └───Button.test.tsx.snap
│   │   │   └───Button.stories.tsx
│   │   │   └───Button.test.tsx
│   │   │   └───Button.tsx
│   │   │   └───Button.types.ts
│   │   │   └───index.ts
│   │   │   └───styles.css
│   │   │   
│   │   ├───Table
│   │   │   ├───TableRow
│   │   │   │   └───index.ts
│   │   │   ├───TableCell
│   │   │   │   └───index.ts
│   │   │   └───index.ts
│   │   │   
│   │   └───index.ts
│   │
│   ├───containers
│   │   ├───dashboard 
│   │   │   └───index.ts
│   │   │   
│   │   ├───user 
│   │   │   └───index.ts    
│   │   │    
│   │   ├───common
│   │   │   ├───NavBar
│   │   │   │   └───NavBar.tsx
│   │   │   │   └───NavBar.test.tsx
│   │   │   │   └───NavBar.types.ts
│   │   │   │   └───styles.css
│   │   │   │   └───index.ts
│   │   │   └───index.ts
│   │   │   
│   │   └───index.ts  
│   │      
|   ├───pages
│   │   └───DashboardPage.tsx
│   │   └───UsersPage.tsx
│   │   └───index.ts
│   │
│   ├───templates
│   │   └───email-template.html
│   │
│   ├───hooks
│   │   └───custom-hooks.ts 
│   │   └───index.ts   
│   │
|   ├───states
|   │   ├───actions
│   │   │   └───index.ts
│   │   │   
|   │   ├───reducers
│   │   │   └───index.ts
│   │   │   
|   │   ├───store
│   │   │   └───index.ts
│   │   │   
│   │   └───index.ts 
│   │
│   ├───models
│   │   └───user.ts
│   │   └───dashboard.ts  
│   │   └───common.ts    
│   │   └───index.ts
│   │
|   ├───usecases
|   │   ├───users
│   │   │   └───add.ts
│   │   │   └───edit.ts
│   │   │   └───delete.ts
│   │   │   └───fetch-all.ts
│   │   │   └───userSlice.ts
│   │   │   └───index.ts
│   │   │   
|   │   ├───dashboard
│   │   │   └───index.ts
│   │   │   
│   │   └───index.ts
│   │
|   ├───services
│   │   └───UserService.ts
│   │   └───DashboardService.ts
│   │   └───index.ts
│   │
|   ├───utils
|   │   ├───constants
│   │   │   └───user.ts
│   │   │   └───dashboard.ts
│   │   │   └───index.ts
│   │   │   
|   │   ├───user
│   │   │   └───index.ts
│   │   │   
|   │   ├───dashboard
│   │   │   └───index.ts
│   │   │   
|   │   ├───common
│   │   │   └───index.ts
│   │   │   
│   │   └───index.ts
│   │
|   ├───core
|   │   ├───errors
│   │   │   └───api-errors.ts
│   │   │   └───index.ts
│   │   │   
|   │   ├───libs
│   │   │   └───axios.ts
│   │   │   └───jsonwebtoken.ts
│   │   │   └───index.ts
│   │   │   
|   │   ├───templates
│   │   │   └───email-template.html
│   │   │   
|   │   ├───utils
│   │   │   └───http.ts
│   │   │   └───websocket.ts
│   │   │   └───date.ts
│   │   │   └───websocket.ts
│   │   │   └───file.ts
│   │   │   └───index.ts
│   │   │   
│   │   └───index.ts
│   └───App.tsx
│   └───main.tsx

```

2. Complex Project Folder Structure

```

├───.storybook
├───cypress
├───docker
│   └───nginx.conf
├───public
├───src
│   ├───routes
│   │   └───index.ts
│   ├───components
│   │   ├───Button
│   │   │   ├───__snapshots__
│   │   │   │   └───Button.test.tsx.snap
│   │   │   └───Button.stories.tsx
│   │   │   └───Button.test.tsx
│   │   │   └───Button.tsx
│   │   │   └───Button.types.ts
│   │   │   └───index.ts
│   │   │   └───styles.css
│   │   ├───Table
│   │   │   ├───TableRow
│   │   │   │   └───index.ts
│   │   │   ├───TableCell
│   │   │   │   └───index.ts
│   │   │   └───index.ts
│   ├───modules
|   │   ├───dashboard
|   │   │   ├───containers
│   │   │   │   ├───dashboard
│   │   │   │   │   ├───Content
│   │   │   │   │   │   └───index.ts  
│   │   │   │   │   └───index.ts
│   │   │   │   ├───dashboard-preview
│   │   │   │   │   ├───Content
│   │   │   │   │   │   └───index.ts  
│   │   │   │   │   └───index.ts       
│   │   │   │   ├───shared
│   │   │   │   │   ├───DashboardBarChart
│   │   │   │   │   │   └───DashboardBarChart.tsx
│   │   │   │   │   │   └───DashboardBarChart.test.tsx
│   │   │   │   │   │   └───DashboardBarChart.types.ts
│   │   │   │   │   │   └───styles.css
│   │   │   │   │   │   └───index.ts
│   │   │   │   │   └───index.ts
|   │   │   ├───pages
│   │   │   │   │   └───Dashboard.tsx
│   │   │   │   │   └───DashboardPreview.tsx
│   │   │   │   │   └───index.ts
|   │   │   ├───usecases
│   │   │   │   └───index.ts
│   │   │   └───index.ts 
|   │   ├───users
|   │   │   ├───containers
│   │   │   │   ├───users
│   │   │   │   │   ├───Content
│   │   │   │   │   │   └───index.ts  
│   │   │   │   │   └───index.ts     
│   │   │   │   ├───shared
│   │   │   │   │   └───index.ts
|   │   │   ├───pages
│   │   │   │   │   └───users.tsx
│   │   │   │   │   └───index.ts
|   │   │   ├───usecases
|   │   │   │   ├───users
│   │   │   │   │   └───add.ts
│   │   │   │   │   └───edit.ts
│   │   │   │   │   └───delete.ts
│   │   │   │   │   └───fetch-all.ts
│   │   │   │   │   └───userSlice.ts
│   │   │   │   │   └───index.ts
│   │   │   │   └───index.ts
│   │   │   └───index.ts
|   │   ├───common
|   │   │   ├───layout
│   │   │   │   ├───NavBar
│   │   │   │   │   └───NavBar.tsx
│   │   │   │   │   └───NavBar.test.tsx
│   │   │   │   │   └───NavBar.types.ts
│   │   │   │   │   └───styles.css
│   │   │   │   │   └───index.ts
│   │   │   │   └───index.ts
│   │   └───index.ts
│   └───index.ts             
│   ├───hooks
│   │   └───custom-hooks.ts 
│   │   └───index.ts  
│   ├───models
│   │   └───common-models.ts  
│   │   └───index.ts  
|   ├───redux
|   │   ├───actions
|   │   ├───reducers
|   │   ├───store
|   ├───utils
|   |   ├───common
│   │   │   └───index.ts
|   |   ├───components
│   │   │   └───index.ts       
|   |   ├───containers
│   │   │   └───index.ts
│   └───App.tsx
│   └───main.tsx

```

### Explanation

#### 1. Routes

#### 2. Components

   - All the base components will be place here.
   - Each component should have a separate folder and all the component related files should be inside that folder.
   - Each component should have a ``` test ``` file.

#### 3. Pages

   - File name should has ``` page ``` suffix.

   - Each route has a specific page.

      ``` /users ``` route will be bound to ``` UsersPage.tsx ``` page file.

   - Each page can have a specific ``` container ``` folder.
      ``` users ``` container folder includes all the container logics of the ``` UsersPage.tsx ```.

#### 4. Containers

   - Each page can have a specific ``` container ``` folder.
      ``` users ``` container folder includes all the container logics of the ``` UsersPage.tsx ```.

#### 5. Hooks

   - All the custom react hooks will be place inside here.


#### 6. States

   - This will contain all the global states of the application.
   - We can use any state management library such as ``` redux ```,  ``` hookstate ``` etc.

#### 7. Models

   - Contains ``` types ``` and ``` dto ``` types.

#### 8. Usecases

#### 9. Services

   - Services is being used inside ``` usecases ```.