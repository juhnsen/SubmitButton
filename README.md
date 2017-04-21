## SubmitButto

[![Travis](https://img.shields.io/badge/download-1.0.1-brightgreen.svg)](https://bintray.com/unstoppable/maven/submitbutton/1.0.1)


README: [English](https://github.com/Someonewow/SubmitButton/blob/master/README.md) | [中文](https://github.com/Someonewow/SubmitButton/blob/master/README-zh.md)


>It's a submit button whit a fun animation for Android.

## Demo

![submit succeed](http://oop9jkflc.bkt.clouddn.com/submitbutton_01.gif)

![submit failed](http://oop9jkflc.bkt.clouddn.com/submitbutton_02.gif)

## Getting Started

##### 1.Specify SubmitButton as a dependency in your build.gradle file;

	dependencies {
		'''
    	compile 'com.unstoppable:submitbutton:1.0.1'
	}

##### 2.Add SubmitButton to the layout file;

	<com.unstoppable.submitbuttonview.SubmitButton
        android:id="@+id/submitbutton"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content" />

##### 3.Attribute

| name          | format   | description                                           |default  |    
|:--------------|:-----    |:------------------------------------------------------|:--------|
|buttonColor    |color     |set the button theme color                             |#19CC95  |
|buttonText     |String    |set the button text                                    |null     |
|buttonTextSize |dimension |set the button text size                               |15sp     |
|succeedColor   |color     |set the button color after the submission is successful|#19CC95  |
|failedColor    |color     |set the button color after the submission fails        |#FC8E34  |

##### 4.Method
	
	 /**
     * Pass the results to show different feedback results
     *
     * @param boolean isSucceed 
     */
	mSubmitView.doResult(isSucceed);

	 /**
     * Reset SubmitButton 
     */
	mSubmitView.reset();

## License

	Copyright 2017 Unstoppable

	Licensed under the Apache License, Version 2.0 (the "License");
	you may not use this file except in compliance with the License.
	You may obtain a copy of the License at

	   http://www.apache.org/licenses/LICENSE-2.0

	Unless required by applicable law or agreed to in writing, software
	distributed under the License is distributed on an "AS IS" BASIS,
	WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
	See the License for the specific language governing permissions and
	limitations under the License.