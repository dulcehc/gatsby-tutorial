# Gatsby and Wordpress Tutorial

### Requirements

1. Node JS
2. npm or yarn
3. A Wordpress site running on your local, with one page and one post.

### Setting up Gatsby

1. Install Gatsby globally

```
npm install -g gatsby-cli
```

2. Create site
```
gatsby new name_of_your_site
```

3. Open directory and run gatsby with the following commands:

```
cd name_of_your_site
gatsby develop
```

4. The project will start in http://localhost:8000/


### Install Wordpress plugin

1. Go to the following link to look for the Wordpress plugin, https://www.gatsbyjs.org/packages/gatsby-source-wordpress/?=wordpress


2. Install the plugin

```
npm install --save gatsby-source-wordpress
```

3. Open the file gatsby-config.js and add configuration from the section [How to use](https://www.gatsbyjs.org/packages/gatsby-source-wordpress/?=wordpress#how-to-use)

4. Update the baseUrl with your local Wordpress URL, for example:

```
baseUrl: "wordpress-site.lndo.site"
```

5. Open the file gatbsy-node.js and add configuration from the section [Site’s gatsby-node.js example](https://www.gatsbyjs.org/packages/gatsby-source-wordpress/?=wordpress#sites-gatsby-nodejs-example)


### Wordpress Site

1. Move the "empty" folder from this project to the Wordpress themes folder, you should have the following:

```
wordpress-site/wp-content/themes

empty           index.php       twentynineteen  twentyseventeen twentysixteen
```

2. Go to your admin panel, e.g https://wordpress-site.lndo.site/wp-admin/.

3. Go to Appearance -> Themes -> Empty Theme Starter -> Activate

![image](https://user-images.githubusercontent.com/19391835/59040731-ec934300-883c-11e9-820a-6b90afaa699e.png)

4. Visit your Wordpress site and you should see that it's blank.


### Rendering Data and GraphQL

1. Copy the folder templates from this repository into your src folder.

![image](https://user-images.githubusercontent.com/19391835/59042216-a9869f00-883f-11e9-8dcc-f3aff8e5e407.png)


2. Execute the Gatsby project:
```
gatsby develop
```

or

```
npm run develop
```

3. In the console, you should see a link to GraphiQL: http://localhost:8000/___graphql, open it in your browser.


![image](https://user-images.githubusercontent.com/19391835/59042551-434e4c00-8840-11e9-8432-808dcbd8907d.png)

4. This query will retrieve the information from the Wordpress pages of your current site.

You can use the Explorer (Left Menu) to see all the different data that you can query.


5. If you visit http://localhost:8000, you should be redirected to http://localhost:8000/sample-page.

![image](https://user-images.githubusercontent.com/19391835/59079749-c7d5b480-88aa-11e9-9ca4-fd5eb0717e74.png)

