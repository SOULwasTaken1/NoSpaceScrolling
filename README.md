# No Space Scroll
### Why did i make this?
I found it annoying when im watching youtube shorts and try to pause using spacebar but it scrolls to the next video.
### How to use this?
##### Step 1:
* Go to Extentions (Im using opera GX but any chromium based browsers would work)
* Chromium based browsers are: Chrome, Firefox, Edge, Brave, opera etc.

![Alt text](/images/step1.png?raw=true "Optional Title")

##### step 2:
* turn on Developer mode

![Alt text](/images/image.png?raw=true "Optional Title")

![Alt text](/images/step2.png?raw=true "Optional Title")

##### step 3
* Click Load Unpacked and select the folder with the script and the json file

![Alt text](/images/step3.png?raw=true "Optional Title")

### Extra
* You can do it for other sites too. 
* In manifest.json file
```js
 . . .
    },
    "content_scripts": [{
        "matches": ["https://www.youtube.com/*"], // add more websites here and separate them with comma //
        "js": ["script.js"]
    }]

}
```
* Why is there a *?
* This * makes it so There could be anything in the star's place and it will still work
* example:
```js
    },
    "content_scripts": [{
        "matches": [
        "https://www.youtube.com/*",
        "https://www.website.org/something/*",
        "https://www.example.com/*"
        ],
        "js": ["script.js"]
    }]

}

```
