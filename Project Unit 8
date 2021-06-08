##### Name: Tuong Tran
##### Project unit: 8 
##### Instructions: PLEASE READ THE INSTRUCTION CAREFULLY!!! 
##### In this game, we're going to be BOTH clicking the mouse and pressing keys. Here are the list of keys:
##### Make your decission in the beginning:
##### 1/ "y" | Press "y" on your keyboard to say "yes" -> starts the game
##### 2/ "n" | Press "n" on your keyboard to say "no" -> receives a message instead
##### Then, a white button (that looks like a target) shows up. Using your MOUSE, click on that button to bring 
##### the first object, a sugar cube, to the game. You will only have 3 tries to change the sugar's position
##### if you don't like the current one.
##### Allow Gretel(object 2 ) and Hansel (object 3) to appear:
##### 3/ "p" | Press "p" on your keyboard to allow the game to create object 2 and 3. Once "p" is pressed, 
##### click on a random location on the canvas. Where you click will create Gretel, the second object, and 
##### where Gretel stands will creates Hansel but on the opposite side. You will see Gretel and Hansel going around.
##### 4/ Activate game mode: 
##### "m" | To actually play the game, press "m" on your keyboard. By doing this, you're also setting up the game features.
##### In game:
##### Move sugar (the white polygon, object 1) up and down:
##### 5/ "w" | Press "w" on your keyboard to move the sugar upwards
##### 6/ "s" | Press "s" on your keyboard to move the sugar downwards
##### 7/ "a" | Press "a" on your keyboard to move the sugar to the left
##### 8/ "d" | Press "d" on your keyboard to move the sugar to the right
##### Changing the radius of sugar (the white polygon, object 1):
##### 9/ "q" | Press "q" on your keyboard to increase the radius of the sugar cube (object 1)
##### 10/ "e" | Press "e" on your keyboard to decrease the radius of the sugar cube (object 1)
##### Changing the rotateAngle speed of Gretel (red dot, object 2) and Hansel (blue dot, object 3):
##### 11/ "g" | I mentioned Hansel and Gretel will go in circle around the sugar. Press "g" to increase their speed
##### 12/ "h" | Press "h" on your keyboard to decrease the speed of Gretel and Hansel
##### Changing the speed of the sugar (the white polygon, object 1):
##### 13/ "2" | Press the number key "2" on your keyboard to increase the sugar cube (object 1)'s speed
##### 14/ "3" | Press the number key "3" on your keyboard to decrease the sugar cube (object 1)'s speed

##### Note that Player 2 can use key "w", "a", "s", "d", "q", "e", "2", and "3" to control the sugar in anyway they 
##### like. Player 1, on the other hand, can only use the mouse to click, and use key "g" and "h". Player one is free
##### to stop Gretels and Hansels (the objects) circling around (press "h" for a long time) if that confuse them.

##### How to play the game: 
##### Once "m" is pressed, the game is officially on. 2 people will be needed in this game, and they're going to  
##### compete against each other. Player 1's score will be presented in a pink number, to the right. Player 1's job 
##### is to click on the sugar cube whenever he or she can. When his or her mouse hits the sugar, one point is added.
##### However, player 2 is there to prevent that. Player 2's score will be presented in a blue number, to the right.
##### Player 2's job is to move the sugar as quickly and complicated as possible to trick player 1 into clicking the 
##### canvas.When player 1 clicks on the canvas (but not the sugar), player 2's score is added one point. Simple, no?
##### After some tries, depends on the score, the victory will either belongs to player 1, 2 or both (yes, that's possible).

##### You might noticed that I named object 2 and 3 as Gretel and Hansel. To me, player 1 and 2 has the same name. 
##### They're Gretel and Hansel, who's collecting sugar cubes (aka the points) to make cookies! However, I won't name
##### the players as Gretel and Hansel as it would confuse players. Play till the end to see what I mean. 

