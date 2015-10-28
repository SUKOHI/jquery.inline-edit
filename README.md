# jquery.inline-edit
A jQuery plugin to manage inline edit.  
I developed this package because I was inspired [jQuery.editable](http://shokai.github.io/jQuery.editable/) which is really useful but unfortunately which seems not to support class-name selector.  
Thank you, [shokai](http://shokai.github.io/)!

Requirements
====

* [jQuery](https://jquery.com/)

Installation
=====
Using bower is the simplest way.

    bower install jquery.inline-edit --save-dev

Usage
====

**Basic Way**

    $('.inline-edit').inlineEdit('click');
    
* You can change `click` to other event name like `mouseover`.
    
**with Callback**
    
    $('.inline-edit').inlineEdit('click', function(text, originalText, element){
                                                   
        // Do something..

    });

**with Options**

    var options = {
        attributes: {
            id: 'input-id',
            class: 'input-class-1 input-class-2 input-class-3',
            style: 'background:#ffe;'
        }
    };
    $('.inline-edit').inlineEdit('click', options, function(text, originalText, element){
                                                            
        // Do something..

    });

**Using Textarea**

    $('.inline-edit').inlineEdit('click', {
        type: 'textarea',
        attributes: {
            rows: 10
        }
    });

License
====

This package is licensed under the MIT License.

Copyright 2015 Sukohi Kuhoh
