---
layout: page
title: Federated Personalized Scanpath
description: Federated Learning
img: assets/img/3.jpg
importance: 2
category: Development Projects_
giscus_comments: true
---
# Online Market

**Online Market** is an ASP.NET Core MVC-based e-commerce platform inspired by popular online marketplaces like Daraz, Amazon, and Alibaba. It allows multiple sellers to list their products while offering customers a seamless shopping experience. The platform includes features such as product recommendations based on customer activity, secure online transactions, and an intuitive interface for both administrators and users.

## Key Features

### For Customers
- **Product Browsing and Search**: Easily search for and browse products listed by multiple sellers.
- **Add to Cart and Place Orders**: Add products to the cart, review orders, and place purchases.
- **Secure Online Transactions**: Supports online payments through SSLCommerz integration.
- **Product Recommendations**: Personalized product suggestions based on recent searches or trending items.

### For Sellers
- **Product Management**: Sellers can list, edit, and manage their products directly on the platform.

### For Administrators
- **Admin Panel**: 
  - Manage users, sellers, and products.
  - Oversee platform performance and trends.
  - Moderate content to ensure a high-quality customer experience.

### General Features
- **User Accounts**: Supports separate user and admin panels with role-based access.
- **Trending Products**: Highlights popular and trending items for customers.

## Project Structure

uting**: Default routing configured for `Home` controller.

## Project Structure

Controllers: Contains the controllers that handle HTTP requests and responses.
Models: Contains the data models used in the application.
Views: Contains the views for the MVC pattern.
Properties: Contains project properties and configuration files.
wwwroot: Contains static files such as CSS, JavaScript, and images.
Program.cs: The entry point of the application.
Startup.cs: Configures services and the app's request pipeline.
appsettings.json: Configuration settings for the application.

## How to Run

1. Clone this repository:
   ```bash
   git clone https://github.com/mdakilraihaniftee/online-market.git
2. Open the project in Visual Studio.
3. Restore dependencies:
   ```bash
   dotnet restore
4. Build and run the project:
   ```bash
   dotnet run
7. Access the app in your browser at https://localhost:5001 or http://localhost:5000.

## Prerequisites
.NET Core SDK 3.1 or later
Visual Studio 2019 or later with ASP.NET and web development workload installed.

## Key Configurations
Development environment: Set in launchSettings.json under the ASPNETCORE_ENVIRONMENT key.
Routing: Configured in Startup.cs to use the Home controller and Index action by default.

##Technologies Used
- ASP.NET Core MVC
- Bootstrap (CSS framework)
- jQuery (JavaScript library)