######## Requirements: (most requirements begin from line 236)
####### Object one with randrange: Line 128 and 236. Line 128 is where I created the sugar, line 236 is where 
###### sugar actually has its centerX and centerY as randrange 
####### Object two with distance and angle to: Line 243 
###### Object three with getPointInDir: Line 259
##### Functions: Line 101 and 105
##### Custom properties: Begins line 66 and 147
##### Nested for loop: Line 118
##### Variables: Line 95, and begins from line 147. Helper variables at line 207 and line 252.
##### Groups: Line 88, begins at line 91, line 135, and line 163
##### Helper variables: Line 205, line 206, begins line 214, and begins line 245

##### Setting!!!!!!!
###Set background 
app.background = rgb(2,20,47)

###Custom properties
###Help in creating the galaxy/star-ish background
app.starCount = 0
app.createStars = True
app.starAdd = 0

### Checks whether it is time to create a sugar or not 
app.SugarIn = False
### Makes sure the player won't change the position of the sugar ude too many timme 
app.sugarOnce=0

### Checks whether is it time to create Gretel and Hansel or no
app.GH = False

### Checks whether is it playmode time or no
app.playmode=False

#### Set the speed for Gretel and Hansel's rotateAngle 
app.rotateAngleSpeed=4

###Empty Groups
### Helps to create the background
stars= Group()

### Makes sure/help Gretel and Hansel to spin around 
Ggroup=Group()
Hgroup=Group()

### Beginning 1
###Setting variables
start = Label('y to start',200,200,fill='white',font='monospace',size=20)
giveUp = Label('n to give up',200,280,font='monospace',fill='white',size=20)

### Making cookie
###Functions (makes dots for cookies)
def makeDots(centerx,centery):
    Circle(centerx,centery,2.5,fill=rgb(54,24,22)) 

### Function to make cookies in the end
def makeCookie(centeRX,centeRY):
    Star(centeRX,centeRY,30,30,roundness=96,fill=rgb(80,56,52)) 
    makeDots(centeRX-14,centeRY-8)
    makeDots(centeRX-15,centeRY+11) 
    makeDots(centeRX+4,centeRY+16)
    makeDots(centeRX+17,centeRY+1) 
    makeDots(centeRX+3,centeRY-16)
    makeDots(centeRX-2,centeRY)

##### Prepare!!!!!!
### The stripes on the cavas. Use as a playground for the game
###Looping groups
#Draw Stripes
for i in range (35,366,85):
    for e in range(75,361,85):
        stripe1 = Line(i,0,i,400,fill=rgb(76,59,113),opacity=15,lineWidth=22)
        stripe2 = Line(0,e,400,e,fill=rgb(76,59,113),opacity=15,lineWidth=22)

stripe1.toFront()
stripe2.toFront()

###Variable
##### Object one !!!! This is where I create object one                         
sugar = RegularPolygon(-10,-10,13,6,fill=rgb(248,247,243))

### Set object one's dx and dy
sugar.dx=6
sugar.dy=6

### Beginning 2
beginning = Group(
    Rect(0,0,400,400,opacity=52),
    Label('Space Chip',200,120,font='monospace',fill='white',size=50),
    start,
    giveUp,
    )
    
### Makes sure that both the sugar and dots (Hansel and Gretel) appear on the playground
sugar.toFront()
Ggroup.toFront()
Hgroup.toFront()
    
###Variables
### Set words on the top-left 
D = Label('Distance:',13,15,fill='white',font='monospace',align='left',size=20)
A = Label('Angle:',13,46,fill='white',font='monospace',align='left',size=20)

### Local variables below will eventually hold the distance and angle of object 2
Di = Label(0,230,16,font='monospace',fill='white',align='left',size=17.5)
An = Label(0,210,46,font='monospace',fill='white',align='left',size=17.5)

### Makes sure that these local variables won't appear before Hansel and Gretel were created
D.visible=False
A.visible=False
Di.visible=False
An.visible=False

### Button in the middle (press on it to create the sugar)
button = Group(
    Circle(352,202,20,fill=None,border=rgb(248,247,243),borderWidth=5,opacity=60),
    Circle(352,202,7,fill=rgb(248,247,243),opacity=60)
    )

