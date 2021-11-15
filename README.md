# vs-console-snippets README

A snippets pack to make you more productive debugging with JavaScript/Typescript.

Download this extension from the [Visual Studio Code Marketplace](https://marketplace.visualstudio.com/items?itemName=jbaro.vs-console-snippets)

## Features

Simply start to write <kbd>log</kbd> (or <kbd>con</kbd>) and next char will define type of log

### logClipboard
Logs content of clipboard.

1. <kbd>⌘ Command</kbd> <kbd>c</kbd> `!true===false`
2. On new line start typing <kbd>logc</kbd>
3. First suggest option should be `logClipboard`
4. <kbd>tab</kbd> and get:
```javascript
console.log('!true===false',!true===false);
```
![logClipboard](https://raw.githubusercontent.com/jbarog/vs-console-snippets/master/assets/logClipboard.gif)

### logFunction
Logs function name params and its values under it definition.

1. At the end of a function definition start typing <kbd>logf</kbd>
2. First suggest option should be `logFunction`
3. <kbd>tab</kbd> and get:
```javascript
console.log('foo(param1, param2)', param1, param2);
```
![logFunction](https://raw.githubusercontent.com/jbarog/vs-console-snippets/master/assets/logFunct.gif)

It supports many function definitions like:
* `function foo(param1, param2) {`
* `const foo = (param1, param2) => {`
* `foo: function(param1, param2) {`

![logFunction 1](https://raw.githubusercontent.com/jbarog/vs-console-snippets/master/assets/logFunct2.gif)

![logFunction 2](https://raw.githubusercontent.com/jbarog/vs-console-snippets/master/assets/logFunct3.gif)

![logFunction 3](https://raw.githubusercontent.com/jbarog/vs-console-snippets/master/assets/logFunct4.gif)

### log--
Logs a sepparator in order to differentiate log lines or find a particular log line.

1. Anywhere start typing <kbd>log-</kbd>
2. First suggest option should be `log--`
3. <kbd>tab</kbd> and get:
```javascript
console.log('------------------');
```
![log--](https://raw.githubusercontent.com/jbarog/vs-console-snippets/master/assets/log--.gif)

### logLineNumber
Logs current line number.

1. Anywhere start typing <kbd>logl</kbd>
2. First suggest option should be `logLineNumber`
3. <kbd>tab</kbd> and get:
```javascript
console.log('line 38');
```
![logLineNumber](https://raw.githubusercontent.com/jbarog/vs-console-snippets/master/assets/logLineNumber.gif)

### logAssigment
Logs the value of a varible after its definition.

1. At the end of a variable definition start typing <kbd>loga</kbd>
2. First suggest option should be `logAssigment`
3. <kbd>tab</kbd> and get:
```javascript
console.log('foo', foo);
```
![logAssigment](https://raw.githubusercontent.com/jbarog/vs-console-snippets/master/assets/logAssigment.gif)

### logThisLine
Logs the value of a varible after its definition.

1. At the end of any line start typing <kbd>logt</kbd>
2. First suggest option should be `logThisLine`
3. <kbd>tab</kbd> and get:
```javascript
console.log('CURRENT LINE TEXT');
```
![logThisLine](https://raw.githubusercontent.com/jbarog/vs-console-snippets/master/assets/logThisLine.gif)

### Generic console snippets

#### conDebug
1. Anywhere start typing <kbd>cond</kbd>
2. First suggest option should be `conDebug`
3. <kbd>tab</kbd> and get:
```javascript
console.
```
with a list of console methods.
4. Select one and use <kbd>tab</kbd> to navigate.
![conDebug](https://raw.githubusercontent.com/jbarog/vs-console-snippets/master/assets/conDebug.gif)

## Requirements

Zero configuration: works out of the box.

## Release Notes

Users appreciate release notes as you update your extension.

### 1.0.0

First release

### 1.0.1

Fix README

### 1.0.2

Fix logAssigment and logFunction

### 1.0.3

Add indentation on logFunction snippet
