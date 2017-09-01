---
layout: post
title:  "learning to use sessions in Sinatra Project"
date:   2017-09-01 16:10:21 -0400
---


Sessions and Authentication Coding Process
The learning process of using sessions, and authentication is quite involved. Finally, I would like to elaborate on the project Developement Workflow. 

After completing the labs, I thought I know it; however, when one of the spec in the Sinatra Project presented validation, I find myself re-reviewing the User Authentication Lab. Moreover, I find myself, inquiring about the helper methods of current user and login yesterday? For instance, in the Authentication Video, Avi had used session(:email) while in the helper method session(:user_id) was used instead.  

**Helper methods**:

It is confusing to determine the truthy or falsey outcome of a method without some 1 on 1 tutorial for the ||= operator.  
In the case of Current User and Loggedin? instance methods, we have the following code, which i could not understand.
def logged_in?
    !!current_user
 end
def current_user
   if session[:user_id]
   @current user ||= User.find_by(:id session(:user_id)
   end 
end

Until, Learn raised the IRB session and showed me the following
[12:42:39] (master) swpp $ irb
2.4.0 :001 > nil
 => nil 
2.4.0 :002 > !!nil
 => false 
2.4.0 :003 > [1, 2, 3]
 => [1, 2, 3] 
2.4.0 :004 > !![1, 2, 3]
 => true 
2.4.0 :005 >

Which I then rewrote the current method to Read:   
1)!!Current Operator READS "IF Current User is NIL, THEN logged in? => "FALSE" 
2)!!Current Operator READS "IF Current User is TRUTH, THEN logged in? => "TRUE"

First scenario occurred during the signup method while the second scenario during loggin with the Application Controller. 

**Validation:**

Ever feel like being in GMAT English test when you read the requirement like Include user input validations?  I find myself asking what method is used to perform this requirement, after I read the requirement. So I query the curriculum, and read the following
"Next, we need to check two conditions: first, did we find a user with that username? This can be written as user != nil or simply user...We also need to check if that user's password matches up with the value in password_digest. We can use a method called authenticate" from Securing Passwords in Sinatra. I then realized the code had already been incorporated into the project.
Project Development Workflow
With little skeleton to start the project, Flatiron provided me with corneal gem to start the project, after I had spent 2 days, part time on trying.  Thereafter, I began the development.  
I found an interesting option in bash, multiple tabs. 
I found myself using tab for migration, tux to interact code, shotgun to continuously run the server, model, controller, view, and github repos postings. So in all 7 to 10 bash tabs, and in over next 17-36 hours, while hunkered down from Hurricane Harvey at home, I persisted to write the project. 

**Hurricane Harvey:**

a 800 year flood event, said the local fort bend judge, when announcing the mandatory evacuation order for my subdivision. Evacuating while having a flu is no fun, but I am grateful for others have lost everything, including loved ones. 




