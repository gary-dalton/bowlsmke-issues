# Issues for Bowls MKE

Here is where you may report any problems you are having with the site or improvements you would like to see. Understand that this is a brand new application that is coming on line. This means that we would like to see it work error-free but then slowly introduce enhancements.

This does require creating an account, sorry, so that you are able to see the corrective actions being taken and for me to request further info if needed.

Make your reports using the **Issues** tab and click the green _New issue_ button to get started.

# User Testing: Round 1

This should get you started. I will post updates on what it available in the Dashboard for fully paid members , i.e. login as `member@example.com` with `password`.

## Getting email

All email sent by the system is captured locally. This means email verification and all others. In order to see these emails, you will need to visit http://app.milwaukeelawnbowls.com:8025 and login in using mailhog:goodbowls.

## Issues

While using this newly developed application, you may come across bugs, error, things that don't work as expected, or have ideas about improvements. We are interested in hearing these and working on making the user experience better. To help with this, we have a place to put all of your issues. It is on a site called github, which is where IO hold all of my developments. Visit this link, https://github.com/gary-dalton/bowlsmke-issues, to add an issue or see any issues that others have created. Thank you.

## Reset

It is intended that all data will be reset at most every other day. Do not expect any information you enter to persist longer than that.

## Create an account

Please DO create a login and then follow the path through membership and volunteering. There are no email verifications at this point, that will happen as a last step. Remember, all data is reset on a regular basis.

## Fake users

A variety of fake users are generated into the system for testing purposes. This allows you to see how the data and interfaces will look and behave under real conditions. You may make any edits to these users as you would like. They will reset to newly generated fake users on the general reset.

## Special fake users

A number fake users are generated for special cases. These include the following:

    'first_name' => 'Young',
    'last_name' => 'Member',
    'birthdate' => date('Y-m-d',  strtotime('-16 years')),
    'member_since' => 2022,
    membership type' => 'Junior Member',
    'amount_due' => 40.00,
    assignRole('member');
<!-- sep -->
    'first_name' => 'Junia',
    'last_name' => 'Yung',
    'birthdate' => date('Y-m-d',  strtotime('-15 years')),
    'member_since' => 2022,
    membership type' => 'Junior Member',
    'amount_due' => 40.00,
    assignRole('member');
<!-- sep -->
    'first_name' => 'Just',
    'last_name' => 'Starting',
    'member_since' => 2023,
    membership type' => 'New Active Member',
    'amount_due' => 70.00,
    assignRole('member');
<!-- sep -->
    'first_name' => 'Hungry',
    'last_name' => 'Owen',
    'member_since' => 2023,
    membership type' => 'New Active Member',
    'amount_due' => 70.00,
    assignRole('member');
<!-- sep -->
    'first_name' => 'Anton',
    'last_name' => 'Place',
    'member_since' => 2021,
    'club' => 'Liverpool',
    membership type' => 'Associate Member',
    'amount_due' => 100.00,
    assignRole('member');

## Roles
The system is designed to provide only appropriate access to the data, messaging, and forms. This access is done via user roles. We have preliminarily defined the following roles:

    Root

    → Treasurer
    →→ Membership Director

    → Games Administrator
    →→ League Director
    →→Tournament Director

    →→→ Marketing Manager
    →→→ Group Event Manager

    →→ Admin
    →→→→ Member
    →→→→→ User
    →→→→→→ Guest

Root, of necessity, has full access to the system and is usually the person who maintains the code and functioning of the system. The other roles should be self-explanatory.

Not all of these roles have been created and more may be created if needed. The number of arrows roughly indicated the level of access given. Typically, this means ability to view and edit user data and build system resources.

## Demonstration users

Demonstration users are those that you may use to login in different roles to see how the system responds to different role types. You may log in as any of these users using the email address listed and the password, "password". The ones most integrated at this time are, User, Member, Admin, and Root.


    'first_name' => 'Example',
    'last_name' => 'User',
    'email' => 'user@example.com',
<!-- sep -->
    'first_name' => 'Member',
    'last_name' => 'Test',
    'email' => 'member@example.com',
    assignRole('member');
<!-- sep -->
    'first_name' => 'Group',
    'last_name' => 'Event',
    'email' => 'group@example.com',
    assignRole('group-event-manager');
<!-- sep -->
    'first_name' => 'Marketing',
    'last_name' => 'Manager',
    'email' => 'marketing@example.com',
    assignRole('marketing-manager');
<!-- sep -->
    'first_name' => 'Membership',
    'last_name' => 'Director',
    'email' => 'membership@example.com',
    assignRole('membership-director');
    assignRole('admin');
<!-- sep -->
    'first_name' => 'Treasurer',
    'last_name' => 'Person',
    'email' => 'treasurer@example.com',
    assignRole('treasurer');
    assignRole('admin');
<!-- sep -->
    'first_name' => 'Admin',
    'last_name' => 'Person',
    'email' => 'admin@example.com',
    assignRole('admin');
<!-- sep -->
    'first_name' => 'Root',
    'last_name' => 'Super',
    'email' => 'root@example.com',
    assignRole('member');
    assignRole('root');

## Conclusion

This should get you started. I will post updates on what it available in the Dashboard for fully paid members , i.e. login as member@example.com.
