---
title: "Appwrite: All you need to know"
seoTitle: "Appwrite: All you need to know"
seoDescription: "Appwrite is a self-hosted solution that provides developers with a set of easy-to-use and integrate REST APIs to manage their core backend needs."
datePublished: Wed Oct 06 2021 12:14:00 GMT+0000 (Coordinated Universal Time)
cuid: ckufh31tj00myzzs1arskc2lb
slug: appwrite-all-you-need-to-know
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1633522348292/v306UN_HE.png
ogImage: https://cdn.hashnode.com/res/hashnode/image/upload/v1633522407471/IFi6XXRvaw.png
tags: web-development, nodejs, backend, full-stack

---

## What's Appwrite?

Appwrite is a self-hosted solution that provides developers with a set of easy-to-use and integrate REST APIs to manage their core backend needs.

Think of Appwrite as a complete toolkit of APIs and Tools with a management console UI to help you make application faster and more efficiently.

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1633503574623/byK7BSzMb.png)

### What all can Appwrite do?

Appwrite can be your backend, a helping handing at your backend or work alongside your backend.

It's services include authentication and account management, user preferences, database and storage persistence, cloud functions, localization, image manipulation, scheduled background tasks, and more.

Appwrite also has a great community and documentation as a cherry on the top.

### Can I use it with my tech stack?

No matter what technologies you're using Appwrite got you covered with Web, Flutter, Swift, Objective C, Android, Node.js, Deno, PHP, Python, Ruby, Go and Java.

## Appwrite's Features

Appwrite has a lot of features, let's discuss about the a few of the ones that you'll require in almost every project.

### Authentication and Account Management

The account server allows you to create users, authenticate users, manage users, manage user activity logs.

Here are a few examples:

- Creating a account
  ```js
  const sdk = new Appwrite()

  sdk
    .setEndpoint(proccess.env.ENDPOINT).setProject(process.env.PROJECT_ID)

  let promise = sdk.account.create('email@example.com', 'password')

  promise.then(function (response) {
      console.log(response)
  }, function (error) {
      console.log(error)
  })
  ```
- Fetch a account
  ```js
  const sdk = new Appwrite()

  sdk
    .setEndpoint(proccess.env.ENDPOINT).setProject(process.env.PROJECT_ID)

  let promise = sdk.account.create('email@example.com', 'password')

  promise.then(function (response) {
    console.log(response)
  }, function (error) {
    console.log(error)
  })
  ```

- Authenticating the user with password
  ```js
  const sdk = new Appwrite()

  sdk
    .setEndpoint(proccess.env.ENDPOINT).setProject(process.env.PROJECT_ID)

  let promise = sdk.account.createSession('email@example.com', 'password')

  promise.then(function (response) {
    console.log(response)
  }, function (error) {
    console.log(error)
  })
  ```

There's a lot more you can do with it like Oauth2, Magic URL Sessions, JWT Auth, Fetch Account Preferences, Update Accounts, Email verifications and more: https://appwrite.io/docs/client/account

### Database API

The Database API is just like a document-based database something like MongoDB. You can use this API to create, list, fetch, update and delete documents.

Here are a few examples:

- Create document
  ```js
  const sdk = new Appwrite()

  sdk
    .setEndpoint(proccess.env.ENDPOINT).setProject(process.env.PROJECT_ID)

  let promise = sdk.database.createDocument('YOUR_COLLECTION_ID', {})

  promise.then(function (response) {
    console.log(response)
  }, function (error) {
    console.log(error)
  })
  ```
- List Documents
  ```js
  const sdk = new Appwrite()

  sdk
    .setEndpoint(proccess.env.ENDPOINT).setProject(process.env.PROJECT_ID)

   let promise = sdk.database.listDocuments('YOUR_COLLECTION_ID')

  promise.then(function (response) {
    console.log(response)
  }, function (error) {
    console.log(error)
  })
  ```

You can also fetch, update and delete these in a similar way, checkout the docs for more: https://appwrite.io/docs/client/database

### Functions API

Appwrite allows you to create backend functions that are triggered by Appwrite system events or cron jobs.

You can learn more by following their [Cloud Functions tutorial](https://appwrite.io/docs/functions).

You can create, list or fetch executions using this API.

This is the last one I'm covering but, Appwrite also has Teams, Storage, Localization, Avatars and Health APIs

## Installation

At this point of time you might be wondering, how do I install such a cool thing? 

If you use unix

```sh
docker run -it --rm \
    --volume /var/run/docker.sock:/var/run/docker.sock \
    --volume "$(pwd)"/appwrite:/usr/src/code/appwrite:rw \
    --entrypoint="install" \
    appwrite/appwrite:0.10.4
```

If you use windows:

```sh
docker run -it --rm ^
    --volume //var/run/docker.sock:/var/run/docker.sock ^
    --volume "%cd%"/appwrite:/usr/src/code/appwrite:rw ^
    --entrypoint="install" ^
    appwrite/appwrite:0.10.4
```

## 30DaysOfAppwrite

If you are familiar with things like 100DaysOfCode, you might have understood this till now. It's all about learning Appwrite in 30Days by making projects. I am also starting to do this and I recommend to you to: https://30days.appwrite.io/

## Demos

If you are still not sure, here's a list of projects made using appwrite: https://github.com/appwrite/awesome-appwrite#showcase-built-with-appwrite-

## Support

If you need any help, feel free to ask the doubt in the comments or ask the appwrite community in their discord server: https://discord.gg/GSeTUeA