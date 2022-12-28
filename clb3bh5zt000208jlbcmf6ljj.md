# alert, prompt and confirm in JavaScript

## alert()
The alert() method displays an alert box with a message and an OK button. The alert() method is used when we want to inform user regarding anything. The alert box takes the focus away from the current window, and forces the user to read the message first.

### Syntax-
`alert(message)`
```
alert("Hello! This is an alert")
```

### Output-

![Screenshot 2022-11-30 122720.jpg](https://cdn.hashnode.com/res/hashnode/image/upload/v1669791451352/1559eTayz.jpg align="left")

## confirm()
The confirm() method displays a dialog box with a message, an OK button, and a Cancel button. The confirm() method returns true if the user clicked "OK", otherwise false.

A confirm box is often used if you want the user to verify or accept something. It also prevents the user from accessing other parts of the page until the box is closed.

### Syntax-
`confirm(message)`
```
confirm("Do you still want to delete?");
```

### Output-

![Screenshot 2022-11-30 124357.jpg](https://cdn.hashnode.com/res/hashnode/image/upload/v1669792489962/SZg_r_d35.jpg align="left")

## prompt()
The prompt() method displays a dialog box with a message that prompts the user for input. The prompt() method returns the input value if the user clicks "OK", otherwise it returns null or default value if given. User may also click on cancel, then nothing will be returned.

A prompt box is used if we want the user to input a value. When a prompt box pops up, the user will have to click either "OK" or "Cancel" to proceed. It prevents the user from accessing other parts of the page until the box is closed.

### Syntax-
`prompt(text, defaultText)`
```
prompt("Enter your name?", "guest");
```
### Output-

![Screenshot 2022-11-30 123424.jpg](https://cdn.hashnode.com/res/hashnode/image/upload/v1669791876994/z-g54Bnei.jpg align="left")

If I enter the name "Rohit", then,

![Screenshot 2022-11-30 123629.jpg](https://cdn.hashnode.com/res/hashnode/image/upload/v1669792006809/dTrVIOCzO.jpg align="left")

I hope you find this post helpful!