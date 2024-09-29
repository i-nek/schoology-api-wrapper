# schoology-wrapper

A simple npm package to implement the [Schoology API](https://developers.schoology.com/api/) using javascript.

### Required dependencies:
```bash
npm i axios
```

### To install package:

```bash
bun install [package-name]
```

# Usage:
```javascript
import SchoologyClient from './index';

const schoologyClient = new SchoologyClient(
    '', // consumer_key
    '' // consumer_secret
);

// Authorize
const authorizationUrl = await schoologyClient.getAuthorizationUrl();

// Retrieve Data
const courseData = await schoologyClient.getCourse(7354453829);

courseTest()
 
};
```

This project was created using `bun init` in bun v1.1.28. [Bun](https://bun.sh) is a fast all-in-one JavaScript runtime.
