## General Steps ##

 1. Create credentials;
 2. Install and configure vue-authenticate;
 3. Create Social Login component;
 4. Get post from the social network on API;
 5. Set data to local storage.

Let's get started!

## Creating credentials ##
First of all, you need to create credentials that will send to the social network, for this purpose need account Google or Facebook because this article will be about login with Google and Facebook.
### Google ###
If you want to use google, go to the https://console.developers.google.com/
<br/>
You should see this page. Click create.
<br/>

> ![Create new project][1]

Enter your project name and organization(if needed).
<br/>
Our next step will add **API services** for your project. After the successfully created project you can see something like this:

> ![Successfully created project][2]

Here click Enable APIs and Services.
<br>
And search for the next services: Google+ API and Contacts API
<br>

> ![Google+ API][3]

> ![Contacts API][4]

Click on service and click enable
<br>

> ![Enable service][5]

After you enable two services to go to the dashboard page and click **Credentials**.

> [Credential link][6]

In the Credentials page click **Create consent screen** and perform the next steps.

> ![Create consent screen][7]

Choose external and go to next.

> ![External][8]

Here you need to enter the project name and authorization domain, this domain cannot be `localhost` or `site.local`. You need to enter something like this `mysite.com`, `mysite.do` - you can add an alias in your /etc/hosts.

> ![Project name][9]

> ![Authorization domain][10]

Now you need to create credentials for this return to the **Credentials** page and click **Create credentials** and choose OAuth client ID.

> ![Create credentials][11]

> ![OAuth client ID][12]

On the next page choose **Web application**. Enter the name and click **Create**.

> ![Web application][13]

Now you can see your client_id and client_secret. Save it in the future we will use it.
<br>
### Facebook ###


  [1]: https://i.stack.imgur.com/wnVww.png
  [2]: https://i.stack.imgur.com/XopGs.png
  [3]: https://i.stack.imgur.com/Ff9md.png
  [4]: https://i.stack.imgur.com/M9lXe.png
  [5]: https://i.stack.imgur.com/yIYfZ.png
  [6]: https://i.stack.imgur.com/OhUGr.png
  [7]: https://i.stack.imgur.com/5fuNf.png
  [8]: https://i.stack.imgur.com/DlkDC.png
  [9]: https://i.stack.imgur.com/kd19I.png
  [10]: https://i.stack.imgur.com/LaOUB.png
  [11]: https://i.stack.imgur.com/RoP4d.png
  [12]: https://i.stack.imgur.com/pQ7UA.png
  [13]: https://i.stack.imgur.com/D53Mp.png
