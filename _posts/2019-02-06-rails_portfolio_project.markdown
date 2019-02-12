---
layout: post
title:      "Rails Portfolio Project"
date:       2019-02-06 13:22:18 -0500
permalink:  rails_portfolio_project
---


Today I start my rails portfolio project. I must admit I am nervous and anxious about what awaits in the coming months.

Like I had originally planned I continued working on my Sinatra Grocery List app but in Rails. I created models for User, Item, List, Store. And the corresponding Join tables. User has many lists and a List belongs to the User.
Store and Items are associated through a StoreItem that has the price offered at the store for that item. As a User, they will be able to login and logout. The User can also use OmniAuth to login using Github. The options for the user are to look at all the lists, all items and all stores.
The user can then create a new List, modify and delete a List. T
