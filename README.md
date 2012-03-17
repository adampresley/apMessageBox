# apMessageBox

### What it Is
apMessageBox is a JavaScript wrapper object around jQuery UI's dialog box. It is
intended to be used like a message box, or alert box to display alert information,
such as errors, warnings, and general info.


### Example
```
&lt;script&gt;
/*
 * Set the paths to images so apMessageBox knows where to find them.
 */
apMessageBox.errorImage = "/resources/images/error-32x32.png";
apMessageBox.informationImage = "/resources/images/information-32x32.png";

/*
 * Pretend we have a button, and when we click it a message is shown
 */
$("#myErrorButton").on("click", function() {
	apMessageBox.error({ message: "Ooops! An error has occured! "});
});

$("#myInfoButton").on("click", function() {
	apMessageBox.information({ message: "Well howdy!" });
});
&lt;/script&gt;
```


### License
Copyright 2012 Adam Presley. All rights reserved.

Redistribution and use in source and binary forms, with or without
modification, are permitted provided that the following conditions are met:

1. Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.

2. Redistributions in binary form must reproduce the above copyright notice,
   this list of conditions and the following disclaimer in the documentation
   and/or other materials provided with the distribution.

THIS SOFTWARE IS PROVIDED BY Adam Presley "AS IS" AND ANY EXPRESS OR IMPLIED
WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF
MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO
EVENT SHALL Adam Presley OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT,
INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT
LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR
PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
