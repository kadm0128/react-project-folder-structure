# React TypeScript Style Guide

### Folder Structure

1. Simple Project Folder Structure

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
│   ├───containers
│   │   ├───dashboard
│   │   │   ├───Content
│   │   │   │   └───index.ts  
│   │   │   └───index.ts     
│   │   ├───shared
│   │   │   ├───NavBar
│   │   │   │   └───NavBar.tsx
│   │   │   │   └───NavBar.test.tsx
│   │   │   │   └───NavBar.types.ts
│   │   │   │   └───styles.css
│   │   │   │   └───index.ts
│   │   │   └───index.ts
│   │   ├───users
│   │   │   └───index.ts        
│   ├───hooks
│   │   └───custom-hooks.ts 
│   │   └───index.ts  
│   ├───models
│   │   └───common-models.ts  
│   │   └───index.ts  
|   ├───pages
│   │   │   └───dashboard.tsx
│   │   │   └───users.tsx
│   │   │   └───index.ts
|   ├───redux
|   │   ├───actions
|   │   ├───reducers
|   │   ├───store
|   ├───usecases
|   │   ├───users
│   │   │   └───add.ts
│   │   │   └───edit.ts
│   │   │   └───delete.ts
│   │   │   └───fetch-all.ts
│   │   │   └───userSlice.ts
│   │   │   └───index.ts
│   │   └───index.ts
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
