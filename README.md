# ExpenseTracker
- Implemented robust APIs using Express.js and Node.js, enabling smooth data retrieval and manipulation.
- Ensured secure access to sensitive features by implementing user authentication and authorization mechanisms in this application.

# How to Use 👥 (Features of Application)
- Make an Account (SignUp) for first Time.
- If Already have an account please Login
- Dashboard Shows
- Please Click Add Expense on the Side Nav or on Plus icon to add new expense
- Here You can Add new Expense by providing details
- You can add your new Category if you want by ADD CATEGORY just above there and proceed to SAVE button.
- After getting message save expense now you can check on View Expense / Dashboard.
- You can See your Profile in Profile Option
- Also you can Edit your Name/ Username and SAVE it.
- Logout (Auto Logout in next 1 hour so don't worry 😊 )
- You can check Expense Summary using BAR chart and PIE charts.
- You can also Import Expense in CSV files.📩

# Flowchart
# flowchart
```mermaid

flowchart TD
    Start([Start]) --> Auth{Authentication}
    Auth -->|New User| SignUp[Sign Up]
    Auth -->|Existing User| Login[Login]
    
    SignUp -->|Create Account| Dashboard
    Login -->|Validate Credentials| Dashboard
    
    Dashboard --> NavOptions{Navigation Options}
    
    NavOptions -->|Add Expense| AddExpense[Add New Expense]
    NavOptions -->|View Expenses| ViewExpense[View Expenses]
    NavOptions -->|Expense Summary| ExpenseSummary[Expense Summary]
    NavOptions -->|User Profile| Profile[User Profile]
    NavOptions -->|Logout| Logout[Logout]
    
    AddExpense --> CategoryExists{Category Exists?}
    CategoryExists -->|Yes| FillExpenseDetails[Fill Expense Details]
    CategoryExists -->|No| AddCategory[Add New Category]
    AddCategory --> FillExpenseDetails
    FillExpenseDetails --> SaveExpense[Save Expense]
    SaveExpense --> Dashboard
    
    ViewExpense --> ExpenseActions{Actions}
    ExpenseActions -->|Edit| EditExpense[Edit Expense]
    ExpenseActions -->|Delete| DeleteExpense[Delete Expense]
    ExpenseActions -->|View Details| ExpenseDetails[View Expense Details]
    EditExpense --> SaveExpense
    DeleteExpense --> Dashboard
    ExpenseDetails --> Dashboard
    
    ExpenseSummary --> ChartOptions{Chart Options}
    ChartOptions -->|Bar Chart| BarChart[Bar Chart View]
    ChartOptions -->|Pie Chart| PieChart[Pie Chart View]
    ChartOptions -->|Import CSV| ImportCSV[Import Expenses from CSV]
    BarChart --> Dashboard
    PieChart --> Dashboard
    ImportCSV --> Dashboard
    
    Profile --> ProfileOptions{Profile Options}
    ProfileOptions -->|View Info| ViewProfile[View Profile Info]
    ProfileOptions -->|Edit Info| EditProfile[Edit Profile]
    EditProfile --> SaveProfile[Save Profile Changes]
    ViewProfile --> Dashboard
    SaveProfile --> Dashboard
    
    Logout --> AutoLogout[Auto Logout after 1 hour]
    AutoLogout --> Start
    Logout --> Start
    
    %% Styling
    classDef default fill:#f9f9f9,stroke:#333,stroke-width:1px
    classDef start fill:#6c5ce7,color:white,stroke:#333,stroke-width:1px
    classDef auth fill:#fdcb6e,stroke:#333,stroke-width:1px
    classDef dashboard fill:#00cec9,color:white,stroke:#333,stroke-width:1px
    classDef action fill:#74b9ff,stroke:#333,stroke-width:1px
    classDef expense fill:#55efc4,stroke:#333,stroke-width:1px
    classDef profile fill:#ff7675,color:white,stroke:#333,stroke-width:1px
    classDef logout fill:#d63031,color:white,stroke:#333,stroke-width:1px
    classDef decision fill:#e17055,color:white,stroke:#333,stroke-width:1px
    classDef summary fill:#a29bfe,color:white,stroke:#333,stroke-width:1px
    
    class Start start
    class Auth,CategoryExists,ExpenseActions,ChartOptions,ProfileOptions decision
    class Dashboard,NavOptions dashboard
    class SignUp,Login auth
    class AddExpense,FillExpenseDetails,SaveExpense,EditExpense,DeleteExpense,ExpenseDetails,ViewExpense expense
    class AddCategory action
    class BarChart,PieChart,ImportCSV,ExpenseSummary summary
    class Profile,ViewProfile,EditProfile,SaveProfile profile
    class Logout,AutoLogout logout
```


## Screenshots
# Dashboard - View Expense

![image](https://github.com/grraghav120/expense-tracker/assets/96789493/47943654-8b88-4adb-afd2-2fc2ce7be0a2)


![image](https://github.com/grraghav120/expense-tracker/assets/96789493/16dc906d-8092-441d-9214-12b42d0404d3)


# Home - Add Expense 

![image](https://github.com/grraghav120/expense-tracker/assets/96789493/b8df0bfe-3d86-4666-a6a6-05f40b026471)

![image](https://github.com/grraghav120/expense-tracker/assets/96789493/a8f01ea0-bbc0-4b92-ad0d-470579b96e68)

![image](https://github.com/grraghav120/expense-tracker/assets/96789493/b9cb123f-2def-4864-868b-999d38984348)

# Expense Summary

![image](https://github.com/grraghav120/expense-tracker/assets/96789493/915db7b6-4567-48bb-8147-21787da4d6d0)

![image](https://github.com/grraghav120/expense-tracker/assets/96789493/a5d048f7-2adc-496b-9c4a-af5fdbf221b0)


# Profile - User

![image](https://github.com/grraghav120/expense-tracker/assets/96789493/dae4b7aa-e337-4584-803a-35cb064d1b5a)

Update info

![image](https://github.com/grraghav120/expense-tracker/assets/96789493/eb86dded-17bf-4546-9e7f-b6493370fbea)


# Edit Expense

![image](https://github.com/grraghav120/expense-tracker/assets/96789493/8f0af600-4311-4b63-9aff-95b20de67be4)

![image](https://github.com/grraghav120/expense-tracker/assets/96789493/02d2e634-cd47-4ed5-944d-77467afc6be7)

# View Expense

![image](https://github.com/grraghav120/expense-tracker/assets/96789493/2eb61c22-2b25-4c21-ace6-efb8e836e36a)



# Import CSV File
![image](https://github.com/grraghav120/expense-tracker/assets/96789493/90d27a08-51cb-4b3c-9dc8-843cdcbcee6f)


# Logout
![image](https://github.com/grraghav120/expense-tracker/assets/96789493/04bc9557-aad8-4f5b-8ec1-077fa3262be9)


# Login
![image](https://github.com/grraghav120/expense-tracker/assets/96789493/7de69073-ad13-40a7-8d7e-8f1b3fd3f492)

# SignUp
![image](https://github.com/grraghav120/expense-tracker/assets/96789493/33d3d042-5283-49c9-8a37-e5ee902d967a)

# Logger
![image](https://github.com/grraghav120/expense-tracker/assets/96789493/7e37a242-533a-41fc-b418-430eb77f4746)

# Database

![image](https://github.com/grraghav120/expense-tracker/assets/96789493/b490db8a-d765-4506-af9c-31185646ad2d)



## Development server
- Run `npm i` or `npm install`.
- Download Angular Material `ng add @angular/material`.
- Download Bootstrap `npm install bootstrap`.
- Run `ng serve`
- Navigate to  `http://localhost:4200/`.
- The application will automatically reload if you change any of the source files.

