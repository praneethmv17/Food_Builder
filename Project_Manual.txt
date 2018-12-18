Name:		Venkata Praneeth Mummaneni
UML ID: 	01662636
UML Email-ID:	venkatapraneeth_mummaneni@student.uml.edu
Project Link:	http://weblab.cs.uml.edu/~vmummane/IWS1/Final_Project/burger-project/
(NOTE: I was not able to deploy my App on weblab server even after numerous tries due to configuration issues, so I have deployed it on Google Firebase. The above link on weblab redirects users to the address where my App is being hosted by Firebase)
---------------------------------------------------------------------------------------------------------------------------
Instructions:

To install the project on your local system perform the following steps :-

1.) Install node package manager(npm) on your PC after downloading it from the following link "https://nodejs.org/en/".
2.) Download files from the following directory: "https://github.com/praneethmv17/Food_Builder/tree/master/Week_12"
    (OR)
    Navigate to the "Week_12" folder after downloading the whole project from "https://github.com/praneethmv17/Food_Builder"
    (OR)
    If you want to check the progress of each week, you can navigate to the project folder present in each week after downloading the       whole project from "https://github.com/praneethmv17/Food_Builder" and then navigate to the week you want to access.
3.) Navigate to the burger-project folder.
4.) Open Windows PowerShell(or)Terminal in the folder.
5.) Execute the following command to start the project - "npm start"
6.) You will observe that your Browser will pop-up and will start the App.
7.) To EXIT from the project, press "ctrl + c" in the terminal/powershell window.

To navigate inside the project, perform the following steps:-  

1.) Open "http://weblab.cs.uml.edu/~vmummane/IWS1/Final_Project/burger-project/". The Burger App will start up.
2.) On the top right corner, you will see an "AUTHENTICATE" button. Click on it and it will take
    you to the log in page. Add some email and password(must be atleast 6 characters long) and click on Submit.
    This will take you to the BurgerBuilder page.
3.) You can start adding ingredients to your burger by clicking more keys beside each ingredient. Then, click on
    "Order Now" button at the bottom and then press "CONTINUE" on the Order Summary pop-up.
4.) Now, you can see your finalized burger with the text "We hope you like it!". Click on "Continue" and then
    scroll down to find a form to fill Name, Street, Zipcode(must be 5 characters long), Country, Email
    and Deliver Method(Fastest/Cheapest). Then, Click on "ORDER". Now, You can see your order in the "ORDERS" tab.
5.) You can click on "LOGOUT" to safely Log out. If you want to log back in with the profile you created earlier,
    click on "AUTHENTICATE" button, and enter your email and password and then, click on
    "SWITCH TO SIGN IN". Then, click on "SUBMIT" to log in.

------------------------------------------------------------------------------------------------------------------------------------
References:

I have used below sources to gain a basic understanding of ReactJS:-
• https://reactjs.org/
• https://medium.freecodecamp.org/all-the-fundamental-react-js-concepts-jammed-into-thissingle-medium-article-c83f9b53eac2

I have used the below course by Maximilian Schwarzmuller to get a better understanding of ReactJS/Redux and build the burger-project step-by-step :-
• https://www.udemy.com/react-the-complete-guide-incl-redux/

The below link contains essential information to host your project on Firebase, handle authentication and use the real-time database :-
• https://firebase.google.com/docs/
• Hosting: https://firebase.google.com/docs/hosting/
• Real-time database: https://firebase.google.com/docs/database/
• Authentication: https://firebase.google.com/docs/auth/

I have utilized the info in the links below to make HTTP requests(GET/POST) to the Firebase database in files axios-orders.js(to create an instance of baseURL to the database on Firebase), BurgerBuilder.js, ContactData.js(in order to POST Contact Data), Orders.js, withErrorHandler(for error handling), auth.js(to POST User authentication data onto Firebase), burgerBuilder.js(GET to retrieve ingredients initially from Firebase) and order.js(to GET previous orders and to POST new orders) :- 
• https://www.npmjs.com/package/axios
• https://hackernoon.com/tutorial-how-to-make-http-requests-in-react-part-3-daa6b31b66be

I have utilized the info in the links below to gain a better understanding of Redux. Code(mainly of the "connect" component) in the following links is being utilized in App.js, Auth.js, Logout.js, BurgerBuilder.js, Checkout.js, ContactData.js, Layout.js, index.js in order to distribute authentication/ingredients/order data(which is common for all mentioned components) as properties to each component :-
• https://redux.js.org/basics/usagewithreact
• https://medium.freecodecamp.org/understanding-redux-the-worlds-easiest-guide-tobeginning-redux-c695f45546f6

I have utilized the info in the links below to handle internal routing in my App. I have used code from the 1st link below namely the code for <Route> for internal routing, <Redirect> for redirection to specific paths in case of an invalid URL, <BrowserRouter> to allow routing throughout the App, <Switch> to Switch between paths in App.js/Index.js :-
• https://reacttraining.com/react-router/web/guides/quick-start
• https://www.npmjs.com/package/react-router-dom

I have used the 2nd spinner CSS code present in the following source to implement a Spinner in Auth.js(to show that User authentication is in progress), BurgerBuilder.js(to show that ingredients are being loaded), ContactData.js(to show that contact data is being sent to Firebase) and in Orders.js(to show that past orders are being retrieved) :-
• https://projects.lukehaas.me/css-loaders/
