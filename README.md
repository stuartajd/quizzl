# Quizzler
VueJS based Quiz system.

Import questions from JSON and formats & returns end question result.

Demo: https://dev.stuartd.co.uk/quizzler/

## Parameters

The JSON is a standard format and has the following parameters.

question - string - The question that will be displayed on the page. (Does not require trailing question mark)
answers - Array of strings - All answers as they appear on the page. Must have atleast 1 answer; can have as many as required.
correct - integer - The index to the correct answer from the answers array.
image (not required) - string - Image to display along with the current question. (Max 150px x 250px).

## Simple question example JSON
```javascript
[{
	"question": "What is an animal starting with the letter C",
	"answers": [ "cat", "dog", "sheep", "monkey"],
	"correct": 0
}]

```

## Multiple questions example JSON

```javascript
[{
	"question": "What is the capital of France",
	"answers": [ "London", "Paris", "Rome" ],
	"correct": 1
},
{
	"question": "How many continents are there in the world",
	"answers": [ "1", "4", "5", "7" ],
	"correct": 3
},
{
	"question": "How many legs does a spider typically have",
	"answers": [ "7", "8" ],
	"correct": 1
}]

```