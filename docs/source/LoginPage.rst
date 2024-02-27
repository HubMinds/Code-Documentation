LOGIN PAGE

The Login Page is used for users to lgoin to there personal accounts.
.. code-block :: Flutter 
  SignIn()

This page works using Firebase authentication service to allow a user to enter an email and password and login into the main application. 
.. code-block :: Flutter 
  FirebaseAuth()

Duirng this process Flutter will collect the U(nique)ID 
.. code-block :: Flutter
  String user = newUser.user!.uid;

it will then push to the main page with this uid to give the user there personalised hub
.. code-block :: Flutter
  Navigator.push(
      context,
      MaterialPageRoute(builder: (context) => Home(uid: user)),
    );
