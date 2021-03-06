---
layout: post
title: Creating a custom scrollbar with scrolljs
tags: [javascript,projects]
---
Over the past couple of years I have run into several cases were I needed to interact with the dom properties related to scrolling an element. I found my self wishing / searching for library to handle the nuances of the api. So I wrote scrolljs.

Scrolljs aims to make it easy to detect if an element can be scrolled, get the current scroll position and provide utility methods that are commonly needed when building a custom scrollbar. So if you don't see a method that you think others would like please feel free to fork and add it or submit an issue for the feature.


* [view demo - creating a custom scrollbar](/demos/2013-07-02-creating-a-custom-scrollbar-with-scrolljs/)
* [on github.com](https://github.com/jebaird/scrolljs)

### Getting Started

Include scrolljs on your page

	<script src="scroll.js"></script>

Setup a target that has scrollable content. 


	<div id="target">....scrollable content....</div>

Create a scrolljs instance.


	var inst = jebaird.scroll( document.getElementById('target');
	if( inst.scrollable() ){
		alert('i can scroll');
	}

 And that's it. Checkout the code and tests for more documentation and examples.