### Makes sure teh button won't show up until the player hit "y"    
button.visible=False

### Scores for each player :))
Gscore = Label(0,352,113,fill=rgb(228,64,94),opacity=67,font='monospace',size=45)
Hscore = Label(0,352,285,fill=rgb(193,241,255),opacity=67,font='monospace',size=45)

### Makes sure the scores won't show up until the player hit "m"
Gscore.visible=False
Hscore.visible=False

### Makes sure the beginning stands above all. After all, it is the intro    
beginning.toFront()

### Make Ending for 4 scenarios: players give up, player 1 wins, player 2 wins, and both players win
def makeEnding(message,color1,color2):
    Rect(0,0,400,400,fill=color1)
    Label(message,200,200,font='courier',size=20,fill=color2)
    makeCookie(0,0)
    makeCookie(41,8)
    makeCookie(15,70)
    makeCookie(103,92)
    makeCookie(11,336)
    makeCookie(19,387)
    makeCookie(123,363)
    makeCookie(337,351)
    makeCookie(370,373)
    makeCookie(336,0)
    makeCookie(381,41)


##### Action!!!!!!
###onStep
###Draw galaxy background
def onStep():
    ### Drawing stars for the galaxy
    #####Set the stars to appear in a random location on the canvas 
    centerX = randrange(0,400)
    centerY = randrange(0,400)
    ### Helper variables below helps creating the opacity effect of the stars
    p = randrange(0,80)
    o=20
    o = o + p
    
    # Create stars
    if(app.createStars == True):
        star = Star(centerX,centerY,4,4,fill='white',opacity=o)
        app.starAdd+=1
        stars.add(star)
    
    ### Increase app.starCount by one whenever the number of stars created ends with a 0       
    if(app.starAdd%10 == 0):
        app.starCount+=1
    
    ### Makes sure the stars will stop appearing when app.starCount > 12  
    if(app.starCount > 12):
        app.createStars=False
    elif(app.starCount < 12):
        app.createStars=True
    
    ### Makes sure Gretel and Hansel spin around    
    if(app.GH==True):
        Ggroup.rotateAngle+=app.rotateAngleSpeed
        Hgroup.rotateAngle-=app.rotateAngleSpeed
        
### onMousePress
def onMousePress(mousEX,mousEY):
    if(app.SugarIn == True):
        ##### Where object one gets its position randomly
        if(app.sugarOnce <4):
            if(button.hits(mousEX,mousEY) == True):
                ####### RANDRANGE IS HERE  !!!!!!!!!!1                              R A N D R A N G E  I S   H E R E !!!
                sugar.centerX = randrange(53,280)
                sugar.centerY =  randrange(85,330)
                app.sugarOnce+=1
            ###### Object 2!!!                                                        OBJECT 2 IS HERE !!!!!!!!!!!!
        if(app.GH == True):
            Gretel = Circle(mousEX,mousEY,6,fill=rgb(228,64,94))
            Ggroup.add(Gretel)
            
            ##### DISTANCE AND ANGLETO IS HERE!!!!!!                              DISTANCE   AND    ANGLE TO !!!!!!
            Di.value = distance(sugar.centerX,sugar.centerY,Gretel.centerX,Gretel.centerY)
            An.value = angleTo(sugar.centerX,sugar.centerY,Gretel.centerX,Gretel.centerY)
            
            ##### VARIABLES THAT STORE DISTANCE AND ANGLE TO !!!!!!!!             VARIABLES STORE MATH RESULTS!!!!!
            Dis = distance(sugar.centerX,sugar.centerY,Gretel.centerX,Gretel.centerY)
            Ang = angleTo(sugar.centerX,sugar.centerY,Gretel.centerX,Gretel.centerY)
            
            ##### GET POINT IN DIRECTION !!!!!!!!!!                             GET POINT IN DIRECTION IS HERE!!!!!
            H1, H2 = getPointInDir(sugar.centerX,sugar.centerY,Ang+180,Dis) 
            
            ##### Object 3 !!!!!!!                                                        OBJECT 3 IS HERE !!!!!!!!
            Hansel = Circle(H1,H2,6,fill=rgb(193,241,255))
            Hgroup.add(Hansel)
            
            ### The circles that helps Gretel and Hansel move
            #Gretel 
            Gcircle=Circle(sugar.centerX,sugar.centerY,abs(Dis*2)+1,fill=None)
            Ggroup.add(Gcircle)
            #Hansel
            Hcircle=Circle(sugar.centerX,sugar.centerY,abs(Dis*2)+1,fill=None)
            Hgroup.add(Hcircle)
            
            ### How the app will increase the score for each player
            if(app.playmode == True):
                Hscore.value+=1
                if(Gretel.hitsShape(sugar) == True):
                    Gscore.value+=1
            
            ### Determines how to end the game according to the points      
            if(Gscore.value > 4 and Hscore.value > 6):
                app.group.clear()
                makeEnding('Both win!! :D',rgb(2,20,47),rgb(187,181,216))
                app.stop()
            elif(Gscore.value > 4 and Hscore.value < 6):
                app.group.clear()
                makeEnding('Player 1 wins! :)',rgb(2,20,47),rgb(228,64,94))
                app.stop()
            elif(Gscore.value < 4 and Hscore.value > 6):
                app.group.clear()
                makeEnding('Player 2 wins! :))',rgb(2,20,47),rgb(193,241,255))
                app.stop()
                
        
