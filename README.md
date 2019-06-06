# gatsby-tutorial

### Requirements

1. Node JS
2. npm or yarn
3. A Wordpress site running on your local

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
baseUrl: "myportfolio.lndo.site"
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







