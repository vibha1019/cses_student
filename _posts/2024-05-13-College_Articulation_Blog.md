<div style="background-color: #e6e6fa; padding: 20px; border-radius: 10px;">
    <h2 style="font-family: 'Helvetica', sans-serif; color: #333; text-align: center;">Game Control Code</h2>
    <h3 style="font-family: 'Helvetica', sans-serif; color: #333; margin-bottom: 10px;">Game Objects Code</h3>
    <div style="background-color: #c8e6c9; padding: 15px; border-radius: 8px; margin-top: 20px;">
        <pre>
            <code>
            // Quidditch Game Level definition...
            const quidditchGameObjects = [
            // GameObject(s), the order is important to z-index...
            { name: 'quidditch', id: 'background', class: Background, data: this.assets.backgrounds.quidditch },
            { name: 'turf', id: 'platform', class: Platform, data: this.assets.platforms.turf },
            { name: 'clouds', id: 'background', class: BackgroundClouds, data:this.assets.backgrounds.clouds }, 
            { name: 'blocks', id: 'jumpPlatform', class: BlockPlatform, data: this.assets.platforms.cobblestone, xPercentage: 0.1, yPercentage: 0.81 },
            { name: 'blocks', id: 'jumpPlatform', class: BlockPlatform, data: this.assets.platforms.cobblestone, xPercentage: 0.14, yPercentage: 0.81 },
            { name: 'blocks', id: 'jumpPlatform', class: BlockPlatform, data: this.assets.platforms.cobblestone, xPercentage: 0.18, yPercentage: 0.81 },
            { name: 'blocks', id: 'jumpPlatform', class: BlockPlatform, data: this.assets.platforms.cobblestone, xPercentage: 0.22, yPercentage: 0.81 },
            { name: 'blocks', id: 'jumpPlatform', class: BlockPlatform, data: this.assets.platforms.cobblestone, xPercentage: 0.22, yPercentage: 0.69 },
            { name: 'blocks', id: 'jumpPlatform', class: BlockPlatform, data: this.assets.platforms.cobblestone, xPercentage: 0.30, yPercentage: 0.81 },
            { name: 'blocks', id: 'jumpPlatform', class: BlockPlatform, data: this.assets.platforms.cobblestone, xPercentage: 0.30, yPercentage: 0.71 },
            { name: 'blocks', id: 'jumpPlatform', class: BlockPlatform, data: this.assets.platforms.cobblestone, xPercentage: 0.30, yPercentage: 0.61 },
            { name: 'blocks', id: 'jumpPlatform', class: BlockPlatform, data: this.assets.platforms.cobblestone, xPercentage: 0.30, yPercentage: 0.33 },
            { name: 'blocks', id: 'jumpPlatform', class: BlockPlatform, data: this.assets.platforms.cobblestone, xPercentage: 0.30, yPercentage: 0.23 },
            { name: 'blocks', id: 'jumpPlatform', class: BlockPlatform, data: this.assets.platforms.cobblestone, xPercentage: 0.30, yPercentage: 0.13 },
            { name: 'blocks', id: 'jumpPlatform', class: BlockPlatform, data: this.assets.platforms.cobblestone, xPercentage: 0.34, yPercentage: 0.81 },
            { name: 'blocks', id: 'jumpPlatform', class: BlockPlatform, data: this.assets.platforms.cobblestone, xPercentage: 0.38, yPercentage: 0.81 },
            { name: 'blocks', id: 'jumpPlatform', class: BlockPlatform, data: this.assets.platforms.cobblestone, xPercentage: 0.42, yPercentage: 0.81 },
            { name: 'blocks', id: 'jumpPlatform', class: BlockPlatform, data: this.assets.platforms.cobblestone, xPercentage: 0.38, yPercentage: 0.57 },
            { name: 'blocks', id: 'jumpPlatform', class: BlockPlatform, data: this.assets.platforms.cobblestone, xPercentage: 0.38, yPercentage: 0.47 },
            { name: 'blocks', id: 'jumpPlatform', class: BlockPlatform, data: this.assets.platforms.cobblestone, xPercentage: 0.38, yPercentage: 0.37 },
            { name: 'blocks', id: 'jumpPlatform', class: BlockPlatform, data: this.assets.platforms.cobblestone, xPercentage: 0.38, yPercentage: 0.27 },
            { name: 'blocks', id: 'jumpPlatform', class: BlockPlatform, data: this.assets.platforms.cobblestone, xPercentage: 0.38, yPercentage: 0.17 },

            { name: 'blocks', id: 'jumpPlatform', class: BlockPlatform, data: this.assets.platforms.cobblestone, xPercentage: 0.536, yPercentage: 0.72 },
            { name: 'blocks', id: 'jumpPlatform', class: BlockPlatform, data: this.assets.platforms.cobblestone, xPercentage: 0.616, yPercentage: 0.81 },
            { name: 'blocks', id: 'jumpPlatform', class: BlockPlatform, data: this.assets.platforms.cobblestone, xPercentage: 0.696, yPercentage: 0.90 },

            { name: 'blocks', id: 'jumpPlatform', class: BlockPlatform, data: this.assets.platforms.yellowpattern, xPercentage: 0.456, yPercentage: 1.08 },
            { name: 'blocks', id: 'jumpPlatform', class: BlockPlatform, data: this.assets.platforms.yellowredpattern, xPercentage: 0.456, yPercentage: 0.985 },
            { name: 'blocks', id: 'jumpPlatform', class: BlockPlatform, data: this.assets.platforms.yellowpattern, xPercentage: 0.456, yPercentage: 0.89 },
            { name: 'blocks', id: 'jumpPlatform', class: BlockPlatform, data: this.assets.platforms.lionpattern, xPercentage: 0.456, yPercentage: 0.795 },
            { name: 'blocks', id: 'jumpPlatform', class: BlockPlatform, data: this.assets.platforms.yellowpattern, xPercentage: 0.456, yPercentage: 0.7 },
            { name: 'blocks', id: 'jumpPlatform', class: BlockPlatform, data: this.assets.platforms.yellowredpattern, xPercentage: 0.456, yPercentage: 0.605 },
            { name: 'blocks', id: 'jumpPlatform', class: BlockPlatform, data: this.assets.platforms.yellowpattern, xPercentage: 0.456, yPercentage: 0.51 },
            { name: 'blocks', id: 'jumpPlatform', class: BlockPlatform, data: this.assets.platforms.lionpattern, xPercentage: 0.456, yPercentage: 0.415 },

            { name: 'draco', id: 'draco', class: Draco, data: this.assets.enemies.draco, xPercentage: 0.3, minPosition: 0.05, difficulties: ["normal", "hard", "impossible"] },
            { name: 'draco', id: 'draco', class: Draco, data: this.assets.enemies.draco, xPercentage: 0.5, minPosition: 0.3, difficulties: ["normal", "hard", "impossible"] },
            { name: 'draco', id: 'draco', class: Draco, data: this.assets.enemies.draco, xPercentage: 0.75, minPosition: 0.5, difficulties: ["normal", "hard", "impossible"] }, //this special name is used for random event 2 to make sure that only one of the Goombas ends the random event
            { name: 'dementor', id: 'dementor', class: Dementor, data: this.assets.enemies.dementor, xPercentage: 0.5, minPosition: 0.05 },
            { name: 'dementor', id: 'dementor', class: Dementor, data: this.assets.enemies.dementor, xPercentage: 0.9, minPosition: 0.5 },

            { name: 'coin', id: 'coin', class: Coin, data: this.assets.obstacles.snitch, xPercentage: 0.095, yPercentage: 0.7 },
            { name: 'coin', id: 'coin', class: Coin, data: this.assets.obstacles.snitch, xPercentage: 0.135, yPercentage: 0.7 },
            { name: 'coin', id: 'coin', class: Coin, data: this.assets.obstacles.snitch, xPercentage: 0.175, yPercentage: 0.7 },
            { name: 'coin', id: 'coin', class: Coin, data: this.assets.obstacles.snitch, xPercentage: 0.375, yPercentage: 0.7 },
            { name: 'coin', id: 'coin', class: Coin, data: this.assets.obstacles.snitch, xPercentage: 0.409, yPercentage: 0.7 },
            { name: 'coin', id: 'coin', class: Coin, data: this.assets.obstacles.snitch, xPercentage: 0.295, yPercentage: 0.46 },

            { name: 'coin', id: 'coin', class: Coin, data: this.assets.obstacles.snitch, xPercentage: 0.687, yPercentage: 0.79, },
            { name: 'coin', id: 'coin', class: Coin, data: this.assets.obstacles.snitch, xPercentage: 0.611, yPercentage: 0.7 },
            { name: 'coin', id: 'coin', class: Coin, data: this.assets.obstacles.snitch, xPercentage: 0.529, yPercentage: 0.61 },

            { name: 'harry', id: 'player', class: PlayerQuidditch, data: this.assets.players.harry },
            { name: 'tube', id: 'tube', class: Tube, data: this.assets.obstacles.tube },
            { name: 'waterEnd', id: 'background', class: BackgroundTransitions,  data: this.assets.transitions.waterEnd },
            ];

            // Quidditch Game Level added to the GameEnv ...
            new GameLevel({ tag: "quidditch", callback: this.playerOffScreenCallBack, objects: quidditchGameObjects });

            </code>
        </pre>
    </div>