###onKeyPress
def onKeyPress(key):
    ### What's next when the players hit "y" or "n"
    if(key == 'y'):
        app.group.remove(beginning)
        app.SugarIn=True
        
    elif(key=='n'):
        app.group.clear()
        app.SugarIn=False
        makeEnding('You missed the game! :(',rgb(2,20,47),rgb(255,233,146))
        app.stop()
    
    ### Once there's a sugar has been created, the preparation for distance and angle will appear    
    if(app.SugarIn == True):
        ###Preparation for distance and angle
        D.visible=True
        A.visible=True
        Di.visible=True
        An.visible=True
        button.visible=True
        
    #### Turn on permission for Hansel and Gretel
    if(key == 'p'):
        app.GH = True
    
    ### Turn on permission for playmode
    if(key == 'm'):
        app.playmode=True
        
def onKeyHold(keys):
    ### WHat is allowed once the player hit "m"
    if(app.playmode == True):
        ### The score for each player is on
        Gscore.visible=True
        Hscore.visible=True
        
        ### Helps player 2 to control the sugar cube
        if('w' in keys):
            sugar.centerY-=sugar.dy
        if('s' in keys):
            sugar.centerY+=sugar.dy
        if('a' in keys):
            sugar.centerX-=sugar.dx
        if('d' in keys):
            sugar.centerX+=sugar.dx
        
        ### Wraparound for the sugar   
        if(sugar.right < 0):
            sugar.left=400
        if(sugar.left > 400):
            sugar.right=0
        if(sugar.bottom < 0):
            sugar.top=400
        if(sugar.top > 400):
            sugar.bottom=0
        
        ### Change the radius of the sugar cube   
        if('q' in keys):
            if(sugar. radius < 151):
                sugar.radius+=2
        if('e' in keys):
            if(sugar.radius > 1):
                sugar.radius-=2
        
        ### Change the speed of Gretel and Hansel's speed   
        if('g' in keys):
            if(app.rotateAngleSpeed < 20):
                app.rotateAngleSpeed+=1
        if('h' in keys):
            if(app.rotateAngleSpeed > 0):
                app.rotateAngleSpeed-=1
                
        ### Change the speed of the sugar
        if('2' in keys):
            if(sugar.dx < 51 or sugar.dy < 51):                
                sugar.dx+=2
                sugar.dy+=2
        if('3' in keys):
            if(sugar.dx > 2 or sugar.dy > 2):
                sugar.dx-=2
                sugar.dy-=2 
