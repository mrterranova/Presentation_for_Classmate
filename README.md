I enjoy interactivity with my audience. 
I enjoy bringing something creative to life.
I like traditional animation. 
I like design. 
I like creating games that are both pleasing to look at and run smoothly





code ideas for Hangman that I would need...

if (player===win){
score = game + 1}
else{
score = game}

Array = random array, changes the amount of letters each time
Read letters in array
create loop for reading letters in array. 


3:00pm - 3:50pm, Monday, June 17, 2019





How the Game Operates…


var won = true;
//option if won the game then will start over once again. 
while (won){	

	var song = [“song1”, “song2”, “song3”, “song4”, “song5”, “song6”, “song7”, “song8”];

//randomize song
	var random = song[Math.floor(Math.random() * song.length)];


	var letter;
	var num;
	var bad;
	var good;

//how many guesses can the player get wrong? 10.
	var goodGuesses;
	for (var a = 0; a <10; a++)

//player picks a letter
	var guess = prompt (“Guess a letter: “);
		var badGuesses = 0;

//compare each letter player gives with letters in chosen word
		for (var i =  0; i < random.length; i++) {
			var count = 0; 
//if the letter doesn’t match a letter in chosen word then compare with all other letters
			if (random.charAt(count) !== guess){
				letter =i;
				count ++;
//also make sure that player doesn’t get double penalty for incorrect guesses
				for (var j = i+1; j <= bad.length; j++) {
					if (letter[i] == letter[j]) {
						return false; 
					}
//also show the player all incorrect guesses and keep tabs on bad guess score
				bad += letter + “, “;
				display bad;
				badGuesses++
				}
			}
//if the user guesses a letter correctly then add that letter to the correct placement on the guessed word and display for the user. 
			else { 
				good.length(count) += i;
				count ++;
				display good;
			}
		}
//pull out the last good guess from player and save it outside the loop
 		goodGuesses = good;
	}

//compare the chosen word with the player’s final word if they match, they win and their score increase. They can choose to go again.
	if (goodGuesses == random) {
		“You Win”
		game ++;
		var yes = true; 
		if (yes) {
			won = true;
		}
		else { 
			won = false;
	}
//if the words don’t match, the player loses, but has the option to play again. 
	else { 
		“You Lose”
		Would you like to play again?
		var yes = true;
		if (yes) {
			won = true;
		}
		else {
			won = false;
		}
	}
}