<h3 style="font-family: 'Helvetica', sans-serif; color: #333; margin-bottom: 10px;">How JavaScript Objects become a GameLevel</h3>
<div style="background-color: #c8e6c9; padding: 15px; border-radius: 8px; margin-top: 20px;">
<p style="font-family: 'Helvetica', sans-serif; color: #333;">
    The quidditchGameObjects array defines the elements that create a Quidditch game level. Each element in this array represents a game object with properties like name, id, class, data, xPercentage, yPercentage, minPosition, and difficulties.
    <br><br>1. Definition of game objects: Each object within the quidditchGameObjects array represents a component of the game level, such as the background, platforms, enemies (like Draco and Dementor), coins, player (Harry), tubes, and background transitions.
    <br><br>
    2. Properties of game objects:
       <br>- name: Describes the category or type of the game object (quidditch, blocks, draco, coin, harry).
       <br>- id: Unique identifier for each game object.
       <br>- class: Specifies the JavaScript class associated with each game object type.
       <br>- data: Contains the specific data or assets required for showing each game object.
       <br>- xPercentage and yPercentage: Indicate the position of the game object relative to the screen size.
       <br>- minPosition: Minimum position of the game object on the screen.
       <br>- difficulties: Specifies the difficulty levels for certain game objects.
    <br><br>
    3. Creation of GameLevel: The GameLevel constructor function is called with an object parameter containing properties like tag, callback, and objects. 
       <br>- tag: Indicates the tag or identifier for the game level (quidditch in this case).
       <br>- callback: Specifies playerOffScreenCallBack to handle certain events within the game level.
       <br>- objects: Contains the array quidditchGameObjects, which defines all the game objects for the level.
    <br><br>
    Overall, JavaScript objects in the quidditchGameObjects are used to define the components of the Quidditch game level, which are then instantiated within a GameLevel instance for use within the game environment.
