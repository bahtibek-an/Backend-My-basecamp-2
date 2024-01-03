# Welcome to My Basecamp 2

 [Demo]       https://my-basecamp2.fly.dev/

## Task

Backend-My-BaseCamp-2  is a web-based project management tool developed using Ruby on Rails framework. It allows users to:

 create and manage projects, 
 create and manage attachments for each project, 
 view threads under each project, and
 creates and manages messages under each thread.

NOTE: Only admin's are allowed to create and manage threads.

User Registration:
Users can create, view, and delete their accounts.
Attachment:
Users associated with the project can create attachments. 
Attachments can be stored in any format (e.g., png, jpg, pdf, txt) 
and can be displayed on the project#show page.
Session:
Users can log in and log out of their accounts.
Role Permission:
Admin privileges can be granted or removed by an existing admin user.
Project:
Users can create, view, edit, and delete projects. 

 Features User Registration Users can create, view, and delete their accounts.
 Session Users can log in and log out of their accounts.
 Role Permission Admin privileges can be granted or removed by an existing admin user.

 Users can create, view, edit, and delete:

   projects,
   messages within each thread,
   view threads within each project, and
   create, view and delete attachments within each projects.

NOTE: Only Admins can create, edit and delete threads.

## Description

Project:
Users can create, view, edit, and delete projects. 
Thread:
Threads allow project admins to initiate discussions within a project.
Thread#new: Enables project admins to create new threads.
Thread#edit: Allows project admins to edit existing threads.
Thread#destroy: Permits project admins to delete threads.

Inside a Thread
Message:
Users associated with the project can create messages within threads.
Message#new: Allows users to create new messages within a thread.
Message#edit: Allows users to edit their own messages.
Message#destroy: Allows users to delete their own messages.
User Roles and Permissions:
Project Admin: Project admins have exclusive permissions to create threads.
All Users: All users associated with the project can create attachments and post messages in threads.

Users can create, view, edit, and delete:

 projects,
 messages within each thread,
 view threads within each project, and
 create, view and delete attachments within each projects.

NOTE: Only Admins can create, edit and delete threads.

## Installation

 Install Ruby on Rails framework.
 Clone the repository. 
 Navigate to the project directory and install the required gems. 
 Install Ruby on Rails framework.

 $ gem install rails
 $ rails new <my_project_name>
 $ cd <my_project_name>
 $ bunle install
 $ rails db:migrate
 $ rails db:seed
 $ rails server


## Usage

    How to Set First Admin User from console 

    * rails console
    * @last_user = User.last.admin = true
    * @last_user.save

    Note: after admin is set subsequent users can be set from edit on admin panel

   Run server:
    
   bundle install
   rails db:migrate
   rails server
    
  bundle exec puma -C config/puma.rb -b tcp://127.0.0.1:3001

  How to Set First Admin User from console

   rails console
   user = User.find(1)
   user.admin = true
   user.save

   NOTE: after admin is set subsequent users can be set from edit on admin panel or from the sign-up page.
   
   [DEMO]         https://my-basecamp2.fly.dev/
  
   Sign in to the above url as an admin with:
   
   Username:  jenisbozdak@gmail.com
   Password:  0123456789

### The Core Team
 &copy;Jenis Bozdaxov