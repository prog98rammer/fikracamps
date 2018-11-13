# fikracamps task-w2
----------------

## Description
--------
Use NodeJS read 'flower.txt' and:
1. Count the number of rows.
2. List the flower name that start with letter 'S'.
3. Count the number of flower that not start with letter 'S'.
4. List the flower start with first letter of your name if your name start with 'S' use second letter.
5. List all the flower the name length is 5.


## Libraries I used.
- NodeJS
- Underscore

## simple filter that did all the task :)
```js
_.filter(names, (name) => {
	if(_.contains(name[0], 'S')) {
		allData.namesStartWithS.push(name)
	} else {

		/**
		 * count the number of names that not start with S letter
		 */
		allData.numberOfNamesThatNotStartWithS += 1;


		if (_.contains(name[0], 'K')) {
			/**
			 * Store names that starts with my letter K
			 */
			allData.namesStartWithMyLetterK.push(name)
		}
	}


	/**
	 * list all names that name length is 5
	 */
	if (name.length === 5) {
		allData.namesLengthFive.push(name)
	}
})
```