</p>

</div>
    <h3 style="font-family: 'Helvetica', sans-serif; color: #333; margin-bottom: 10px;">Game Level Code</h3>
    <div style="background-color: #c8e6c9; padding: 15px; border-radius: 8px; margin-top: 20px;">
        <pre>
            <code>
                // Load GameLevel objects
                    if (GameEnv.currentLevel !== newLevel) {
                        GameEnv.claimedCoinIds = [];
                    }
                    await newLevel.load();
                    GameEnv.currentLevel = newLevel;
            </code>
        </pre>
    
    <div style="background-color: #c8e6c9; padding: 15px; border-radius: 8px; margin-top: 20px;">
        <h3 style="font-family: 'Helvetica', sans-serif; color: #333; margin-bottom: 10px;">Where Game Level is Used in Game Control</h3>
        <p style="font-family: 'Helvetica', sans-serif; color: #333;">
            The newLevel.load() method is called to load the game objects associated with the new level. This method is defined within the GameLevel class and is used to initialize and load game elements such as background, platforms, enemies, etc. Then, the GamEnv.currentLevel is also updated. 

            After loading the new level, various things happen, such as updating certain properties, setting the invert property, and  a resize event to redraw canvas elements.
        </p>
   
</div>


</div>
    <h3 style="font-family: 'Helvetica', sans-serif; color: #333; margin-bottom: 10px;">GameLoop Code</h3>
    <div style="background-color: #c8e6c9; padding: 15px; border-radius: 8px; margin-top: 20px;">
        <pre>
            <code>
                gameLoop() {
                    // Turn game loop off during transitions
                    if (!this.inTransition) {
                        // Get current level
                        GameEnv.update();
                        const currentLevel = GameEnv.currentLevel;
                        // currentLevel is defined
                        if (currentLevel) {
                            // run the isComplete callback function
                            if (currentLevel.isComplete && currentLevel.isComplete()) {
                                const currentIndex = GameEnv.levels.indexOf(currentLevel);
                                // next index is in bounds
                                if (currentIndex !== -1 && currentIndex + 1 < GameEnv.levels.length) {
                                    // transition to the next level
                                    this.transitionToLevel(GameEnv.levels[currentIndex + 1]);
                                } 
                            }
                        // currentLevel is null, (ie start or restart game)
                        } else {
                            // transition to beginning of game
                            this.transitionToLevel(GameEnv.levels[0]);
                        }
                    }
                    // recycle gameLoop, aka recursion
                    requestAnimationFrame(this.gameLoop.bind(this));  
                },
            </code>
        </pre>
    </div>


