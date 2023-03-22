# Introduction to Persistence with Local Storage

[Local Storage and How To Use It on Websites](https://www.smashingmagazine.com/2010/10/local-storage-and-how-to-use-it/)

The main problem with HTTP as the main transport layer of the Web is that it is **stateless**. This means that when you use an application and then close it, its state will be reset the next time you open it. If you close an application on your desktop and re-open it, its most recent state is restored.

We use local storage to keep a key on the users computer and read it out when the user returns.

The classic way to do this is by using a **cookie**. A cookie is a text file hosted on the user’s computer and connected to the domain that your website runs on.

## What Not To Store In Local Storage

- Sensitive Information like passwods, social, credit card numbers etc because it is not a secure storage mechanism.

- Local storage has limited storage. Not reccomended to store large amounts of data.

## Local Storage Type of Data

Local storage can only store strings. Before any data can be stored as a string it must get converted to a string. We can use **JSON.stringify** and/ or **JSON.parse** to convert.