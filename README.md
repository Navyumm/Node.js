# steps to work on this :
-------------------------------

1) package.json file banao
    -> npm init

2) git me upload karenge
    -> git init

____________

ab maan lo hume koi image vgra upload karni hai to use hum to usko hum tempraroly apne server par rakhte hai
kyoki maan lo kbhi server(AWS, AZURE) ka connection fail ho to images hmari store ho

to iske liye hum ek folder bnayenge public naam server

-> Public -> temp ->  git status -> .gitkeep

<!--  -->

.gitignore 
-> jo file hume git par upload nhi karni usai is file me daalte hai

# we have git ignore generator 

<!-- -->

# .env file bnayenge :
# ab src folder bnayenge : directories files ke liye
# aur uske ye 3 files banao 
    -> app.js constants.js index.js

____________________



# ab import waale tarike se kaam karne ke liye 
package.json me ye add karo -> "type":"module",

# ab nodemon install karo 
    -> npm i -D nodemon

# ab package.json me script me ye add karo
    -> "dev": "nodemon src/index.js"   

-------------------

# ab mujhe kuch folders bhi chahiye src ke andr 
 -> aur aage chalkar hmare kaam aayenge production me

-> controllers : yaha par hmari hogi major functionality
-> db : database connect kaise karna hai 
-> middlewares : code in between 
-> modules
-> routes : alg alg sbhi route ko manage karne ke liye 
-> utils : utilities me hmari vo file aati hai jo functionality baar baar repeat hoti hai 

---------------------

# Now install prettier from npm
-> because of hum code team me likhenge, ab koi kaisa code likh rha hai koi kaisa, to waha prettier add karna imp hai
    npm i -D prettier

-> install karne ke baad ye 2 files banao

.prettierrc -> sbhi jagah apply karne ke liye 
.prettierignore -> idhr apply nhi karna vo

------------------------


# DB connection karenge ab hum 

.env -> me PORT or variables set karo

fir db ka naam constants file me likhna hai 

------------------------

# db connection mainly 2 tarike se ho sakta hai 

1) sara code index.js me likho -> aur usko execute karwado
2) db naam ka koi folder banau isme connection jo bhi fuction hai vo likhuaur fir index file mein function ko import karwau aur waha execute karwau


-----------------------

# ab db connection akrte hai 

1) install dotenv, mongoose, and express 
    npm i mongoose express dotenv

2) point to me notice    
    -> jab bhi db se baat karo try and catch appoarch jarur lagao with async await

3) ab index.js file me jaakr code likhe hai    

-------------------------
 # ab 2nd appoarch

 -> bd ke andr -> index.js
 -> dotenv ko require karo