<div style="background-color: #c8e6c9; padding: 15px; border-radius: 8px; margin-top: 20px;">
        <h3 style="font-family: 'Helvetica', sans-serif; color: #333; margin-bottom: 10px;">Where Game Loop is Used</h3>
        <p style="font-family: 'Helvetica', sans-serif; color: #333;">
            In the gameLoop method:
            <br><br>- The GameEnv.update() method is called, which is responsible for updating the state of the game environment, meaning positions and animations of all game objects. This method iterates over all game objects and calls their update methods to handle their behavior for each frame.
            <br><br>- The currentLevel variable is retrieved from GameEnv. This represents the current level of the game.
            <br><br>- If a current level exists (currentLevel is defined), the isComplete callback function of the current level is checked. If the level is complete, the game will transition to the next level using the transitionToLevel method.
            <br><br>- If there's no current level (at the start or restart of the game), the game transitions to the beginning of the game, loading the first level.
            <br><br>- Finally, the requestAnimationFrame function is used to call this.gameLoop, called recursively, creating a continuous loop for the game control flow.
            <br><br>
            Overall, the gameLoop method starts the main loop of the game, ensuring that the game environment is updated and transitioning between levels.
        </p>
    </div>

<div style="background-color: #c8e6c9; padding: 15px; border-radius: 8px; margin-top: 20px;">
    <h3 style="font-family: 'Helvetica', sans-serif; color: #333; margin-bottom: 10px;">Examine Game Objects in Inspect</h3>
    <div style="background-color: #e6e6fa; padding: 20px; border-radius: 10px;">
        <img src="images/canvas_inspect.png" alt="Canvas Inspect" style="max-width: 100%; height: auto; display: block; margin: 0 auto;">
    </div>



</div>
    <h3 style="font-family: 'Helvetica', sans-serif; color: #333; margin-bottom: 10px;">End and Transition of Level Code</h3>
    <div style="background-color: #c8e6c9; padding: 15px; border-radius: 8px; margin-top: 20px;">
        <pre>
            <code>
                * Transitions to a new level. Destroys the current level and loads the new level.
                * @param {Object} newLevel - The new level to transition to.
                */
                async transitionToLevel(newLevel) {
                    this.inTransition = true;

                    // Destroy existing game objects
                    GameEnv.destroy();

                    // Load GameLevel objects
                    if (GameEnv.currentLevel !== newLevel) {
                        GameEnv.claimedCoinIds = [];
                    }
                    await newLevel.load();
                    GameEnv.currentLevel = newLevel;

                    // Update invert property
                    GameEnv.setInvert();
                    
                    // Trigger a resize to redraw canvas elements
                    window.dispatchEvent(new Event('resize'));

                    this.inTransition = false;
                },

                gameLoop() {
                    // Turn game loop off during transitions
                    if (!this.inTransition) {

                        // Get current level
                        GameEnv.update();
                        const currentLevel = GameEnv.currentLevel;

                        // currentLevel is defined
                        if (currentLevel) {
                            // run the isComplete callback function
                            if (currentLevel.isComplete && currentLevel.isComplete()) {
                                const currentIndex = GameEnv.levels.indexOf(currentLevel);
                                // next index is in bounds
                                if (currentIndex !== -1 && currentIndex + 1 < GameEnv.levels.length) {
                                    // transition to the next level
                                    this.transitionToLevel(GameEnv.levels[currentIndex + 1]);
                                } 
                            }
                        // currentLevel is null, (ie start or restart game)
                        } else {
                            // transition to beginning of game
                            this.transitionToLevel(GameEnv.levels[0]);
                        }
                    }

                    // recycle gameLoop, aka recursion
                    requestAnimationFrame(this.gameLoop.bind(this));  
                }

            </code>
        </pre>
    
    <div style="background-color: #c8e6c9; padding: 15px; border-radius: 8px; margin-top: 20px;">
        <h3 style="font-family: 'Helvetica', sans-serif; color: #333; margin-bottom: 10px;">How Transition Level is Determined</h3>
        <p style="font-family: 'Helvetica', sans-serif; color: #333;">
            Here, the transitionToLevel method is responsible for transitioning to a new level within the game. Within this method, the newLevel parameter represents the new level to transition to. The newLevel object is an instance of GameLevel.

            To check if the current level is complete, 
            The gameLoop method continuously runs, updating the game state and checking the completion status of the current level.
            If the currentLevel exists (if (currentLevel)), the code checks if the isComplete method  of currentLevel returns true.
            The isComplete method is part of the GameLevel class and returns true when the leve is complete. 

            To transition to new level
            If the isComplete method returns true, the current level is considered complete.
            The gameLoop method then finds the index of the currentLevel in the GameEnv.levels array.
            If the index is valid and the next level exists in the array (if (currentIndex !== -1 && currentIndex + 1 < GameEnv.levels.length)), it calls the transitionToLevel method to load the next level.
            If the current level is null (meaning the game is starting or restarting), it transitions to the first level in the GameEnv.levels array.

=        </p>
    </div>
</div>
