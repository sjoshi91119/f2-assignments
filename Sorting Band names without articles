You are given an array of band names. You need to sort those band names in lexicographic order excluding any articles('a', 'an', 'the') and list down those names inside ul id='band' tag using the li tag.

Ex:

// suppose an array that contains a list of popular tourise spots
let touristSpots = ['The Virupaksha Temple', 'Victoria Memorial', 'Tajmahal'];

// So here the lexicographically sorted order is (without articles)---
touristSpots = ['Tajmahal', 'Victoria Memorial', 'The Virupaksha Temple'];

------------------------------++++++++++++++++++++++++++++++++++=---------------------------------------
-----------------------------==============================-----------------------------------------

//your code here
	const bandNames = ['The Beatles', 'Led Zeppelin', 'Pink Floyd', 'The Who', 'Aerosmith', 'Rolling Stones', 'Queen', 'Anthrax', 'Black Sabbath'];

		function sortBands(bands) {
			const articles = ['the', 'a', 'an'];
			const sortedBands = bands.sort(function(a, b) {
				const nameA = a.toLowerCase().replace(/^(the|an|a)\s+/, '');
				const nameB = b.toLowerCase().replace(/^(the|an|a)\s+/, '');
				if (nameA < nameB) {
					return -1;
				}
				if (nameA > nameB) {
					return 1;
				}
				return 0;
			});
			return sortedBands;
		}

		const sortedBands = sortBands(bandNames);

		const bandList = document.getElementById("band");
		sortedBands.forEach(function(band) {
			const li = document.createElement("li");
			li.appendChild(document.createTextNode(band));
			bandList.appendChild(li);
		});
