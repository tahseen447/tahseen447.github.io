---
layout: post
title:      "Rails Portfolio Project"
date:       2019-02-06 13:22:18 -0500
permalink:  rails_portfolio_project
---


Today I start my rails portfolio project. I must admit I am nervous and anxious about what awaits in the coming months.

Like I had originally planned I continued working on my Sinatra Grocery List app but in Rails. I created models for User, Item, List, Store. And the corresponding Join tables. User has many lists and a List belongs to the User.
Store and Items are associated through a StoreItem that has the price offered at the store for that item. As a User, they will be able to login and logout. The User can also use OmniAuth to login using Github. The options for the user are to look at all the lists, all items and all stores.
The user can then create a new List, modify and delete a List. I am still debating if I should use nested route for creating lists. Doesn't make sense now as  a list is in user's scope anyway. 
Through Stores, new Items can be added which is where I have used nested route for new, show. I think I should add edit probably. May be sometime.  It was interesting to see the issues i faced creating a new nested Item for a store. There is a user attribute "Price" that I required to create a StoreItem. So I used a nested_form using the fields_for tag and was able to navigate through the issue.
Anyhow, I also added scope level methods to display items based on the particular department they're sold under. It was particularly interesting to follow the syntax for scope level methods. 
For stores, I even wrote instance level methods that sorted the items sold in the store based on price and rating.(Rating is a TODO ). After cleaning up my code and adding few routes to view the functionality, I was set for project review. Excited to hear feedback and particularly proud of my work.


