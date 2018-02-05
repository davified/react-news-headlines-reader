# React News Headlines Reader

In this assignment, you are going to create your own news reader!

Prerequisite knowledge:
- React and testing in React
- HTTP requests with `fetch`
- promises (`.then()`)
- `react-router`

Steps for part 1 (fetching and rendering news articles):
- Register for API key at https://newsapi.org/
- Try making GET requests using Insomnia (available as a Chrome Extension)
- `yarn add whatwg-fetch`
- In the App component, make a HTTP GET request using `fetch` and store the articles in the response in the component's state. The http request should be made in `componentDidMount()`
- Create children components to render each article (it's up to you how to slice/dice/design it) 

Steps for part 2 (react-router):
- install `react-router`
- On clicking on the article, route the user to a **detail** view for a single article
- On clicking the "React News Headlines Reader" title, route user back to the **master** view of all articles

#### News API response format
```json
{
	"status": "ok",
	"totalResults": 34962,
	"articles": [
		{
			"source": {
				"id": null,
				"name": "Dribbble.com"
			},
			"author": "Fishfinger",
			"title": "Olympics",
			"description": "Russia has been banned from the 2018 Pyeongchang Winter Olympics after evidence emerged of widespread doping but some of its athletes will be allowed to compete under the tag of \"Olympic Athlete of Russia\", the IOC said on Tuesday",
			"url": "https://dribbble.com/shots/3941673-Olympics",
			"urlToImage": "https://cdn.dribbble.com/users/976907/screenshots/3941673/cycle.png",
			"publishedAt": "2017-11-12T12:44:56Z"
		},
    // ... more article objects
  ]
}
```

---
Copyright (c) 2018 ThoughtWorks. For personal use and training purposes only; not to be copied or distributed without further approval.
