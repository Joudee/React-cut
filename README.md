# React-cut

##Intention
JavaScript library for cutting images in React both width mobile and pc.It provides flexible operation on cutting.(At present,it just support for mobild.I will promote it in version 1.0.1.)


##Installation

```sh
npm install react-cut
```

## Usage

```js
import Cut from 'react-cut'

let config = {
	url:'https://img.dev.tusoapp.com/896d71e4-6b1f-403f-84a1-9eacf82a4438.jpg', // the image you want to cut
	imgScale:false,	//	if true ,user can scale image
	frameScale:false,	// if true , user can scale the cutting frame
	frameWidth:300,		// the cutting frame's default width
	frameHeight:300,	// the cutting frame's default height
	minW:200,	//	the cutting frame's min width
	minH:200,	//	the cutting frame's min height
	width:document.body.clientWidth  //Cut's component's width
}

<Cut config={config}></Cut>
```

## Method
You can use [getCutImage()]() to get information after click cutting button.This method has two arguements.
```js
getCutImage:function(base64,file){
	// base64 of cutting image
	//file of cutting image , you can convert it to form and send to server.
},
```

##[Example](http://www.joudee.com/reactCut/index.html)