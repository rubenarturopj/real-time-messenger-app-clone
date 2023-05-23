### To keep in mind

If you see the following files like a plain text and not dynamically like vscode usually does, then you need to install an extension for vscode called `Prisma`, from Prisma.

# MongoDB, Prisma setup

1. In the terminal run to install Prisma:

```sh
npm install -D prisma
npx prisma init
```

These lines of code will create a folder called `prisma` with the `schema.prisma` inside of it and another file outside called `.env` (environment).

2. Go to `schema.prisma` file and change the provider from `"postgresql"` to `"mongodb"`.

3. For MongoDB, search on google "mongo db altas", log in. Then click on `Build a database`. If you cannot see it in big on the main screen, that's because you need to create a new project first. Then chose `M0` or `free`. You can leave the rest as it is. Click on `create`. On the next screen, create your `username and password`, let's go for `admin/admin` combo. Then click on `create user`. Leave the `Where would you like to connect from` as `My Local Environment`. Next step is to set the `IP address`, you will have already one, but let's better type `0.0.0.0/0` to make sure DB can be accessed from everywhere, press `add entry`. Finally, click `finish and close`, when the pop up appears, click on `go to database`. Now that the database host is done, click on `connect` button. From the options, choose connect with `VSCODE`. Copy the url provided, which looks more or less like this: `mongodb+srv://admin:<password>@cluster0.7awrvea.mongodb.net/test`. It must end with "test"

4. Go to `.env` file and replace the url of the `DATABASE_URL`. Remember to replace the `<password>` part with your password.

# Creating the database schema or blueprint

1. In `schema.prisma` we are going to create the database models and relationships between its elements.

2. After the schema is done, we need `to push this schema to the database` on mongo db atlas. To do that, type on the terminal:

```sh
npx prisma db push
```

-   If you go now to MongoDB Atlas > Browse collection you should be able to see the 4 models or tables push from vscode.
