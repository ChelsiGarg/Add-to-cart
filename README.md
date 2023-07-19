Hi!

I have built a mobile app which is not a native mobile app but is disguised as the one. It is basically a **Progressive Web App**.
You can access the site [here](https://add-to-cart-chelsi.netlify.app)

To fetch and store the data in realtime database, I have used firebase. The functionalities of firebase that were used are listed below:
1. **Firebase:initializeapp -** It is used to initialize the app using the database URL.
2. **Firebase:getDatabase -** It returns the realtime database that is associated with the firebase App that we just created using *initializeapp*
3. **Firebase:reference -** It will create a reference of name passed as 2nd parameter to ref function. In this project, name given was *shopping list*. So, in the 
   realtime database, under the name *shopping list* all shopping list items would be present.
4. **Firebase:push -** It is used to push the data to our database.
5. **Firebase:onValue -** It listens for the changes in database. Whenever a change occurs, it runs the piece of code written inside it to reflect the changes accordingly.
6. **Firebase:remove -** It takes the exact path of the value that needs to be removed from database & then removes it from databse.

Some other properties that I specifically added to improve user experience are:
1. **user-select :** This is CSS property added so that user couldn't unintentionally select parts of the app.
2. **Setting the viewport:** This is the line added in html file under *title tag* to set the width of app correct in mobile devices.
3. **Favicon:** It is a small icon that we can see in the tab header in the browser. More importantly, it is something that we will see in the mobile home screen when we launch the app.
4. **Web Application Manifest:** This is the file which allowed us to transform the web application to look like the native app on our mobile devices.
