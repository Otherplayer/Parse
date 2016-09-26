# Parse

## Parse是专为移动APP服务的云计算平台，它本身提供Restful的service及相关API让app直接访问服务器，进行增删改查数据。

Parse offers a cloud backend service for mobile apps. This lets developers focus on on creating an awesome app and user experience without having to worry about managing server maintenance or infrastructure.

### Users
At the core of many apps, there is a notion of user accounts that lets users access their information in a secure manner. We provide a specialized user class called PFUser that automatically handles much of the functionality required for user account management.

### Sessions
Sessions represent an instance of a user logged into a device. Sessions are automatically created when users log in or sign up. They are automatically deleted when users log out. There is one distinct Session object for each user-installation pair; if a user issues a login request from a device they’re already logged into, that user’s previous Session object for that Installation is automatically deleted. Session objects are stored on Parse in the Session class, and you can view them on the Parse.com Data Browser. We provide a set of APIs to manage Session objects in your app.

### Roles
As your app grows in user-base, you may find yourself needing more coarse-grained control over access to pieces of your data than user-linked ACLs(访问控制列表) can provide. To address this requirement, Parse supports a form of Role-based Access Control. Roles provide a logical way of grouping users with common access privileges to your Parse data. Roles are named objects that contain users and other roles. Any permission granted to a role is implicitly granted to its users as well as to the users of any roles that it contains.

### Files
PFFile lets you store application files in the cloud that would otherwise be too large or cumbersome to fit into a regular PFObject. The most common use case is storing images but you can also use it for documents, videos, music, and any other binary data (up to 10 megabytes).

### GeoPoints

Parse allows you to associate real-world latitude and longitude coordinates with an object. Adding a PFGeoPoint to a PFObject allows queries to take into account the proximity of an object to a reference point. This allows you to easily do things like find out what user is closest to another user or which places are closest to a user.

### Local Datastore
### App Extensions
### Push Notifications
There are two ways to send push notifications using Parse: channels and advanced targeting. 

USING CHANNELS

The simplest way to start sending notifications is using channels. This allows you to use a publisher-subscriber model for sending pushes. Devices start by subscribing to one or more channels, and notifications can later be sent to these subscribers. The channels subscribed to by a given Installation are stored in the channels field of the Installation object.

SUBSCRIBING TO CHANNELS

A channel is identified by a string that starts with a letter and consists of alphanumeric characters, underscores, and dashes. It doesn’t need to be explicitly created before it can be used and each Installation can subscribe to any number of channels at a time.
### ...

